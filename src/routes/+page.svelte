<script>
    import AboutUs from "../components/about/aboutUs.svelte";
    import OurMission from "../components/about/ourMission.svelte";
    import Credit from "../components/credit/credit.svelte";
    import Service from "../components/service/service.svelte";

    let photographer = "Michael Rivera";
    let linkPhotographer = "https://unsplash.com/@monkeydmykie?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash";
    let linkImg = "https://unsplash.com/photos/yellow-and-white-duck-plush-toy-on-green-grass-during-daytime-DypO_XgAE4Y?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash";
    let site = "Unsplash";
</script>
<!-- HERO SECTION -->
<div class="relative w-full h-screen">
    <img src="./image/michael-rivera-DypO_XgAE4Y-unsplash.jpg" alt="Pokemon-themed hero background featuring plush toy" class="w-full h-full object-cover" />

    <div class="absolute inset-0 bg-black/40 flex flex-col items-center justify-center text-center px-4">
        <h1 class="text-white text-5xl sm:text-7xl md:text-9xl font-black tracking-tight drop-shadow-xl">
            Pokémon Co. Ltd
        </h1>
        <p class="text-white text-2xl sm:text-3xl mt-6 italic font-medium drop-shadow">
            "Gotta catch 'em all!"
        </p>
    </div>

    <!-- credit -->
    <Credit {photographer} {site} {linkPhotographer} {linkImg} />
</div>

<!-- ABOUT SECTION -->
<AboutUs />
<!-- MISSION HEADER -->
<div class="bg-blue-900">
    <div class="max-w-7xl mx-auto px-4 py-12 text-center">
        <h2 class="text-white text-5xl font-bold inter-big">Our Mission</h2>
    </div>
</div>
<!-- MISSION CHECKLIST -->
<OurMission />
<!-- SERVICES SECTION -->
<section class="bg-gradient-to-br from-yellow-100 to-red-100 py-16">
    <Service />
</section>