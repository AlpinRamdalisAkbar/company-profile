<script>
    let services = [
        {
            iconPath: "M2.25 8.25h19.5M2.25 9h19.5m-16.5 5.25h6m-6 2.25h3m-3.75 3h15a2.25 2.25 0 0 0 2.25-2.25V6.75A2.25 2.25 0 0 0 19.5 4.5h-15a2.25 2.25 0 0 0-2.25 2.25v10.5A2.25 2.25 0 0 0 4.5 19.5Z", // PokéPay
            iconColor: "text-red-600",
            borderColor: "border-yellow-400",
            title: "PokéPay Integration",
            description: "Empower trainers with QR-ready mobile transactions, Poké-points, and secure in-game purchases.",
            btnColor: "bg-yellow-400 hover:bg-yellow-300",
            btnTextColor: "text-red-800"
        },
        {
            iconPath: "m6.75 7.5 3 2.25-3 2.25m4.5 0h3m-9 8.25h13.5A2.25 2.25 0 0 0 21 18V6a2.25 2.25 0 0 0-2.25-2.25H5.25A2.25 2.25 0 0 0 3 6v12a2.25 2.25 0 0 0 2.25 2.25Z", // App icon
            iconColor: "text-blue-500",
            borderColor: "border-blue-400",
            title: "Web & Mobile Adventures",
            description: "From Pokédex apps to real-time battle platforms — scalable and immersive digital experiences await.",
            btnColor: "bg-blue-400 hover:bg-blue-300",
            btnTextColor: "text-white"
        },
        {
            iconPath: "M11.42 15.17L17.25 21A2.652 2.652 0 0 0 21 17.25l-5.877-5.877M11.42 15.17l2.496-3.03c.317-.384.74-.626 1.208-.766M11.42 15.17l-4.655 5.653a2.548 2.548 0 1 1-3.586-3.586l6.837-5.63", // Infra icon
            iconColor: "text-red-500",
            borderColor: "border-red-400",
            title: "Battle-Ready Infrastructure",
            description: "Host, evolve, and scale apps on top-tier cloud setups — built for the modern Pokémon Trainer's ecosystem.",
            btnColor: "bg-red-400 hover:bg-red-300",
            btnTextColor: "text-white"
        }
    ];
</script>
<section class="bg-gradient-to-br from-yellow-100 to-red-100 py-16">
    <div class="max-w-7xl mx-auto px-4 text-center">
        <h2 class="text-4xl md:text-5xl font-bold text-red-700 mb-12 inter-big">
            Our Services
        </h2>

        <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 inter-light">

            {#each services as service}
                <div class={`bg-white text-gray-800 rounded-xl p-8 shadow-lg flex flex-col items-center hover:shadow-xl transition ${service.borderColor}`}>
                    <svg xmlns="http://www.w3.org/2000/svg"
                        class={`w-16 h-16 mb-4 ${service.iconColor}`}
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke-width="1.5"
                        stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" d={service.iconPath} />
                    </svg>

                    <h3 class="text-xl font-semibold mb-2 text-blue-900">{service.title}</h3>
                    <p class="text-sm text-gray-600 mb-6">{service.description}</p>
                    <a href="#"
                        class={`font-semibold px-5 py-2 rounded-md flex items-center gap-2 transition ${service.btnColor} ${service.btnTextColor}`}>
                        Learn More →
                    </a>
                </div>
            {/each}

        </div>
    </div>
</section>