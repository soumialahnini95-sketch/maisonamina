<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Cutie Corner - Accessoires Féminins de Haute Qualité, Casablanca</title>
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css"> <!-- Icônes Font Awesome pour féminité -->
    <style>
        /* Styles généraux avec thème féminin et professionnel */
        body {
            font-family: 'Georgia', serif; /* Police élégante et féminine */
            line-height: 1.8;
            color: #4a4a4a;
            background-color: #fefefe;
        }

        /* Logo avec touche féminine */
        .logo {
            font-weight: bold;
            color: #e91e63; /* Rose profond pour féminité */
            font-size: 2rem;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }

        /* Section Hero avec gradient féminin */
        .hero {
            background: linear-gradient(135deg, #fce4ec 0%, #f8bbd9 100%); /* Dégradé rose doux */
            background-size: cover;
            background-position: center;
            min-height: 70vh;
            display: flex;
            align-items: center;
            position: relative;
        }
        .hero::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: rgba(255,255,255,0.1);
        }
        .hero .container {
            position: relative;
            z-index: 1;
        }

        /* Cartes de produits avec effets féminins */
        .card {
            border: none;
            border-radius: 15px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            overflow: hidden;
        }
        .card:hover {
            transform: translateY(-10px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.2);
        }
        .card-img-top {
            height: 200px;
            object-fit: cover;
        }

        /* Boutons avec style féminin */
        .btn-primary {
            background: linear-gradient(45deg, #e91e63, #f06292);
            border: none;
            border-radius: 25px;
            padding: 10px 20px;
            font-weight: bold;
            transition: all 0.3s ease;
        }
        .btn-primary:hover {
            background: linear-gradient(45deg, #c2185b, #e91e63);
            transform: scale(1.05);
        }

        /* Section À propos avec message féminin */
        #about {
            background: #fff;
            padding: 60px 0;
        }
        #about h3 {
            color: #e91e63;
            font-weight: bold;
        }

        /* Témoignages pour attractivité */
        #testimonials {
            background: #fce4ec;
            padding: 60px 0;
        }
        .testimonial {
            text-align: center;
            margin-bottom: 30px;
        }
        .testimonial img {
            width: 80px;
            height: 80px;
            border-radius: 50%;
            margin-bottom: 15px;
        }

        /* Newsletter */
        #newsletter {
            background: #e91e63;
            color: white;
            padding: 40px 0;
            text-align: center;
        }

        /* Footer professionnel */
        footer {
            background: #333;
            color: white;
            padding: 20px 0;
        }

        /* Animations subtiles */
        .fade-in {
            opacity: 0;
            animation: fadeIn 1s ease-in-out forwards;
        }
        @keyframes fadeIn {
            to { opacity: 1; }
        }

        /* Responsivité */
        @media (max-width: 768px) {
            .hero h2 {
                font-size: 2rem;
            }
            .nav {
                flex-direction: column;
            }
        }
    </style>
</head>
<body>
    <!-- Header avec navigation -->
    <header class="bg-white py-3 shadow-sm">
        <div class="container">
            <div class="row align-items-center">
                <div class="col-md-3">
                    <h1 class="logo"><i class="fas fa-heart"></i> Cutie Corner</h1> <!-- Icône cœur pour féminité -->
                </div>
                <div class="col-md-9">
                    <nav>
                        
                        <ul class="nav justify-content-end">
                            <li class="nav-item"><a class="nav-link" href="#home"><i class="fas fa-home"></i> Accueil</a></li>
                            <li class="nav-item"><a class="nav-link" href="#products"><i class="fas fa-gem"></i> Produits</a></li>
                            <li class="nav-item"><a class="nav-link" href="#about"><i class="fas fa-info-circle"></i> À propos</a></li>
                            <li class="nav-item"><a class="nav-link" href="#testimonials"><i class="fas fa-star"></i> Témoignages</a></li>
                            <li class="nav-item"><a class="nav-link" href="#contact"><i class="fas fa-envelope"></i> Contact</a></li>
                            <li class="nav-item"><a class="nav-link" href="#cart"><i class="fas fa-shopping-cart"></i> Panier</a></li>
                        </ul>::``

                    </nav>
                </div>
            </div>
        </div>
    </header>

    <!-- Section Hero (accueil) -->
    <section id="home" class="hero text-white text-center py-5 fade-in">
        <div class="container">
            <h2 class="display-4">Élevez Votre Style Féminin avec Cutie Corner</h2>
            <p class="lead">Bagues, colliers et boucles d'oreilles de haute qualité, conçus pour sublimer votre beauté. Expédiés depuis Casablanca, pour une élégance intemporelle et accessible.</p>
            <a href="#products" class="btn btn-light btn-lg"><i class="fas fa-arrow-down"></i> Découvrez nos produits</a>
        </div>
    </section>

    <!-- Section Produits -->
    <section id="products" class="py-5 bg-light">
        <div class="container">
            <h3 class="text-center mb-5" style="color: #e91e63;">Nos Accessoires Féminins</h3>
            <div class="row">
                <!-- Produit 1 : Bagues -->
                <div class="col-md-4 mb-4">
                    <div class="card h-100">
                        <img src="bague1.jpg" class="card-img-top" alt="Bague élégante" onerror="this.src='https://via.placeholder.com/300x200?text=Bague+Elegante'">
                        <div class="card-body">
                            <h5 class="card-title">Bague en Argent avec Pierre Précieuse</h5>
                            <p class="card-text">Design délicat et raffiné, parfait pour ajouter une touche de glamour à votre quotidien. Matériau hypoallergénique, durable et ajustable. Idéale pour les occasions spéciales ou le port quotidien, symbolisant l'élégance féminine.</p>
                            <p class="text-primary font-weight-bold">350 MAD</p>
                            <a href="#" class="btn btn-primary add-to-cart"><i class="fas fa-cart-plus"></i> Ajouter au panier</a>
                        </div>
                    </div>
                </div>
                <!-- Produit 2 : Colliers -->
                <div class="col-md-4 mb-4">
                    <div class="card h-100">
                        <img src="collier1.jpg" class="card-img-top" alt="Collier chic" onerror="this.src='https://via.placeholder.com/300x200?text=Collier+Chic'">
                        <div class="card-body">
                            <h5 class="card-title">Collier en Or Blanc avec Pendentif</h5>
                            <p class="card-text">Chaîne fine et pendentif scintillant pour un look sophistiqué. Inspiré par la beauté naturelle des femmes, ce collier met en valeur votre cou avec grâce. Longueur ajustable, facile à porter seul ou en layering.</p>
                            <p class="text-primary font-weight-bold">500 MAD</p>
                            <a href="#" class="btn btn-primary add-to-cart"><i class="fas fa-cart-plus"></i> Ajouter au panier</a>
                        </div>
                    </div>
                </div>
                <!-- Produit 3 : Boucles d'oreilles -->
                <div class="col-md-4 mb-4">
                    <div class="card h-100">
                        <img src="boucles1.jpg" class="card-img-top" alt="Boucles d'oreilles" onerror="this.src='https://via.placeholder.com/300x200?text=Boucles+Ooreilles'">
                        <div class="card-body">
                            <h5 class="card-title">Boucles d'Oreilles en Cristal Swarovski</h5>
                            <p class="card-text">Éclat cristallin pour illuminer votre visage. Design asymétrique moderne, confortable pour un port prolongé. Parfaites pour les soirées ou le bureau, ajoutant une note de féminité et de confiance à votre tenue.</p>
                            <p class="text-primary font-weight-bold">250 MAD</p>
                            <a href="#" class="btn btn-primary add-to-cart"><i class="fas fa-cart-plus"></i> Ajouter au panier</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Section À propos avec message féminin -->
    <section id="about" class="py-5">
        <div class="container">
            <h3 class="text-center mb-4">À propos de Cutie Corner : Célébrer la Féminité</h3>
            <div class="row">
                <div class="col-md-6">
                    <p>Basée à Casablanca, Cutie Corner est dédiée à offrir des bagues, colliers et boucles d'oreilles qui célèbrent la beauté et la force des femmes. Chaque pièce est sélectionnée avec soin pour sa qualité, son élégance et son accessibilité. Notre mission est d'aider les femmes à se sentir confiantes et stylées, en promouvant une mode inclusive et durable.</p>
                    <p><strong>Pourquoi nous choisir ?</strong> Pièces uniques, livraison rapide et un service personnalisé pour sublimer votre look.</p>
                </div>
                <div class="col-md-6">
                    <img src="about-image.jpg" class="img-fluid rounded" alt="Équipe Cutie Corner" onerror="this.src='https://via.placeholder.com/500x300?text=Equipe'">
                </div>
            </div>
        </div>
    </section>

    <!-- Section Témoignages pour attractivité -->
    <section id="testimonials" class="py-5">
        <div class="container">
            <h3 class="text-center mb-5" style="color: #e91e63;">Ce que disent nos clientes</h3>
            <div class="row">
                <div class="col-md-4 testimonial">
                    <img src="https://via.placeholder.com/80x80?text=Femme1" alt="Témoignage 1">
                    <p>"Ces bagues sont magnifiques et confortables. Elles me font sentir spéciale tous les jours !"</p>
                    <p><strong>- Amina, Casablanca</strong></p>
                </div>
                <div class="col-md-4 testimonial">
                    <img src="https://via.placeholder.com/80x80?text=Femme2" alt="Témoignage 2">
                    <p>"Le collier est parfait pour mes tenues. Qualité exceptionnelle et livraison rapide."</p>
                    <p><strong>- Fatima, Rabat</strong></p>
                </div>
                <div class="col-md-4 testimonial">
                    <img src="https://via.placeholder.com/80x80?text=Femme3" alt="Témoignage 3">
                    <p>"Les boucles d'oreilles ajoutent une touche d'élégance. Merci Cutie Corner !"</p>
                    <p><strong>- Leila, Marrakech</strong></p>
                </div>
            </div>
        </div>
    </section>

    <!-- Section Contact -->
    <section id="contact" class="py-5 bg-light">
        <div class="container">
            <h3 class="text-center mb-4" style="color: #e91e63;">Contactez-nous</h3>
            <div class="row">
                <div class="col-md-6">
                    <form id="contact-form">
                        <div class="form-group">
                            <label for="name"><i class="fas fa-user"></i> Nom</label>
                            <input type="text" class="form-control" id="name" required>
                        </div>
                        <div class="form-group">
                            <label for="email"><i class="fas fa-envelope"></i> Email</label>
                            <input type="email" class="form-control" id="email" required>
                        </div>
                        <div class="form-group">
                            <label for="message"><i class="fas fa-comment"></i> Message</label>
                            <textarea class="form-control" id="message" rows="4" required></textarea>
                        </div>
                        <button type="submit" class="btn btn-primary"><i class="fas fa-paper-plane"></i> Envoyer</button>
                    </form>
                </div>
                <div class="col-md-6">
                    <p><strong><i class="fas fa-map-marker-alt"></i> Adresse :</strong> Casablanca, Maroc</p>
                    <p><strong><i class="fas fa-envelope"></i> Email :</strong> info@cutiecorner.ma</p>
                    <p><strong><i class="fas fa-phone"></i> Téléphone :</strong> +212 6XX XXX XXX</p>
                    <p><strong><i class="fas fa-truck"></i> Livraison :</strong> Gratuite à Casablanca, frais réduits ailleurs. Commandez en ligne pour une élégance livrée à domicile.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Newsletter -->
    <section id="newsletter">
        <div class="container">
            <h4>Abonnez-vous à notre newsletter</h4>
            <p>Recevez des conseils de style, des offres exclusives et des inspirations pour vos looks féminins.</p>
            <form class="form-inline justify-content-center">
                <input type="email" class="form-control mr-2" placeholder="Votre email" required>
                <button type="submit" class="btn btn-light"><i class="fas fa-envelope"></i> S'abonner</button>
            </form>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-dark text-white py-3">
        <div class="container text-center">
            <p>&copy; 2025 Cutie Corner. Tous droits réservés. | <a href="#" class="text-white">Mentions légales</a> | <a href="#" class="text-white">Politique de confidentialité</a></p>
            <div class="social-links">
                <a href="#" class="text-white mx-2"><i class="fab fa-facebook"></i> Facebook</a>
                <a href="#" class="text-white mx-2"><i class="fab fa-instagram"></i> Instagram</a>
                <a href="#" class="text-white mx-2"><i class="fab fa-twitter"></i> Twitter</a>
            </div>
        </div>
    </footer>

    <!-- Scripts -->
    <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@4.5.2/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // Script pour le panier simple et animations
        document.addEventListener('DOMContentLoaded', function() {
            const addToCartButtons = document.querySelectorAll('.add-to-cart');
            addToCartButtons.forEach(button => {
                button.addEventListener('click', function(event) {
                    event.preventDefault();
                    alert('Produit ajouté au panier ! Continuez à célébrer votre féminité.');
                });
            });

            // Validation du formulaire de contact
            const contactForm = document.getElementById('contact-form');
            contactForm.addEventListener('submit', function(event) {
                event.preventDefault();
                alert('Message envoyé ! Merci de nous contacter.');
            });

            // Animation fade-in pour les sections
            const sections = document.querySelectorAll('section');
            const observer = new IntersectionObserver(entries => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.classList.add('fade-in');
                    }
                });
            });
            sections.forEach(section => observer.observe(section));
        });
    </script>
</body>
</html>
