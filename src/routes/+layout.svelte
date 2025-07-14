<script>
    let { children } = $props();
    import "../app.css";
    import Footer from "../components/footer/footer.svelte";
    import Navbar from "../components/navbar/navbar.svelte";
</script>
<div class="flex flex-col min-h-screen">
	<Navbar />
	<main class="flex-1">
        {@render children()}
	</main>
	<Footer />
</div>

<style lang="postcss">
    @reference "tailwindcss";
    :global(html) {
        background-color: theme(--color-white);
    }
</style>