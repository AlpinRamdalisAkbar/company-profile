<script>
    let { photographer, site, linkPhotographer, linkImg } = $props();
</script>

<div class="absolute bottom-2 left-2 bg-black/50 text-white text-xs px-3 py-1 rounded-md">
    Photo by
    <a
        href="{linkPhotographer}"
        target="_blank"
        rel="noopener noreferrer"
        class="underline hover:text-yellow-300"
        >{photographer}</a
    >
    on
    <a
        href="{linkImg}"
        target="_blank"
        rel="noopener noreferrer"
        class="underline hover:text-yellow-300"
        >{site}</a
    >
</div>