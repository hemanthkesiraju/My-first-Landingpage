# My-first-Landingpage
Project Name: My-first-Landingpage – VoltCore: The Ultimate Charger
Purpose: A modern, responsive landing page for a fictional fast-charging device
Tech Stack:
HTML5
Tailwind CSS
Vanilla JavaScript
Inter font
Features:
Fully responsive design (mobile → desktop)
Dark theme with yellow accents
Smooth scrolling between sections
Hover effects & animations
Single-file structure (index.html)
File:
index.html → contains all HTML, CSS, and JS
How to Run:
Just open index.html in any browser (no server needed)
Customization:
Change colors via Tailwind classes
Edit text directly in HTML
Replace placeholder images with product images
Contact:
Email: 24eu08023@vrsec.ac.in
Phone: 91772 27514
Address: Sri City, Chennai

CODE:
<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>VoltCore - The Ultimate Charger</title>
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Inter Font -->
    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap">
    <style>
        body {
            font-family: 'Inter', sans-serif;
        }
        /* Custom Keyframes for a subtle glow effect */
        @keyframes pulse-glow {
            0%, 100% {
                box-shadow: 0 0 10px rgba(255, 204, 0, 0.4), 0 0 20px rgba(255, 204, 0, 0.2);
            }
            50% {
                box-shadow: 0 0 20px rgba(255, 204, 0, 0.8), 0 0 40px rgba(255, 204, 0, 0.4);
            }
        }
        .cta-pulse {
            animation: pulse-glow 2s infinite ease-in-out;
        }
    </style>
</head>
<body class="bg-zinc-950 text-gray-200">

    <!-- Navigation Bar -->
    <nav class="fixed top-0 left-0 w-full z-50 bg-black/70 backdrop-blur-md shadow-lg">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <a href="#" class="font-bold text-2xl text-yellow-400 rounded-lg p-2 transition-colors hover:text-yellow-600">VoltCore</a>
            <div class="space-x-8 hidden md:flex">
                <a href="#hero" class="text-gray-400 hover:text-yellow-400 transition-colors">Home</a>
                <a href="#why-voltcore" class="text-gray-400 hover:text-yellow-400 transition-colors">Why VoltCore</a>
                <a href="#features" class="text-gray-400 hover:text-yellow-400 transition-colors">Features</a>
                <a href="#testimonials" class="text-gray-400 hover:text-yellow-400 transition-colors">Testimonials</a>
                <a href="#faq" class="text-gray-400 hover:text-yellow-400 transition-colors">FAQ</a>
                <a href="#footer" class="text-gray-400 hover:text-yellow-400 transition-colors">Contact</a>
            </div>
            <!-- Mobile Menu -->
            <button id="menu-button" class="md:hidden text-gray-400 hover:text-yellow-400 focus:outline-none">
                <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
                </svg>
            </button>
        </div>
        <div id="mobile-menu" class="hidden md:hidden bg-black/90 backdrop-blur-md px-4 pb-4 transition-all duration-300 ease-in-out">
            <a href="#hero" class="block py-2 text-gray-400 hover:text-yellow-400">Home</a>
            <a href="#why-voltcore" class="block py-2 text-gray-400 hover:text-yellow-400">Why VoltCore</a>
            <a href="#features" class="block py-2 text-gray-400 hover:text-yellow-400">Features</a>
            <a href="#testimonials" class="block py-2 text-gray-400 hover:text-yellow-400">Testimonials</a>
            <a href="#faq" class="block py-2 text-gray-400 hover:text-yellow-400">FAQ</a>
            <a href="#footer" class="block py-2 text-gray-400 hover:text-yellow-400">Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <header id="hero" class="relative overflow-hidden bg-gradient-to-br from-zinc-900 via-zinc-950 to-black py-16 md:py-32 flex flex-col md:flex-row items-center justify-center min-h-screen pt-24">
        <div class="container mx-auto px-6 text-center md:text-left flex flex-col md:flex-row items-center justify-between">
            <div class="md:w-1/2 mb-10 md:mb-0 md:pr-16">
                <!-- CRO Change: More specific and benefit-driven headline -->
                <h1 class="text-5xl md:text-7xl font-extrabold text-white leading-tight mb-4 tracking-tight">
                    Get a Full Day of Power <br> in 30 Minutes.
                </h1>
                <!-- CRO Change: Clear value proposition -->
                <p class="text-xl text-gray-400 mb-8 max-w-lg mx-auto md:mx-0">
                    The VoltCore Pro's groundbreaking technology delivers an 80% charge in just 30 minutes, keeping you connected without the wait.
                </p>
                <!-- CRO Change: More benefit-oriented CTA button text -->
                <a href="javascript:void(0);" class="inline-block px-10 py-5 text-lg font-bold text-zinc-950 bg-yellow-400 rounded-full shadow-lg transition-all duration-300 ease-in-out transform hover:scale-110 hover:shadow-2xl active:scale-95 cta-pulse">
                    Claim Your Fast Charger Now
                </a>
                <!-- CRO Change: Adding trust signals below the CTA -->
                <div class="flex items-center justify-center md:justify-start space-x-4 mt-6">
                    <span class="text-sm text-gray-400 flex items-center">
                        <svg class="h-5 w-5 mr-2 text-green-400" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm3.707-9.293a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd" />
                        </svg>
                        Free Shipping on All Orders
                    </span>
                    <span class="text-sm text-gray-400 flex items-center">
                        <svg class="h-5 w-5 mr-2 text-green-400" fill="currentColor" viewBox="0 0 20 20">
                            <path fill-rule="evenodd" d="M10 18a8 8 0 100-16 8 8 0 000 16zm-1.414-1.414l4-4a1 1 0 00-1.414-1.414L10 12.586 7.414 10a1 1 0 10-1.414 1.414l3 3z" clip-rule="evenodd" />
                        </svg>
                        30-Day Money-Back Guarantee
                    </span>
                </div>
            </div>
            <div class="md:w-1/2 flex justify-center mt-12 md:mt-0">
                <!-- CRO Change: More specific placeholder text for a powerful product shot -->
                <img src="https://placehold.co/600x400/18181B/FACC15?text=VOLTCORE+CHARGER+IN+HAND" alt="VoltCore Pro Charger in hand, dynamic product shot" class="w-full max-w-lg rounded-2xl shadow-2xl transform transition-transform duration-500 hover:scale-105">
            </div>
        </div>
    </header>

    <!-- Why VoltCore Section -->
    <section id="why-voltcore" class="bg-zinc-800 py-16 md:py-24">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl font-bold text-gray-100 mb-4">Why Choose VoltCore?</h2>
            <p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto">
                We're not just a charger—we're an investment in speed, safety, and a seamless digital life.
            </p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- CRO Change: Rephrased for a stronger benefit-driven message -->
                <div class="bg-zinc-900 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">Recharge in Minutes</h3>
                    <p class="text-gray-400 text-sm">
                        Our charging technology reduces your wait time from hours to minutes, getting you back to what matters most.
                    </p>
                </div>
                <!-- CRO Change: Rephrased for a stronger benefit-driven message -->
                <div class="bg-zinc-900 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.018A12.001 12.001 0 0012 21a12.001 12.001 0 00-7.618-17.018" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">Worry-Free Charging</h3>
                    <p class="text-gray-400 text-sm">
                        Advanced thermal regulation and surge protection keeps your devices safe, protecting your valuable investments.
                    </p>
                </div>
                <!-- CRO Change: Rephrased for a stronger benefit-driven message -->
                <div class="bg-zinc-900 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 6l3 1m3 0l6-1m-6 1a3 3 0 100-6m0 6a3 3 0 110-6m0 6h4a2 2 0 012 2v2m0-4a2 2 0 00-2-2m-4 4h4" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">One for All Your Devices</h3>
                    <p class="text-gray-400 text-sm">
                        Our universal compatibility means you only need one charger, reducing clutter and hassle on your desk and in your bag.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Highlights/Feature Section -->
    <section id="features" class="bg-zinc-900 py-16 md:py-24">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl font-bold text-gray-100 mb-4">Key Features</h2>
            <p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto">
                Discover what makes VoltCore the ultimate solution for all your charging needs.
            </p>
            <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-8">
                <!-- CRO Change: More visual and detailed features -->
                <div class="group bg-zinc-950 p-8 rounded-2xl shadow-lg transition-all duration-300 transform hover:scale-105 hover:bg-zinc-800 border border-zinc-800 hover:border-yellow-400">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400 transition-colors duration-300 group-hover:text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">30-Minute Charge</h3>
                    <p class="text-gray-400 text-sm">
                        Experience our proprietary technology that gets your battery from 0% to 50% in under 30 minutes.
                    </p>
                </div>
                <!-- Feature 2 -->
                <div class="group bg-zinc-950 p-8 rounded-2xl shadow-lg transition-all duration-300 transform hover:scale-105 hover:bg-zinc-800 border border-zinc-800 hover:border-yellow-400">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400 transition-colors duration-300 group-hover:text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m5.618-4.018A12.001 12.001 0 0012 21a12.001 12.001 0 00-7.618-17.018" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">Multi-Device Power</h3>
                    <p class="text-gray-400 text-sm">
                        The VoltCore intelligently adapts to your device, providing optimal power for smartphones, tablets, and even laptops.
                    </p>
                </div>
                <!-- Feature 3 -->
                <div class="group bg-zinc-950 p-8 rounded-2xl shadow-lg transition-all duration-300 transform hover:scale-105 hover:bg-zinc-800 border border-zinc-800 hover:border-yellow-400">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400 transition-colors duration-300 group-hover:text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20 7l-8-4-8 4m16 0l-8 4m8-4v10a2 2 0 01-2 2h-4a2 2 0 01-2-2V7m-4 0v10a2 2 0 002 2h2m-4 4h4m-8-4h4m-12 0h4m-8-4a2 2 0 012-2h4a2 2 0 012 2v2a2 2 0 002 2h2a2 2 0 002-2v-2a2 2 0 012-2h4a2 2 0 012 2v2a2 2 0 002 2h2a2 2 0 002-2v-2" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">Military-Grade Durability</h3>
                    <p class="text-gray-400 text-sm">
                        Built with an aerospace aluminum shell and reinforced internal components to withstand daily wear and tear.
                    </p>
                </div>
                <!-- Feature 4 -->
                <div class="group bg-zinc-950 p-8 rounded-2xl shadow-lg transition-all duration-300 transform hover:scale-105 hover:bg-zinc-800 border border-zinc-800 hover:border-yellow-400">
                    <div class="flex justify-center mb-4">
                        <svg class="h-14 w-14 text-yellow-400 transition-colors duration-300 group-hover:text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4m-7 4a5 5 0 11-10 0 5 5 0 0110 0z" />
                        </svg>
                    </div>
                    <h3 class="text-xl font-bold text-gray-100 mb-2">Intelligent Safety Chip</h3>
                    <p class="text-gray-400 text-sm">
                        Our smart chip automatically detects your device's charging state and prevents overcharging and overheating.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Testimonials Section -->
    <section id="testimonials" class="bg-zinc-800 py-16 md:py-24">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl font-bold text-gray-100 mb-4">What Our Customers Say</h2>
            <p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto">
                Don't just take our word for it—see what real users have to say about VoltCore.
            </p>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- CRO Change: Added user photo and more specific title for credibility -->
                <div class="bg-zinc-950 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex flex-col items-center mb-4">
                        <img src="https://placehold.co/80x80/28282B/FACC15?text=J.D." alt="Photo of Jane Doe" class="rounded-full w-20 h-20 mb-2">
                        <p class="font-bold text-white">- Jane D.</p>
                        <p class="text-sm text-gray-500">Los Angeles, CA</p>
                    </div>
                    <p class="text-gray-300 mb-4 italic">
                        "I've been using this for a month now, and it's a game-changer. My phone battery used to be a constant worry, but with VoltCore, I'm always at 100% and ready to go!"
                    </p>
                </div>
                <!-- CRO Change: Added user photo and more specific title for credibility -->
                <div class="bg-zinc-950 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex flex-col items-center mb-4">
                        <img src="https://placehold.co/80x80/28282B/FACC15?text=J.S." alt="Photo of John Smith" class="rounded-full w-20 h-20 mb-2">
                        <p class="font-bold text-white">- John S.</p>
                        <p class="text-sm text-gray-500">Digital Nomad</p>
                    </div>
                    <p class="text-gray-300 mb-4 italic">
                        "As a frequent traveler, I need gear that's reliable. The VoltCore is compact, powerful, and charges my laptop and phone at the same time. A must-have!"
                    </p>
                </div>
                <!-- CRO Change: Added user photo and more specific title for credibility -->
                <div class="bg-zinc-950 p-8 rounded-2xl shadow-lg border border-zinc-700">
                    <div class="flex flex-col items-center mb-4">
                        <img src="https://placehold.co/80x80/28282B/FACC15?text=E.W." alt="Photo of Emily White" class="rounded-full w-20 h-20 mb-2">
                        <p class="font-bold text-white">- Emily W.</p>
                        <p class="text-sm text-gray-500">Creative Professional</p>
                    </div>
                    <p class="text-gray-300 mb-4 italic">
                        "The safety features are incredible. My last charger got so hot, but this one stays perfectly cool. I finally have peace of mind while charging overnight."
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- CRO Change: Added new FAQ section to reduce friction and answer common questions -->
    <section id="faq" class="bg-black py-16 md:py-24">
        <div class="container mx-auto px-6 text-center">
            <h2 class="text-4xl font-bold text-gray-100 mb-4">Frequently Asked Questions</h2>
            <p class="text-lg text-gray-400 mb-12 max-w-2xl mx-auto">
                Got questions? We have answers.
            </p>
            <div class="max-w-3xl mx-auto text-left">
                <!-- FAQ Item 1 -->
                <div class="bg-zinc-900 p-6 rounded-lg mb-4 shadow-md">
                    <h3 class="text-xl font-semibold text-white mb-2">Is VoltCore compatible with my device?</h3>
                    <p class="text-gray-400">
                        Yes! VoltCore Pro uses a universal USB-C PD (Power Delivery) port, making it compatible with all major smartphones, tablets, and laptops.
                    </p>
                </div>
                <!-- FAQ Item 2 -->
                <div class="bg-zinc-900 p-6 rounded-lg mb-4 shadow-md">
                    <h3 class="text-xl font-semibold text-white mb-2">How long does shipping take?</h3>
                    <p class="text-gray-400">
                        We offer free standard shipping which typically takes 3-5 business days. You will receive a tracking number via email once your order has shipped.
                    </p>
                </div>
                <!-- FAQ Item 3 -->
                <div class="bg-zinc-900 p-6 rounded-lg mb-4 shadow-md">
                    <h3 class="text-xl font-semibold text-white mb-2">Do you offer a warranty?</h3>
                    <p class="text-gray-400">
                        Absolutely. All VoltCore products come with a 1-year limited warranty covering manufacturing defects.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- CRO Change: Added a repeated CTA to capture users who have scrolled through the page -->
    <section class="bg-zinc-800 py-16 md:py-24 text-center">
        <div class="container mx-auto px-6">
            <h2 class="text-4xl font-bold text-gray-100 mb-4">Ready to Change the Way You Charge?</h2>
            <p class="text-lg text-gray-400 mb-8 max-w-2xl mx-auto">
                Join thousands of satisfied customers who are already experiencing the power of VoltCore. Don't wait, get yours today!
            </p>
            <a href="javascript:void(0);" class="inline-block px-10 py-5 text-lg font-bold text-zinc-950 bg-yellow-400 rounded-full shadow-lg transition-all duration-300 ease-in-out transform hover:scale-110 hover:shadow-2xl active:scale-95 cta-pulse">
                Order Your VoltCore Now
            </a>
        </div>
    </section>

    <!-- Footer Section -->
    <footer id="footer" class="bg-zinc-950 text-gray-400 py-12">
        <div class="container mx-auto px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8 mb-8">
                <!-- Navigation -->
                <div>
                    <h4 class="font-bold text-lg mb-4 text-white">Navigation</h4>
                    <ul>
                        <li class="mb-2"><a href="#hero" class="hover:text-white transition-colors">Home</a></li>
                        <li class="mb-2"><a href="#why-voltcore" class="hover:text-white transition-colors">Why VoltCore</a></li>
                        <li class="mb-2"><a href="#features" class="hover:text-white transition-colors">Features</a></li>
                        <li class="mb-2"><a href="#testimonials" class="hover:text-white transition-colors">Testimonials</a></li>
                        <li class="mb-2"><a href="#faq" class="hover:text-white transition-colors">FAQ</a></li>
                    </ul>
                </div>
                <!-- Contact -->
                <div>
                    <h4 class="font-bold text-lg mb-4 text-white">Contact Us</h4>
                    <ul>
                        <li class="mb-2">Email: <a href="mailto:24eu08023@vrsec.ac.in" class="hover:text-white transition-colors">24eu08023@vrsec.ac.in</a></li>
                        <li class="mb-2">Phone: <a href="tel:9177227514" class="hover:text-white transition-colors">91772 27514</a></li>
                        <li class="mb-2">Address: sri city ,Chennai.</li>
                    </ul>
                </div>
                <!-- Socials -->
                <div>
                    <h4 class="font-bold text-lg mb-4 text-white">Follow Us</h4>
                    <div class="flex space-x-4">
                        <a href="javascript:void(0);" class="hover:text-yellow-400 transition-colors">
                            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                                <path d="M22 6.98a.997.997 0 00-.77-.77c-1.5-.4-3.1-.6-4.7-.6-1.6 0-3.2.2-4.7.6a.997.997 0 00-.77.77l-.6 2.4a.997.997 0 00.77.77c1.5.4 3.1.6 4.7.6s3.2-.2 4.7-.6a.997.997 0 00.77-.77l-.6-2.4zm-14.7.6c-1.5.4-3.1.6-4.7.6-1.6 0-3.2-.2-4.7-.6a.997.997 0 00-.77-.77l-.6-2.4a.997.997 0 00.77-.77c1.5-.4 3.1-.6 4.7-.6s3.2.2 4.7.6a.997.997 0 00.77.77l-.6 2.4z" />
                                <path d="M12 24a12 12 0 100-24 12 12 0 000 24zM12 2.5a9.5 9.5 0 110 19 9.5 9.5 0 010-19z" />
                                <path d="M12 17.5a5.5 5.5 0 100-11 5.5 5.5 0 000 11zM12 8a4 4 0 110 8 4 4 0 010-8z" />
                            </svg>
                        </a>
                        <a href="javascript:void(0);" class="hover:text-yellow-400 transition-colors">
                            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                                <path d="M22.46 6.09a5.95 5.95 0 00-1.65-.65c-1.5-.3-3.05-.45-4.6-.45H12c-1.55 0-3.1.15-4.6.45a5.95 5.95 0 00-1.65.65C4.2 6.7 3 7.85 3 9.35v5.3c0 1.5 1.2 2.65 2.5 2.9h.1a5.95 5.95 0 001.65.65c1.5.3 3.05.45 4.6.45h2.1c1.55 0 3.1-.15 4.6-.45a5.95 5.95 0 001.65-.65c1.3-.25 2.5-1.4 2.5-2.9v-5.3c0-1.5-1.2-2.65-2.5-2.9zM12 17.5a5.5 5.5 0 110-11 5.5 5.5 0 010 11z" />
                                <path d="M12 11.5a3.5 3.5 0 100 7 3.5 3.5 0 000-7zM12 13a1.5 1.5 0 100-3 1.5 1.5 0 000 3z" />
                            </svg>
                        </a>
                        <a href="javascript:void(0);" class="hover:text-yellow-400 transition-colors">
                            <svg class="h-6 w-6" fill="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                                <path d="M19.63 5.09a.997.997 0 00-.77-.77c-1.5-.4-3.1-.6-4.7-.6s-3.2.2-4.7.6a.997.997 0 00-.77.77l-.6 2.4a.997.997 0 00.77.77c1.5.4 3.1.6 4.7.6s3.2-.2 4.7-.6a.997.997 0 00.77-.77l-.6-2.4z" />
                                <path d="M12 24a12 12 0 100-24 12 12 0 000 24zM12 2.5a9.5 9.5 0 110 19 9.5 9.5 0 010-19z" />
                            </svg>
                        </a>
                    </div>
                </div>
                <!-- Logo & Copyright -->
                <div class="md:text-right">
                    <h4 class="font-bold text-lg mb-4 text-white">VoltCore</h4>
                    <p class="text-sm">
                        &copy; 2024 VoltCore. All rights reserved.
                    </p>
                </div>
            </div>
        </div>
    </footer>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Mobile menu toggle
        const menuButton = document.getElementById('menu-button');
        const mobileMenu = document.getElementById('mobile-menu');

        menuButton.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
        });

        // Close mobile menu when a link is clicked
        mobileMenu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
            });
        });
    </script>
</body>
</html>

