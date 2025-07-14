<!-- MISSION CHECKLIST -->
<div class="bg-blue-400">
    <div class="flex flex-col md:flex-row justify-center items-center gap-12 p-8 max-w-7xl mx-auto">
        <div class="md:w-1/2 flex justify-center">
            <img src="./image/programmer_2.png" alt="Programmer" class="w-72 h-72 md:w-96 md:h-96 object-contain">
        </div>

        <div class="md:w-1/2 text-white">
            <p class="text-lg md:text-xl leading-loose mb-6">
                At Pokémon Co. Ltd, we aim to blend technology and tradition, creating adventures that unite fans through joy and connection.
            </p>

            <ul class="space-y-4">
                {#each [
                    'Deliver world-class interactive entertainment and games.',
                    'Foster imagination and creativity through storytelling.',
                    'Build inclusive communities of passionate fans.',
                    'Expand global influence while honoring Japanese roots.',
                    'Innovate through technology and meaningful design.'
                ] as item}
                    <li class="flex items-start gap-3">
                        <span class="bg-white text-blue-500 rounded-full p-1 shadow">
                            <svg xmlns="http://www.w3.org/2000/svg" class="size-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1.5"
                                d="M9 12.75L11.25 15L15 9.75M21 12A9 9 0 1112 3a9 9 0 019 9z" />
                            </svg>
                        </span>
                        <span>{item}</span>
                    </li>
                {/each}
            </ul>
        </div>
    </div>
</div>