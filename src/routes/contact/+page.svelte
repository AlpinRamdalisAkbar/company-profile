<section class="bg-gradient-to-br from-blue-50 to-white min-h-screen py-16">
    <div class="max-w-7xl mx-auto px-4">
        
        <!-- Header -->
        <div class="text-center mb-12">
            <h1 class="text-4xl md:text-5xl font-bold text-blue-800 inter-big">Contact Pokémon Co. Ltd</h1>
            <p class="text-lg text-gray-600 mt-2">Whether you’re a trainer, partner, or just a fan — we’d love to hear from you!</p>
        </div>

        <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">

            <!-- Contact Info -->
            <div class="space-y-6 text-blue-900">
                <div>
                    <h2 class="text-2xl font-bold mb-2 text-red-600">📍 Office</h2>
                    <p>The Pokémon Company, Tokyo Headquarters<br/>1-2-3 PokéStreet, Kanto, Japan</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold mb-2 text-yellow-500">📞 Phone</h2>
                    <p>+81-3-1234-5678</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold mb-2 text-green-500">✉️ Email</h2>
                    <p>info@pokemoncoltd.com</p>
                </div>

                <div>
                <h2 class="text-2xl font-bold mb-2 text-pink-500">🔗 Social</h2>
                    <div class="flex space-x-4 mt-2 text-xl">
                        <a href="#" class="hover:text-yellow-500">Facebook</a>
                        <a href="#" class="hover:text-yellow-500">Twitter</a>
                        <a href="#" class="hover:text-yellow-500">Instagram</a>
                    </div>
                </div>
            </div>

            <!-- Contact Form -->
            <form class="bg-white rounded-lg shadow-md p-8 space-y-6" on:submit|preventDefault={() => alert('Message sent! (placeholder)')}>
                <h2 class="text-2xl font-semibold text-blue-800 mb-4">Send Us a Message</h2>

                <div>
                    <label for="name" class="block mb-2 text-sm font-medium text-blue-700">Name</label>
                    <input type="text" id="name" class="w-full px-4 py-2 border rounded-md focus:ring-2 focus:ring-blue-300 shadow" required />
                </div>

                <div>
                    <label for="email" class="block mb-2 text-sm font-medium text-blue-700">Email</label>
                    <input type="email" id="email" class="w-full px-4 py-2 border rounded-md focus:ring-2 focus:ring-blue-300 shadow" required />
                </div>

                <div>
                    <label for="message" class="block mb-2 text-sm font-medium text-blue-700">Message</label>
                    <textarea id="message" rows="5" class="w-full px-4 py-2 border rounded-md focus:ring-2 focus:ring-blue-300 shadow" required></textarea>
                </div>

                <button type="submit" class="bg-amber-300 text-black px-6 py-2 rounded-md hover:bg-red-600 transition shadow">
                    Send Message
                </button>
            </form>
        </div>
    </div>
</section>
