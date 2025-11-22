<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Maison Amina - Boulangerie & Pâtisserie</title>
  <style>
    /* Reset */
    * {
      margin: 0; padding: 0; box-sizing: border-box;
    }
    body {
      font-family: 'Poppins', sans-serif;
      background: #f9f7f1;
      color: #333;
      line-height: 1.6;
      scroll-behavior: smooth;
    }
    a {
      text-decoration: none;
      color: inherit;
    }
    header {
      position: fixed;
      top: 0; left: 0; right: 0;
      background: #fff;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      z-index: 1000;
    }
    nav {
      max-width: 1200px;
      margin: 0 auto;
      display: flex;
      align-items: center;
      padding: 15px 20px;
      justify-content: space-between;
    }
    
    nav.logo-img{
      height: 60px;
      width: auto;
      flex-shrink: 0;
    }
    
    nav ul {
      list-style: none;
      display: flex;
      gap: 25px;
      flex: 1;
      justify-content: center;
    }
    nav ul li a {
      font-weight: 600;
      font-size: 1rem;
      color: #555;
      padding: 6px 10px;
      border-radius: 4px;
      transition: background-color 0.3s ease, color 0.3s ease;
    }
    nav ul li a:hover,
    nav ul li a.active {
      background-color: #d2691e;
      color: #fff;
    }

    /* Hero Section */
    .hero {
      margin-top: 65px; /* header height */
      position: relative;
      height: 80vh;
      background: url('https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=1470&q=80') center/cover no-repeat;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      text-align: center;
      padding: 0 20px;
    }
    .hero::after {
      content: "";
      position: absolute;
      inset: 0;
      background: rgba(139, 69, 19, 0.6);
      z-index: 0;
    }
    .hero-content {
      position: relative;
      z-index: 1;
      max-width: 700px;
    }
    .hero-content h1 {
      font-size: 3rem;
      font-family: 'Georgia', serif;
      margin-bottom: 15px;
      text-shadow: 2px 2px 6px rgba(0,0,0,0.8);
    }
    .hero-content p {
      font-size: 1.2rem;
      margin-bottom: 25px;
      text-shadow: 1px 1px 4px rgba(0,0,0,0.7);
    }
    .btn-primary {
      background-color: #d2691e;
      color: #fff;
      padding: 12px 30px;
      font-weight: 600;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      font-size: 1.1rem;
      transition: background-color 0.3s ease;
      box-shadow: 0 4px 10px rgba(210,105,30,0.4);
    }
    .btn-primary:hover {
      background-color: #a0521d;
      box-shadow: 0 6px 15px rgba(160,82,29,0.6);
    }

    /* Sections */
    section {
      max-width: 1100px;
      margin: 60px auto;
      padding: 0 20px;
    }
    section h2 {
      font-family: 'Georgia', serif;
      font-size: 2.5rem;
      color: #d2691e;
      margin-bottom: 20px;
      border-bottom: 3px solid #d2691e;
      padding-bottom: 8px;
      max-width: max-content;
    }
    section p, section ul {
      font-size: 1.1rem;
      color: #444;
      max-width: 800px;
    }
    section ul {
      list-style: disc inside;
      margin-top: 15px;
    }

    /* Galerie */
    .gallery {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap: 20px;
      margin-top: 25px;
    }
    .gallery img {
      width: 100%;
      height: 180px;
      object-fit: cover;
      border-radius: 12px;
      box-shadow: 0 6px 15px rgba(0,0,0,0.15);
      transition: transform 0.3s ease;
      cursor: pointer;
    }
    .gallery img:hover {
      transform: scale(1.05);
      box-shadow: 0 10px 25px rgba(0,0,0,0.3);
    &}

    /* Formulaire */
    form {
      max-width: 600px;
      background: #fff;
      padding: 30px 25px;
      border-radius: 12px;
      box-shadow: 0 6px 20px rgba(0,0,0,0.1);
    }
    form label {
      display: block;
      margin-bottom: 8px;
      font-weight: 600;
      color: #5a3e1b;
    }
    form input[type="text"],
    form input[type="email"],
    form textarea {
      width: 100%;
      padding: 12px 15px;
      margin-bottom: 20px;
      border: 2px solid #d2691e;
      border-radius: 8px;
      font-size: 1rem;
      font-family: inherit;
      resize: vertical;
      transition: border-color 0.3s ease;
    }
    form input[type="text"]:focus,
    form input[type="email"]:focus,
    form textarea:focus {
      border-color: #a0521d;
      outline: none;
    }
    form button {
      background-color: #d2691e;
      color: #fff;
      border: none;
      padding: 14px 30px;
      font-size: 1.1rem;
      font-weight: 700;
      border-radius: 30px;
      cursor: pointer;
      transition: background-color 0.3s ease;
      box-shadow: 0 6px 15px rgba(210,105,30,0.4);
    }
    form button:hover {
      background-color: #a0521d;
      box-shadow: 0 8px 20px rgba(160,82,29,0.6);
    }

    /* Newsletter */
    .newsletter {
      background: #d2691e;
      color: #fff;
      padding: 40px 20px;
      text-align: center;
      border-radius: 12px;
      max-width: 600px;
      margin: 0 auto 60px;
      box-shadow: 0 6px 20px rgba(210,105,30,0.4);
    }
    .newsletter h3 {
      font-size: 1.8rem;
      margin-bottom: 15px;
      font-family: 'Georgia', serif;
    }
    .newsletter form {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
    }
    .newsletter input[type="email"] {
      flex: 1 1 250px;
      padding: 12px 15px;
      border-radius: 30px;
      border: none;
      font-size: 1rem;
      font-family: inherit;
    }
    .newsletter button {
      flex: 0 0 auto;
      padding: 12px 30px;
      border-radius: 30px;
      border: none;
      background: #fff;
      color: #d2691e;
      font-weight: 700;
      cursor: pointer;
      transition: background-color 0.3s ease, color 0.3s ease;
    }
    .newsletter button:hover {
      background-color: #a0521d;
      color: #fff;
    }

    /* Footer */
    footer {
      background: #3e2f1c;
      color: #f0e6d2;
      text-align: center;
      padding: 20px 10px;
      font-size: 0.9rem;
      letter-spacing: 1px;
    }

    /* Responsive */
    @media (max-width: 768px) {
      .hero-content h1 {
        font-size: 2.2rem;
      }
      .hero-content p {
        font-size: 1rem;
      }
      nav ul {
        gap: 15px;
      }
    }
    @media (max-width: 480px) {
      nav {
        flex-direction: column;
        gap: 10px;
      }
      nav ul {
        flex-wrap: wrap;
        justify-content: center;
      }
      .newsletter form {
        flex-direction: column;
      }
      .newsletter input[type="email"],
      .newsletter button {
        width: 100%;
        flex: none;
      }
    }
  </style>
</head>
<body>

<header>
  <nav>
    <img src="images/logomaisonamina.png"height="auto" width="120" alt="logo maison amina" class="logo-img" />
    <ul>
      <li><a href="#hero" class="active">Accueil</a></li>
      <li><a href="#specialites">Spécialités</a></li>
      <li><a href="#galerie">Galerie</a></li>
      <li><a href="#contact">Contact</a></li>
      <li><a href="#newsletter">Newsletter</a></li>
    </ul>
  </nav>
</header>

<section class="hero" id="hero">
  <div class="hero-content">
    <h1>Maison Amina</h1>
    <p>La boulangerie & pâtisserie traditionnelle de Casablanca, où passion rime avec saveurs.</p>
    <button class="btn-primary" onclick="document.getElementById('contact').scrollIntoView({behavior:'smooth'})">Contactez-nous</button>
  </div>
</section>

<section id="specialites">
  <h2>Nos spécialités</h2>
  <p>Nous vous proposons une large gamme de produits frais et artisanaux, préparés avec soin :</p>
  <ul>
    <li>Pains traditionnels marocains cuits au four à bois</li>
    <li>Viennoiseries françaises feuilletées et gourmandes</li>
    <li>Pâtisseries marocaines parfumées à la fleur d'oranger</li>
    <li>Produits bio et ingrédients locaux sélectionnés</li>
  </ul>
</section>

<section id="galerie">
  <h2>Galerie de nos produits</h2>
  <div class="gallery">
    <img src="images/cookies.PNG" alt="cookies" />
    <img src="images/IMG_6776.JPG" alt="Viennoiseries" />
    <img src="images/foret.jpg" alt="foret" />
    <img src="images/praliné.jpg" alt="praliné" />
    <img src="images/IMG_6770.jpg">
    <img src="images/IMG_6776.JPG">
    <img src="images/IMG_6777.JPG">
  </div>
</section>

<section id="contact">
  <h2>Contactez-nous</h2>
  <form onsubmit="event.preventDefault(); alert('Merci pour votre message ! Nous vous répondrons bientôt.'); this.reset();">
    <label for="name">Nom complet</label>
    <input type="text" id="name" name="name" placeholder="Votre nom" required />

    <label for="email">Adresse e-mail</label>
    <input type="email" id="email" name="email" placeholder="Votre e-mail" required />

    <label for="message">Message</label>
    <textarea id="message" name="message" rows="5" placeholder="Votre message" required></textarea>

    <button type="submit">Envoyer</button>
  </form>
</section>

<section class="newsletter" id="newsletter">
  <h3>Abonnez-vous à notre newsletter</h3>
  <form onsubmit="event.preventDefault(); alert('Merci pour votre abonnement !'); this.reset();">
    <input type="email" placeholder="Votre adresse e-mail" required />
    <button type="submit">S'abonner</button>
  </form>
</section>

<footer>
  &copy; 2024 Maison Amina - Tous droits réservés - Casablanca
</footer>

</body>
</html>
