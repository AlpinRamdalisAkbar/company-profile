<script>
    import { page } from '$app/stores';

    $: pathname = $page.url.pathname;

    const navLinks = [
        { href: '/', label: 'Home' },
        { href: '/about', label: 'About' },
        { href: '/service', label: 'Service' },
        { href: '/contact', label: 'Contact' }
    ];

    let isOpen = false;
</script>

<nav class="w-full bg-white sticky top-0 z-50 shadow-md font-sans">
    <div class="max-w-7xl mx-auto px-4 py-4 flex justify-between items-center">
        <!-- Logo -->
        <a href="/" class="flex items-center gap-2 text-red-600 font-black text-2xl tracking-tight">
            <span>Pokémon Co. Ltd</span>
        </a>

        <!-- Burger button (small screens) -->
        <button
            class="sm:hidden text-blue-900 focus:outline-none"
            on:click={() => (isOpen = !isOpen)}
            aria-label="Toggle menu"
        >
            <svg class="w-6 h-6" fill="none" stroke="currentColor" stroke-width="2" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round"
                    d={isOpen
                        ? 'M6 18L18 6M6 6l12 12' // X icon
                        : 'M4 6h16M4 12h16M4 18h16' // Hamburger icon
                    }
                />
            </svg>
        </button>

        <!-- Nav Links -->
        <ul class={`flex-col sm:flex-row sm:flex gap-4 sm:gap-8 items-center text-blue-900 text-lg font-semibold
            ${isOpen ? 'flex absolute top-[72px] left-0 w-full bg-white px-4 py-6 shadow-md sm:static sm:bg-transparent' : 'hidden sm:flex'}
        `}>
            {#each navLinks as link}
                <li>
                    <a
                        href={link.href}
                        class="hover:text-yellow-500 border-b-2 transition-colors duration-300 block py-2"
                        class:text-yellow-500={pathname === link.href}
                        class:border-yellow-500={pathname === link.href}
                        class:border-transparent={pathname !== link.href}>
                            {link.label}
                    </a>
                </li>
            {/each}
        </ul>
    </div>
</nav>
