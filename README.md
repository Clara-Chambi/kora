<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>EndoVitalité - Complément alimentaire pour femmes atteintes d'endométriose</title>
    <style>
        /* Couleurs vives et joyeuses dans l'esprit du dopamine decor */
        :root {
            --primary: #ff6b98;
            --secondary: #7e54ed;
            --accent: #ffc145;
            --background: #fff8fd;
            --text: #333333;
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        body {
            background-color: var(--background);
            color: var(--text);
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Style fun et féminin avec des formes ludiques */
        .header {
            background-color: var(--primary);
            padding: 20px 0;
            text-align: center;
            position: relative;
            overflow: hidden;
        }
        
        .header:before {
            content: "";
            position: absolute;
            top: -30px;
            left: -30px;
            width: 120px;
            height: 120px;
            border-radius: 50%;
            background-color: var(--accent);
            opacity: 0.6;
            z-index: 0;
        }
        
        .header:after {
            content: "";
            position: absolute;
            bottom: -50px;
            right: -50px;
            width: 180px;
            height: 180px;
            border-radius: 50%;
            background-color: var(--secondary);
            opacity: 0.4;
            z-index: 0;
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            color: white;
            position: relative;
            z-index: 1;
        }
        
        .logo span {
            color: var(--accent);
        }
        
        .hero {
            padding: 100px 0;
            text-align: center;
            position: relative;
        }
        
        .hero:before {
            content: "";
            position: absolute;
            top: 50%;
            left: 15%;
            width: 80px;
            height: 80px;
            background-color: var(--accent);
            border-radius: 50%;
            opacity: 0.15;
        }
        
        .hero:after {
            content: "";
            position: absolute;
            bottom: 20%;
            right: 10%;
            width: 150px;
            height: 150px;
            background-color: var(--secondary);
            border-radius: 20px;
            transform: rotate(25deg);
            opacity: 0.1;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 20px;
            color: var(--primary);
            position: relative;
            z-index: 1;
        }
        
        .hero p {
            font-size: 1.2rem;
            max-width: 800px;
            margin: 0 auto 30px;
            position: relative;
            z-index: 1;
        }
        
        .benefits {
            padding: 80px 0;
            background-color: white;
            position: relative;
            overflow: hidden;
        }
        
        .benefits-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 60px;
            color: var(--secondary);
        }
        
        .benefits-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 30px;
        }
        
        .benefit-card {
            flex: 0 0 calc(33.333% - 30px);
            min-width: 300px;
            background-color: var(--background);
            border-radius: 20px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
            transition: transform 0.3s ease;
            position: relative;
            z-index: 1;
        }
        
        .benefit-card:hover {
            transform: translateY(-10px);
        }
        
        .benefit-icon {
            width: 80px;
            height: 80px;
            background-color: var(--primary);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            margin: 0 auto 20px;
            font-size: 2rem;
            color: white;
        }
        
        .benefit-card h3 {
            margin-bottom: 15px;
            color: var(--secondary);
        }
        
        .about {
            padding: 100px 0;
            text-align: center;
        }
        
        .about h2 {
            font-size: 2.5rem;
            color: var(--primary);
            margin-bottom: 30px;
        }
        
        .about p {
            max-width: 800px;
            margin: 0 auto 20px;
            font-size: 1.1rem;
        }
        
        .cta-section {
            padding: 100px 0;
            text-align: center;
            background-color: var(--background);
            position: relative;
            overflow: hidden;
        }
        
        .cta-section:before {
            content: "";
            position: absolute;
            top: -60px;
            left: 10%;
            width: 180px;
            height: 180px;
            background-color: var(--primary);
            border-radius: 50%;
            opacity: 0.1;
        }
        
        .cta-section:after {
            content: "";
            position: absolute;
            bottom: -80px;
            right: 5%;
            width: 200px;
            height: 200px;
            background-color: var(--accent);
            border-radius: 30px;
            transform: rotate(-15deg);
            opacity: 0.15;
        }
        
        .cta-section h2 {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 30px;
            position: relative;
            z-index: 1;
        }
        
        .cta-section p {
            font-size: 1.2rem;
            max-width: 700px;
            margin: 0 auto 40px;
            position: relative;
            z-index: 1;
        }
        
        .cta-form {
            max-width: 500px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
        }
        
        .cta-form input {
            width: 100%;
            padding: 15px 20px;
            border: none;
            border-radius: 50px;
            font-size: 1rem;
            margin-bottom: 20px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.05);
        }
        
        .cta-form button {
            background-color: var(--primary);
            color: white;
            border: none;
            border-radius: 50px;
            padding: 15px 40px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(var(--primary-rgb), 0.3);
        }
        
        .cta-form button:hover {
            background-color: var(--secondary);
            transform: translateY(-3px);
        }
        
        .footer {
            background-color: var(--primary);
            color: white;
            text-align: center;
            padding: 30px 0;
            position: relative;
        }
        
        .footer p {
            margin: 10px 0;
            position: relative;
            z-index: 1;
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }
        
        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: color 0.3s ease;
        }
        
        .social-links a:hover {
            color: var(--accent);
        }
        
        /* Animations pour un style plus dynamique */
        @keyframes float {
            0% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
            100% { transform: translateY(0px); }
        }
        
        .float-animation {
            animation: float 4s ease-in-out infinite;
        }
        
        /* Design responsive */
        @media (max-width: 768px) {
            .hero h1 {
                font-size: 2.2rem;
            }
            
            .benefit-card {
                flex: 0 0 100%;
            }
        }

        /* Éléments de forme décoratifs */
        .shape {
            position: absolute;
            z-index: 0;
            opacity: 0.1;
        }
        
        .shape-1 {
            top: 20%;
            left: 5%;
            width: 100px;
            height: 100px;
            background-color: var(--accent);
            border-radius: 50%;
        }
        
        .shape-2 {
            top: 60%;
            right: 10%;
            width: 150px;
            height: 150px;
            background-color: var(--primary);
            border-radius: 30% 70% 70% 30% / 30% 30% 70% 70%;
        }
    </style>
    <!-- Font Awesome pour les icônes -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Police Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
</head>
<body>
    <!-- En-tête -->
    <header class="header">
        <div class="container">
            <div class="logo">Endo<span>Vitalité</span></div>
        </div>
    </header>

    <!-- Section héro -->
    <section class="hero">
        <div class="container">
            <h1 class="float-animation">Un soutien naturel pour les femmes atteintes d'endométriose</h1>
            <p>Notre complément alimentaire spécialement formulé pour apaiser les symptômes et améliorer votre bien-être au quotidien.</p>
            <div class="shape shape-1"></div>
            <div class="shape shape-2"></div>
        </div>
    </section>

    <!-- Section bénéfices -->
    <section class="benefits">
        <div class="container">
            <h2 class="benefits-title">Comment EndoVitalité peut vous aider</h2>
            <div class="benefits-container">
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-heart"></i>
                    </div>
                    <h3>Soulage les douleurs</h3>
                    <p>Des ingrédients naturels sélectionnés pour leurs propriétés anti-inflammatoires et apaisantes.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-bolt"></i>
                    </div>
                    <h3>Boost d'énergie</h3>
                    <p>Combattez la fatigue chronique souvent associée à l'endométriose avec notre formule énergisante.</p>
                </div>
                <div class="benefit-card">
                    <div class="benefit-icon">
                        <i class="fas fa-balance-scale"></i>
                    </div>
                    <h3>Équilibre hormonal</h3>
                    <p>Des nutriments essentiels qui contribuent à un meilleur équilibre hormonal et une régulation du cycle.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Section à propos -->
    <section class="about">
        <div class="container">
            <h2>Notre engagement</h2>
            <p>EndoVitalité est né d'une volonté de proposer une solution naturelle et complémentaire aux femmes touchées par l'endométriose. Nous avons travaillé avec des experts en nutrition et des spécialistes de l'endométriose pour créer un complément adapté à vos besoins spécifiques.</p>
            <p>Tous nos ingrédients sont rigoureusement sélectionnés, d'origine naturelle et notre formule est fabriquée en France, sans perturbateurs endocriniens.</p>
        </div>
    </section>

    <!-- Section CTA -->
    <section class="cta-section">
        <div class="container">
            <h2>Soyez prévenue du lancement !</h2>
            <p>EndoVitalité sera bientôt disponible. Laissez-nous votre email pour être parmi les premières informées et bénéficier d'une offre spéciale de lancement.</p>
            <form class="cta-form" id="newsletter-form">
                <input type="email" placeholder="Votre adresse email" required>
                <button type="submit">Je veux être alertée !</button>
            </form>
        </div>
    </section>

    <!-- Pied de page -->
    <footer class="footer">
        <div class="container">
            <p>© 2025 EndoVitalité - Tous droits réservés</p>
            <p>Les compléments alimentaires ne remplacent pas un traitement médical. Consultez votre médecin.</p>
            <div class="social-links">
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-facebook"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
            </div>
        </div>
    </footer>

    <script>
        // Script pour gérer le formulaire d'inscription à la newsletter
        document.getElementById('newsletter-form').addEventListener('submit', function(e) {
            e.preventDefault();
            const email = this.querySelector('input[type="email"]').value;
            
            // En production, vous remplaceriez ceci par votre propre logique pour sauvegarder l'email
            // Par exemple, en envoyant les données à une API ou en les stockant dans localStorage
            alert('Merci ! Votre email ' + email + ' a bien été enregistré. Nous vous tiendrons informée du lancement !');
            this.reset();
        });
    </script>
</body>
</html>
