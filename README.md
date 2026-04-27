<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>IsmaTrott Knokke | Location de trottinettes électriques</title>
    <!-- Tailwind CSS for styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- FontAwesome for Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        sans: ['Poppins', 'sans-serif'],
                    },
                    colors: {
                        'brand-green': '#10B981', // Emerald 500
                        'brand-dark': '#1F2937', // Gray 800
                    }
                }
            }
        }
    </script>
    <style>
        /* Smooth scrolling */
        html { scroll-behavior: smooth; }
        
        /* Hero background with overlay */
        .hero-bg {
            background-image: linear-gradient(rgba(31, 41, 55, 0.7), rgba(31, 41, 55, 0.7)), url('https://images.unsplash.com/photo-1593950315186-76a92975b60c?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 font-sans flex flex-col min-h-screen">

    <!-- Navigation -->
    <nav class="bg-white shadow-md fixed w-full z-50 top-0">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between h-20">
                <div class="flex items-center">
                    <a href="#" class="flex items-center gap-2">
                        <i class="fa-solid fa-bolt text-brand-green text-3xl"></i>
                        <span class="font-bold text-2xl text-brand-dark tracking-tight">Isma<span class="text-brand-green">Trott</span></span>
                    </a>
                </div>
                <div class="hidden md:flex items-center space-x-8">
                    <a href="#accueil" class="text-gray-600 hover:text-brand-green font-medium transition">Accueil</a>
                    <a href="#tarifs" class="text-gray-600 hover:text-brand-green font-medium transition">Tarifs & Services</a>
                    <a href="#infos" class="text-gray-600 hover:text-brand-green font-medium transition">Horaires & Contact</a>
                    <a href="#contact" class="bg-brand-green text-white px-6 py-2 rounded-full font-semibold hover:bg-green-600 transition shadow-lg">Réserver</a>
                </div>
                <!-- Mobile menu button -->
                <div class="md:hidden flex items-center">
                    <button id="mobile-menu-btn" class="text-gray-600 hover:text-brand-dark focus:outline-none">
                        <i class="fa-solid fa-bars text-2xl"></i>
                    </button>
                </div>
            </div>
        </div>
        <!-- Mobile Menu -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t">
            <a href="#accueil" class="block px-4 py-3 text-gray-600 hover:bg-gray-50 hover:text-brand-green">Accueil</a>
            <a href="#tarifs" class="block px-4 py-3 text-gray-600 hover:bg-gray-50 hover:text-brand-green">Tarifs & Services</a>
            <a href="#infos" class="block px-4 py-3 text-gray-600 hover:bg-gray-50 hover:text-brand-green">Horaires & Contact</a>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="accueil" class="hero-bg h-screen min-h-[600px] flex items-center justify-center mt-10">
        <div class="text-center px-4 max-w-4xl mx-auto">
            <h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
                Découvrez Knokke en <span class="text-brand-green">Toute Liberté</span>
            </h1>
            <p class="text-lg md:text-2xl text-gray-200 mb-10">
                Location de trottinettes électriques haut de gamme. Rapide, écologique et fun !
            </p>
            <div class="flex flex-col sm:flex-row gap-4 justify-center">
                <a href="#tarifs" class="bg-brand-green text-white px-8 py-4 rounded-full font-bold text-lg hover:bg-green-600 transition shadow-lg flex items-center justify-center gap-2">
                    <i class="fa-solid fa-scooter"></i> Voir nos tarifs
                </a>
                <a href="#infos" class="bg-white text-brand-dark px-8 py-4 rounded-full font-bold text-lg hover:bg-gray-100 transition shadow-lg flex items-center justify-center gap-2">
                    <i class="fa-solid fa-location-dot"></i> Nous trouver
                </a>
            </div>
        </div>
    </section>

    <!-- Welcome / About Section -->
    <section class="py-16 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <h2 class="text-3xl md:text-4xl font-bold text-brand-dark mb-6">Bienvenue chez IsmaTrott Knokke</h2>
            <p class="text-lg text-gray-600 max-w-3xl mx-auto leading-relaxed">
                Bonjour, je suis <span class="font-bold text-brand-green">Ismael</span>. Passionné par la mobilité douce et notre belle côte belge, j'ai créé IsmaTrott pour vous offrir la meilleure façon d'explorer Knokke-Heist et ses environs. Que vous souhaitiez faire du shopping sur la Lippenslaan ou découvrir la magnifique réserve naturelle du Zwin, nos trottinettes sont prêtes pour vous !
            </p>
        </div>
    </section>

    <!-- Pricing & Services -->
    <section id="tarifs" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold text-brand-dark mb-4">Nos Tarifs & Services</h2>
                <p class="text-gray-600 text-lg">Choisissez la formule qui correspond à vos envies.</p>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <!-- Card 1: 1 Heure -->
                <div class="bg-white rounded-2xl shadow-lg p-8 border-t-4 border-brand-green transform transition duration-300 hover:-translate-y-2">
                    <div class="text-brand-green text-4xl mb-4 text-center">
                        <i class="fa-regular fa-clock"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-center text-brand-dark mb-2">Location Courte</h3>
                    <p class="text-center text-gray-500 mb-6">Idéal pour un petit trajet</p>
                    <div class="text-center mb-6">
                        <span class="text-5xl font-bold text-brand-dark">15 €</span>
                        <span class="text-gray-500"> / 1 heure</span>
                    </div>
                    <ul class="text-gray-600 space-y-3 mb-8">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-green"></i> Trottinette chargée à 100%</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-green"></i> Casque inclus sur demande</li>
                    </ul>
                    <button onclick="openModal('Location 1 Heure')" class="w-full bg-brand-dark text-white py-3 rounded-xl font-semibold hover:bg-gray-700 transition">Choisir</button>
                </div>

                <!-- Card 2: 4 Heures -->
                <div class="bg-brand-dark rounded-2xl shadow-xl p-8 transform md:-translate-y-4 relative">
                    <div class="absolute top-0 right-0 bg-brand-green text-white text-xs font-bold px-3 py-1 rounded-bl-lg rounded-tr-xl uppercase tracking-wider">
                        Populaire
                    </div>
                    <div class="text-brand-green text-4xl mb-4 text-center">
                        <i class="fa-solid fa-battery-three-quarters"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-center text-white mb-2">Demi-Journée</h3>
                    <p class="text-center text-gray-400 mb-6">Parfait pour explorer la digue</p>
                    <div class="text-center mb-6">
                        <span class="text-5xl font-bold text-white">40 €</span>
                        <span class="text-gray-400"> / 4 heures</span>
                    </div>
                    <ul class="text-gray-300 space-y-3 mb-8">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-green"></i> Batterie longue durée</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-green"></i> Cadenas de sécurité fourni</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-brand-green"></i> Assistance en cas de panne</li>
                    </ul>
                    <button onclick="openModal('Location Demi-Journée')" class="w-full bg-brand-green text-white py-3 rounded-xl font-semibold hover:bg-green-600 transition">Choisir</button>
                </div>

                <!-- Card 3: Tour Zwin -->
                <div class="bg-white rounded-2xl shadow-lg p-8 border-t-4 border-blue-500 transform transition duration-300 hover:-translate-y-2">
                    <div class="text-blue-500 text-4xl mb-4 text-center">
                        <i class="fa-solid fa-map-location-dot"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-center text-brand-dark mb-2">Tour "Le Zwin"</h3>
                    <p class="text-center text-gray-500 mb-6">Aventure guidée en nature</p>
                    <div class="text-center mb-6">
                        <span class="text-5xl font-bold text-brand-dark">25 €</span>
                        <span class="text-gray-500"> / personne</span>
                    </div>
                    <ul class="text-gray-600 space-y-3 mb-8">
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-blue-500"></i> Guide local (Ismael)</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-blue-500"></i> Découverte de la réserve</li>
                        <li class="flex items-center gap-2"><i class="fa-solid fa-check text-blue-500"></i> Souvenirs garantis</li>
                    </ul>
                    <button onclick="openModal('Tour Guidé Le Zwin')" class="w-full bg-brand-dark text-white py-3 rounded-xl font-semibold hover:bg-gray-700 transition">Réserver le tour</button>
                </div>
            </div>
        </div>
    </section>

    <!-- Info & Contact Section -->
    <section id="infos" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="bg-gray-50 rounded-3xl overflow-hidden shadow-xl flex flex-col lg:flex-row">
                
                <!-- Left Details -->
                <div class="p-10 lg:w-1/2 flex flex-col justify-center">
                    <h2 class="text-3xl font-bold text-brand-dark mb-8">Nos Informations</h2>
                    
                    <div class="flex items-start gap-4 mb-8">
                        <div class="bg-brand-green/20 p-3 rounded-full text-brand-green">
                            <i class="fa-solid fa-location-dot text-xl w-6 text-center"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-gray-800 text-lg">Adresse</h4>
                            <p class="text-gray-600 mt-1">Lippenslaan 172 Bus 01<br>8300 — KNOKKE</p>
                        </div>
                    </div>

                    <div class="flex items-start gap-4 mb-8">
                        <div class="bg-brand-green/20 p-3 rounded-full text-brand-green">
                            <i class="fa-solid fa-clock text-xl w-6 text-center"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-gray-800 text-lg">Heures d'ouverture</h4>
                            <p class="text-gray-600 mt-1">
                                Lundi - Dimanche<br>
                                <span class="font-semibold text-brand-dark">10:00 – 18:00</span>
                            </p>
                        </div>
                    </div>

                    <div class="mt-4">
                        <p class="text-gray-600 mb-4">Une question ? Passez nous voir directement en boutique !</p>
                        <a href="mailto:contact@ismatrott.be" class="inline-block bg-brand-dark text-white px-6 py-3 rounded-xl font-medium hover:bg-gray-700 transition">
                            <i class="fa-regular fa-envelope mr-2"></i> Nous contacter
                        </a>
                    </div>
                </div>

                <!-- Right Visual/Map Area (Placeholder) -->
                <div class="lg:w-1/2 bg-gray-200 relative min-h-[300px] lg:min-h-full">
                    <!-- A decorative map placeholder -->
                    <img src="https://images.unsplash.com/photo-1524661135-423995f22d0b?ixlib=rb-4.0.3&auto=format&fit=crop&w=800&q=80" alt="Knokke City" class="absolute inset-0 w-full h-full object-cover opacity-80 mix-blend-multiply">
                    <div class="absolute inset-0 flex items-center justify-center pointer-events-none">
                        <div class="bg-white/90 p-4 rounded-xl shadow-lg text-center backdrop-blur-sm">
                            <i class="fa-solid fa-location-dot text-brand-green text-3xl mb-2"></i>
                            <p class="font-bold text-brand-dark">IsmaTrott Knokke</p>
                            <p class="text-sm text-gray-600">Lippenslaan 172</p>
                        </div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-brand-dark text-white py-12 border-t-4 border-brand-green mt-auto">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 flex flex-col md:flex-row justify-between items-center">
            <div class="mb-6 md:mb-0 text-center md:text-left">
                <div class="flex items-center gap-2 justify-center md:justify-start mb-2">
                    <i class="fa-solid fa-bolt text-brand-green text-2xl"></i>
                    <span class="font-bold text-xl tracking-tight">Isma<span class="text-brand-green">Trott</span></span>
                </div>
                <p class="text-gray-400 text-sm">Location de trottinettes électriques à Knokke.</p>
            </div>
            
            <div class="flex space-x-6 mb-6 md:mb-0">
                <a href="#" class="text-gray-400 hover:text-white transition"><i class="fa-brands fa-instagram text-2xl"></i></a>
                <a href="#" class="text-gray-400 hover:text-white transition"><i class="fa-brands fa-facebook text-2xl"></i></a>
                <a href="#" class="text-gray-400 hover:text-white transition"><i class="fa-brands fa-tiktok text-2xl"></i></a>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mt-8 pt-8 border-t border-gray-700 text-center text-sm text-gray-500">
            &copy; 2024 IsmaTrott Knokke. Tous droits réservés. Propulsé par Ismael.
        </div>
    </footer>

    <!-- Reservation Modal (Simple interaction) -->
    <div id="reservation-modal" class="fixed inset-0 bg-black/60 z-[100] hidden flex items-center justify-center px-4 backdrop-blur-sm">
        <div class="bg-white rounded-2xl shadow-2xl max-w-md w-full p-8 relative transform scale-95 opacity-0 transition-all duration-300" id="modal-content">
            <button onclick="closeModal()" class="absolute top-4 right-4 text-gray-400 hover:text-gray-800">
                <i class="fa-solid fa-xmark text-2xl"></i>
            </button>
            <h3 class="text-2xl font-bold text-brand-dark mb-2">Demande de réservation</h3>
            <p class="text-gray-600 mb-6">Vous avez sélectionné : <span id="modal-service" class="font-bold text-brand-green"></span></p>
            
            <form onsubmit="submitForm(event)" class="space-y-4">
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Votre Nom</label>
                    <input type="text" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-brand-green focus:border-transparent outline-none">
                </div>
                <div>
                    <label class="block text-sm font-medium text-gray-700 mb-1">Date souhaitée</label>
                    <input type="date" required class="w-full px-4 py-2 border border-gray-300 rounded-lg focus:ring-2 focus:ring-brand-green focus:border-transparent outline-none">
                </div>
                <button type="submit" class="w-full bg-brand-green text-white py-3 rounded-xl font-bold hover:bg-green-600 transition shadow-md mt-4">
                    Confirmer la demande
                </button>
            </form>
            <p class="text-xs text-center text-gray-400 mt-4">*Ceci est une démonstration du système de réservation.</p>
        </div>
    </div>

    <!-- Scripts -->
    <script>
        // Mobile Menu Toggle
        const btn = document.getElementById('mobile-menu-btn');
        const menu = document.getElementById('mobile-menu');

        btn.addEventListener('click', () => {
            menu.classList.toggle('hidden');
        });

        // Close mobile menu on link click
        menu.querySelectorAll('a').forEach(link => {
            link.addEventListener('click', () => {
                menu.classList.add('hidden');
            });
        });

        // Modal Logic
        const modal = document.getElementById('reservation-modal');
        const modalContent = document.getElementById('modal-content');
        const modalServiceText = document.getElementById('modal-service');

        function openModal(serviceName) {
            modalServiceText.textContent = serviceName;
            modal.classList.remove('hidden');
            // Small timeout for the transition to work
            setTimeout(() => {
                modalContent.classList.remove('scale-95', 'opacity-0');
                modalContent.classList.add('scale-100', 'opacity-100');
            }, 10);
        }

        function closeModal() {
            modalContent.classList.remove('scale-100', 'opacity-100');
            modalContent.classList.add('scale-95', 'opacity-0');
            setTimeout(() => {
                modal.classList.add('hidden');
            }, 300);
        }

        // Close modal when clicking outside
        modal.addEventListener('click', (e) => {
            if (e.target === modal) {
                closeModal();
            }
        });

        function submitForm(e) {
            e.preventDefault();
            alert("Merci ! Votre demande a été envoyée. Ismael vous recontactera très vite pour confirmer.");
            closeModal();
            e.target.reset();
        }
    </script>
</body>
</html>
