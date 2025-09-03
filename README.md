<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Remedios Naturales para Piel Seca, Grasa y Mixta | Tratamientos Caseros</title>
    <meta name="description" content="Descubre los mejores remedios naturales para el cuidado de la piel según tu tipo: seca, grasa, mixta. Soluciones caseras para acné, puntos negros, manchas, arrugas y más. Aprende a preparar mascarillas, tónicos e hidratantes naturales.">
    <meta name="keywords" content="remedios naturales piel, cuidado facial natural, mascarillas caseras, acné tratamiento natural, puntos negros eliminar, piel seca hidratación, piel grasa control sebo, poros dilatados, arrugas naturales, manchas faciales, belleza natural, skincare casero, rostro luminoso, antioxidantes naturales">
    <meta name="author" content="NaturalSkin">
    <meta name="robots" content="index, follow">
    <link rel="canonical" href="https://www.naturalskin.com/remedios-naturales">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        :root {
            --primary: #5d8a82;
            --secondary: #a7c4b5;
            --accent: #f6ae84;
            --light: #f9f6f0;
            --dark: #3a5a53;
        }
        
        body {
            background-color: #f9f9f9;
            color: #333;
            line-height: 1.6;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
            padding: 20px 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .header-content {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 28px;
            font-weight: 700;
            display: flex;
            align-items: center;
        }
        
        .logo i {
            margin-right: 10px;
            color: var(--accent);
        }
        
        nav ul {
            display: flex;
            list-style: none;
            align-items: center;
        }
        
        nav ul li {
            margin-left: 25px;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
            padding: 8px 15px;
            border-radius: 20px;
        }
        
        nav ul li a:hover, nav ul li a.active {
            background-color: rgba(255, 255, 255, 0.2);
            color: var(--accent);
        }
        
        /* Search Box */
        .search-container {
            position: relative;
            margin-left: 20px;
        }
        
        .search-box {
            padding: 10px 15px;
            padding-right: 40px;
            border: none;
            border-radius: 25px;
            width: 250px;
            font-size: 14px;
            outline: none;
        }
        
        .search-btn {
            position: absolute;
            right: 10px;
            top: 50%;
            transform: translateY(-50%);
            background: none;
            border: none;
            color: var(--dark);
            cursor: pointer;
        }
        
        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(93, 138, 130, 0.8), rgba(58, 90, 83, 0.9)), url('https://images.unsplash.com/photo-1596462502278-27bfdc403348?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
            color: white;
            padding: 100px 0;
            text-align: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 48px;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero p {
            font-size: 20px;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: #333;
            padding: 14px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            transition: all 0.3s;
        }
        
        .btn:hover {
            background-color: #f8c4a2;
            transform: translateY(-3px);
            box-shadow: 0 10px 20px rgba(0, 0, 0, 0.1);
        }
        
        /* Skin Types */
        .skin-types {
            padding: 80px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 50px;
            color: var(--primary);
            font-size: 36px;
        }
        
        .types-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .type-card {
            background-color: var(--light);
            border-radius: 10px;
            padding: 30px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
            text-decoration: none;
            color: inherit;
            display: block;
            cursor: pointer;
        }
        
        .type-card:hover {
            transform: translateY(-10px);
            text-decoration: none;
            color: inherit;
        }
        
        .type-card i {
            font-size: 50px;
            margin-bottom: 20px;
        }
        
        .dry-skin-icon {
            color: #8d6e63;
        }
        
        .oily-skin-icon {
            color: #78909c;
        }
        
        .mixed-skin-icon {
            color: #81c784;
        }
        
        .type-card h3 {
            margin-bottom: 15px;
            color: var(--dark);
        }
        
        /* Remedies Pages */
        .remedies-page {
            display: none;
            padding: 60px 0;
            background-color: #f1f5f9;
            min-height: calc(100vh - 80px);
        }
        
        .remedies-page.active {
            display: block;
        }
        
        .back-btn {
            display: inline-flex;
            align-items: center;
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
            margin-bottom: 30px;
            padding: 10px 20px;
            border-radius: 50px;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
            transition: all 0.3s;
        }
        
        .back-btn:hover {
            background-color: var(--primary);
            color: white;
            text-decoration: none;
        }
        
        .back-btn i {
            margin-right: 8px;
        }
        
        .problems-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 30px;
            margin-bottom: 50px;
        }
        
        .problem-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .problem-card:hover {
            transform: translateY(-5px);
        }
        
        .problem-header {
            padding: 20px;
            text-align: center;
            color: white;
        }
        
        .dry-skin-header {
            background: linear-gradient(135deg, #8d6e63 0%, #6d4c41 100%);
        }
        
        .oily-skin-header {
            background: linear-gradient(135deg, #78909c 0%, #546e7a 100%);
        }
        
        .mixed-skin-header {
            background: linear-gradient(135deg, #81c784 0%, #66bb6a 100%);
        }
        
        .problem-content {
            padding: 25px;
        }
        
        .problem-content h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        .problem-content ul {
            padding-left: 20px;
            margin-bottom: 20px;
        }
        
        .problem-content li {
            margin-bottom: 10px;
        }
        
        .problem-content p {
            margin-bottom: 15px;
        }
        
        .benefit-tag {
            display: inline-block;
            background-color: var(--secondary);
            color: white;
            padding: 5px 10px;
            border-radius: 20px;
            font-size: 12px;
            margin-top: 10px;
            margin-right: 5px;
        }
        
        /* Category Filter */
        .category-filter {
            display: flex;
            justify-content: center;
            margin-bottom: 40px;
            flex-wrap: wrap;
            gap: 10px;
        }
        
        .filter-btn {
            padding: 10px 20px;
            background-color: white;
            border: 2px solid var(--primary);
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s;
            font-weight: 500;
        }
        
        .filter-btn:hover, .filter-btn.active {
            background-color: var(--primary);
            color: white;
        }
        
        /* Search Results */
        .search-results {
            display: none;
            background-color: white;
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 30px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
        }
        
        .search-results h3 {
            color: var(--primary);
            margin-bottom: 15px;
        }
        
        /* Newsletter */
        .newsletter {
            background: linear-gradient(135deg, var(--primary) 0%, var(--dark) 100%);
            color: white;
            padding: 80px 0;
            text-align: center;
        }
        
        .newsletter h2 {
            margin-bottom: 20px;
        }
        
        .newsletter p {
            max-width: 600px;
            margin: 0 auto 30px;
        }
        
        .newsletter-form {
            display: flex;
            max-width: 500px;
            margin: 0 auto;
        }
        
        .newsletter-form input {
            flex: 1;
            padding: 15px;
            border: none;
            border-radius: 50px 0 0 50px;
            outline: none;
        }
        
        .newsletter-form button {
            background-color: var(--accent);
            color: #333;
            border: none;
            padding: 0 25px;
            border-radius: 0 50px 50px 0;
            font-weight: 600;
            cursor: pointer;
        }
        
        /* Footer */
        footer {
            background-color: #1a1a2e;
            color: white;
            padding: 60px 0 30px;
        }
        
        .footer-content {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 40px;
            margin-bottom: 40px;
        }
        
        .footer-column h3 {
            margin-bottom: 20px;
            font-size: 20px;
            color: var(--accent);
        }
        
        .footer-column ul {
            list-style: none;
        }
        
        .footer-column ul li {
            margin-bottom: 10px;
        }
        
        .footer-column ul li a {
            color: #ccc;
            text-decoration: none;
            transition: color 0.3s;
        }
        
        .footer-column ul li a:hover {
            color: var(--accent);
        }
        
        .social-icons {
            display: flex;
            gap: 15px;
        }
        
        .social-icons a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 40px;
            height: 40px;
            background-color: #333;
            border-radius: 50%;
            color: white;
            text-decoration: none;
            transition: all 0.3s;
        }
        
        .social-icons a:hover {
            background-color: var(--accent);
            color: #333;
            transform: translateY(-3px);
        }
        
        .copyright {
            text-align: center;
            padding-top: 30px;
            border-top: 1px solid #333;
            color: #ccc;
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 968px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 20px;
                justify-content: center;
                flex-wrap: wrap;
            }
            
            nav ul li {
                margin: 10px;
            }
            
            .search-container {
                margin: 15px 0 0 0;
                width: 100%;
            }
            
            .search-box {
                width: 100%;
                max-width: 300px;
            }
            
            .hero h1 {
                font-size: 36px;
            }
            
            .types-grid {
                grid-template-columns: 1fr;
            }
            
            .problems-grid {
                grid-template-columns: 1fr;
            }
            
            .newsletter-form {
                flex-direction: column;
            }
            
            .newsletter-form input {
                border-radius: 50px;
                margin-bottom: 10px;
            }
            
            .newsletter-form button {
                border-radius: 50px;
                padding: 15px;
            }
            
            .category-filter {
                flex-direction: column;
                align-items: center;
            }
            
            .filter-btn {
                width: 200px;
                text-align: center;
            }
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <div class="container">
            <div class="header-content">
                <div class="logo">
                    <i class="fas fa-spa"></i>
                    <span>NaturalSkin</span>
                </div>
                <nav>
                    <ul>
                        <li><a href="#" class="active" id="home-link">Inicio</a></li>
                        <li><a href="#" id="dry-skin-link">Piel Seca</a></li>
                        <li><a href="#" id="oily-skin-link">Piel Grasa</a></li>
                        <li><a href="#" id="mixed-skin-link">Piel Mixta</a></li>
                        <li>
                            <div class="search-container">
                                <input type="text" class="search-box" id="search-input" placeholder="Buscar remedios...">
                                <button class="search-btn" id="search-button">
                                    <i class="fas fa-search"></i>
                                </button>
                            </div>
                        </li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Home Page -->
    <section id="home-page">
        <div class="hero">
            <div class="container">
                <div class="hero-content">
                    <h1>Remedios Naturales para el Cuidado de tu Piel</h1>
                    <p>Descubre los mejores tratamientos naturales según tu tipo de piel. Soluciones efectivas para acné, puntos negros, manchas y más.</p>
                    <a href="#" class="btn">Explorar Tratamientos</a>
                </div>
            </div>
        </div>

        <div class="skin-types">
            <div class="container">
                <h2 class="section-title">Selecciona tu Tipo de Piel</h2>
                <div class="types-grid">
                    <div class="type-card" id="dry-skin-card">
                        <i class="fas fa-hand-holding-water dry-skin-icon"></i>
                        <h3>Piel Seca</h3>
                        <p>Remedios para hidratar, nutrir y rejuvenecer la piel seca. Soluciones para descamación, irritación y sensibilidad.</p>
                    </div>
                    <div class="type-card" id="oily-skin-card">
                        <i class="fas fa-tint oily-skin-icon"></i>
                        <h3>Piel Grasa</h3>
                        <p>Tratamientos para regular el sebo, minimizar poros y combatir el acné. Soluciones para brillos y puntos negros.</p>
                    </div>
                    <div class="type-card" id="mixed-skin-card">
                        <i class="fas fa-adjust mixed-skin-icon"></i>
                        <h3>Piel Mixta</h3>
                        <p>Balancea las zonas grasas y secas de tu rostro con estos remedios naturales. Equilibrio perfecto para tu piel.</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Newsletter -->
        <div class="newsletter">
            <div class="container">
                <h2>Suscríbete a Nuestro Newsletter</h2>
                <p>Recibe semanalmente recetas naturales, consejos de cuidado de la piel y promociones exclusivas.</p>
                <form class="newsletter-form">
                    <input type="email" placeholder="Tu correo electrónico" required>
                    <button type="submit">Suscribirme</button>
                </form>
            </div>
        </div>

        <!-- Footer -->
        <footer>
            <div class="container">
                <div class="footer-content">
                    <div class="footer-column">
                        <h3>NaturalSkin</h3>
                        <p>Tu fuente confiable de remedios naturales para el cuidado de la piel. Soluciones efectivas para cada tipo de piel.</p>
                        <div class="social-icons">
                            <a href="#"><i class="fab fa-facebook-f"></i></a>
                            <a href="#"><i class="fab fa-instagram"></i></a>
                            <a href="#"><i class="fab fa-twitter"></i></a>
                            <a href="#"><i class="fab fa-youtube"></i></a>
                        </div>
                    </div>
                    <div class="footer-column">
                        <h3>Enlaces Rápidos</h3>
                        <ul>
                            <li><a href="#" class="footer-link" data-page="home">Inicio</a></li>
                            <li><a href="#" class="footer-link" data-page="dry-skin">Piel Seca</a></li>
                            <li><a href="#" class="footer-link" data-page="oily-skin">Piel Grasa</a></li>
                            <li><a href="#" class="footer-link" data-page="mixed-skin">Piel Mixta</a></li>
                        </ul>
                    </div>
                    <div class="footer-column">
                        <h3>Recursos Populares</h3>
                        <ul>
                            <li><a href="#">Remedios para el acné</a></li>
                            <li><a href="#">Mascarillas naturales</a></li>
                            <li><a href="#">Aceites esenciales</a></li>
                            <li><a href="#">Rutina de cuidado facial</a></li>
                            <li><a href="#">Alimentos para una piel sana</a></li>
                        </ul>
                    </div>
                </div>
                <div class="copyright">
                    <p>&copy; 2023 NaturalSkin - Todos los derechos reservados</p>
                </div>
            </div>
        </footer>
    </section>

    <!-- Dry Skin Page -->
    <section id="dry-skin-page" class="remedies-page">
        <div class="container">
            <a href="#" class="back-btn" id="dry-skin-back"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Seca</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel seca necesita hidratación intensa y nutrición profunda. Descubre estos remedios naturales para restaurar la humedad natural de tu piel y lograr un aspecto radiante.
            </p>
            
            <div class="search-results" id="dry-skin-search-results">
                <h3>Resultados de búsqueda para: <span id="dry-search-query"></span></h3>
                <div id="dry-search-results-container"></div>
            </div>
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
                <button class="filter-btn" data-category="acne">Acné</button>
                <button class="filter-btn" data-category="arrugas">Arrugas</button>
                <button class="filter-btn" data-category="manchas">Manchas</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (3) -->
                <div class="problem-card" data-category="hidratantes" data-tags="piel seca hidratación profunda aceite coco vitamina e">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratación Intensa</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Coco y Vitamina E</h3>
                        <ul>
                            <li>2 cucharadas de aceite de coco</li>
                            <li>1 cápsula de vitamina E</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro con suaves masajes circulares antes de dormir. No enjuagues.</p>
                        <span class="benefit-tag">Regenerador</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel seca suero aguacate jojoba nutrición">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratación Profunda</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Serum de Aguacate y Jojoba</h3>
                        <ul>
                            <li>1 cucharada de aceite de aguacate</li>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>5 gotas de aceite esencial de manzanilla</li>
                        </ul>
                        <p>Mezcla los aceites en un frasco de vidrio. Aplica 2-3 gotas en el rostro después de la limpieza, antes de la crema hidratante.</p>
                        <span class="benefit-tag">Nutritivo</span>
                        <span class="benefit-tag">Regenerador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel seca bálsamo karité almendras reparación nocturna">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratación Nocturna</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Bálsamo Nocturno de Karité</h3>
                        <ul>
                            <li>1 cucharada de manteca de karité</li>
                            <li>1 cucharadita de aceite de almendras</li>
                            <li>3 gotas de aceite esencial de incienso</li>
                        </ul>
                        <p>Derrite la manteca de karité al baño maría, añade los aceites. Aplica una capa fina antes de dormir.</p>
                        <span class="benefit-tag">Reparador</span>
                        <span class="benefit-tag">Nutritivo</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (3) -->
                <div class="problem-card" data-category="mascarillas" data-tags="piel seca mascarilla aguacate miel hidratación">
                    <div class="problem-header dry-skin-header">
                        <h3>Nutrición Intensa</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Aguacate y Miel</h3>
                        <ul>
                            <li>1/2 aguacate maduro</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharada de aceite de oliva</li>
                        </ul>
                        <p>Machaca el aguacate y mezcla con miel y aceite. Aplica sobre el rostro durante 20 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Hidratante profunda</span>
                        <span class="benefit-tag">Nutritiva</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel seca mascarilla plátano miel calmante">
                    <div class="problem-header dry-skin-header">
                        <h3>Calmante y Nutritiva</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Plátano y Miel</h3>
                        <ul>
                            <li>1 plátano maduro</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de aceite de almendras</li>
                        </ul>
                        <p>Machaca el plátano hasta hacer puré, añade miel y aceite. Aplica durante 15-20 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Nutritiva</span>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel seca mascarilla yogur miel revitalizante">
                    <div class="problem-header dry-skin-header">
                        <h3>Revitalizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Yogur y Miel</h3>
                        <ul>
                            <li>2 cucharadas de yogur natural</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de aceite de coco</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro durante 15 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Revitalizante</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (3) -->
                <div class="problem-card" data-category="exfoliantes" data-tags="piel seca exfoliante avena miel suavizante">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliación Suave</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Avena y Miel</h3>
                        <ul>
                            <li>3 cucharadas de avena molida</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharada de yogurt natural</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Masajea suavemente durante 3 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Suavizante</span>
                        <span class="benefit-tag">Gentil</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel seca exfoliante azúcar miel nutritivo">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliación Nutritiva</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Azúcar Moreno y Miel</h3>
                        <ul>
                            <li>2 cucharadas de azúcar moreno</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharada de aceite de oliva</li>
                        </ul>
                        <p>Mezcla los ingredientes. Aplica con movimientos circulares suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Nutritivo</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel seca exfoliante café coco energizante">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliación de Café</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Café y Aceite de Coco</h3>
                        <ul>
                            <li>2 cucharadas de café molido</li>
                            <li>1 cucharada de aceite de coco</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con suaves masajes circulares. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Energizante</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (3) -->
                <div class="problem-card" data-category="tonicos" data-tags="piel seca tónico rosas hidratante calmante">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratante y Calmante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Rosas Hidratante</h3>
                        <ul>
                            <li>1 puñado de pétalos de rosa</li>
                            <li>1 taza de agua mineral</li>
                            <li>2 cucharadas de agua de hamamelis</li>
                        </ul>
                        <p>Hierve los pétalos de rosa en el agua durante 5 minutos. Deja enfriar, cuela y añade el hamamelis. Aplica con un algodón.</p>
                        <span class="benefit-tag">Hidratante</span>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel seca tónico manzanilla lavanda calmante">
                    <div class="problem-header dry-skin-header">
                        <h3>Calmante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Manzanilla y Lavanda</h3>
                        <ul>
                            <li>2 bolsas de té de manzanilla</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Prepara una infusión con la manzanilla. Cuando esté fría, añade el aceite de lavanda. Aplica con un algodón.</p>
                        <span class="benefit-tag">Calmante</span>
                        <span class="benefit-tag">Antiinflamatorio</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel seca tónico pepino menta revitalizante">
                    <div class="problem-header dry-skin-header">
                        <h3>Revitalizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Pepino y Menta</h3>
                        <ul>
                            <li>1/2 pepino mediano</li>
                            <li>1 cucharada de hojas de menta fresca</li>
                            <li>1 taza de agua de rosas</li>
                        </ul>
                        <p>Licúa el pepino con la menta y el agua de rosas. Cuela y guarda en refrigeración. Aplica por las mañanas.</p>
                        <span class="benefit-tag">Revitalizante</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <!-- ACNÉ (3) -->
                <div class="problem-card" data-category="acne" data-tags="piel seca acné tratamiento árbol té antiinflamatorio">
                    <div class="problem-header dry-skin-header">
                        <h3>Acné Suave</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento Localizado de Árbol de Té</h3>
                        <ul>
                            <li>5 gotas de aceite de árbol de té</li>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>Algodón o hisopo</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica directamente sobre los granos con un hisopo. No enjuagues.</p>
                        <span class="benefit-tag">Antibacterial</span>
                        <span class="benefit-tag">Antiinflamatorio</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="acne" data-tags="piel seca acné mascarilla miel canela antibacterial">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla para Acné</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Miel y Canela</h3>
                        <ul>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharadita de canela en polvo</li>
                            <li>1 cucharadita de aceite de coco</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre las áreas con acné. Deja actuar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Antibacterial</span>
                        <span class="benefit-tag">Antiinflamatorio</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="acne" data-tags="piel seca acné tónico hamamelis lavanda">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico para Acné</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Hamamelis y Lavanda</h3>
                        <ul>
                            <li>1/2 taza de hamamelis</li>
                            <li>10 gotas de aceite esencial de lavanda</li>
                            <li>2 cucharadas de agua de rosas</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con un algodón en las zonas afectadas dos veces al día.</p>
                        <span class="benefit-tag">Astringente suave</span>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <!-- ARRUGAS (3) -->
                <div class="problem-card" data-category="arrugas" data-tags="piel seca arrugas suero rosa mosqueta antioxidante">
                    <div class="problem-header dry-skin-header">
                        <h3>Antiarrugas</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Rosa Mosqueta</h3>
                        <ul>
                            <li>2 cucharadas de aceite de rosa mosqueta</li>
                            <li>5 gotas de aceite esencial de neroli</li>
                            <li>3 gotas de aceite esencial de incienso</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en rostro y cuello mañana y noche.</p>
                        <span class="benefit-tag">Regenerador</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="arrugas" data-tags="piel seca arrugas mascarilla aguacate plátano">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla Antiaging</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Aguacate y Plátano</h3>
                        <ul>
                            <li>1/4 de aguacate maduro</li>
                            <li>1/2 plátano maduro</li>
                            <li>1 cucharada de miel</li>
                        </ul>
                        <p>Machaca el aguacate y el plátano, añade miel. Aplica durante 20 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Nutritiva</span>
                        <span class="benefit-tag">Antienvejecimiento</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="arrugas" data-tags="piel seca arrugas contorno ojos manzanilla">
                    <div class="problem-header dry-skin-header">
                        <h3>Contorno de Ojos</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento para Contorno de Ojos</h3>
                        <ul>
                            <li>1 cucharada de aceite de almendras</li>
                            <li>2 gotas de aceite esencial de manzanilla</li>
                            <li>1 gota de aceite esencial de limón</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica una cantidad mínima con suaves toques alrededor de los ojos antes de dormir.</p>
                        <span class="benefit-tag">Antiojeras</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <!-- MANCHAS (3) -->
                <div class="problem-card" data-category="manchas" data-tags="piel seca manchas tratamiento limón miel">
                    <div class="problem-header dry-skin-header">
                        <h3>Manchas y Hiperpigmentación</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento de Limón y Miel</h3>
                        <ul>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 cucharada de miel</li>
                            <li>Algodón</li>
                        </ul>
                        <p>Mezcla el limón con miel. Aplica sobre las manchas con un algodón. Deja actuar 10 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Despigmentante</span>
                        <span class="benefit-tag">Suave</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="manchas" data-tags="piel seca manchas mascarilla cúrcuma yogur">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla Uniformizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Cúrcuma y Yogur</h3>
                        <ul>
                            <li>1 cucharadita de cúrcuma en polvo</li>
                            <li>2 cucharadas de yogur natural</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro evitando contorno de ojos. Deja 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Uniformizante</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="manchas" data-tags="piel seca manchas suero vitamina e limón">
                    <div class="problem-header dry-skin-header">
                        <h3>Suero para Manchas</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Vitamina E y Limón</h3>
                        <ul>
                            <li>2 cápsulas de vitamina E</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 cucharada de aceite de rosa mosqueta</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre las manchas antes de dormir. No enjuagues.</p>
                        <span class="benefit-tag">Despigmentante</span>
                        <span class="benefit-tag">Regenerador</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Oily Skin Page -->
    <section id="oily-skin-page" class="remedies-page">
        <div class="container">
            <a href="#" class="back-btn" id="oily-skin-back"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Grasa</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel grasa requiere regulación del sebo, limpieza profunda y minimización de poros. Estos tratamientos naturales te ayudarán a controlar el brillo y prevenir imperfecciones.
            </p>
            
            <div class="search-results" id="oily-skin-search-results">
                <h3>Resultados de búsqueda para: <span id="oily-search-query"></span></h3>
                <div id="oily-search-results-container"></div>
            </div>
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
                <button class="filter-btn" data-category="acne">Acné</button>
                <button class="filter-btn" data-category="poros">Poros Dilatados</button>
                <button class="filter-btn" data-category="brillo">Control de Brillo</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (3) -->
                <div class="problem-card" data-category="hidratantes" data-tags="piel grasa hidratante aloe vera árbol té matificante">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratación Ligera</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel de Aloe Vera</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera puro</li>
                            <li>5 gotas de aceite esencial de árbol de té</li>
                            <li>1 cucharadita de agua de hamamelis</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica una capa fina como hidratante diario. No enjuagues.</p>
                        <span class="benefit-tag">Matificante</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel grasa suero jojoba lavanda balanceador">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratación Balanceada</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Jojoba y Lavanda</h3>
                        <ul>
                            <li>2 cucharadas de aceite de jojoba</li>
                            <li>5 gotas de aceite essential de lavanda</li>
                            <li>3 gotas de aceite esencial de limón</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en el rostro después de la limpieza.</p>
                        <span class="benefit-tag">Balanceador</span>
                        <span class="benefit-tag">Regulador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel grasa hidratante té verde aloe vera sin aceites">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratación sin Aceites</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Hidratante de Té Verde</h3>
                        <ul>
                            <li>1/4 taza de té verde fuerte frío</li>
                            <li>1 cucharada de gel de aloe vera</li>
                            <li>1 cucharadita de glicerina vegetal</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro limpio. No enjuagues.</p>
                        <span class="benefit-tag">Libre de aceites</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (3) -->
                <div class="problem-card" data-category="mascarillas" data-tags="piel grasa mascarilla arcilla verde té verde purificante">
                    <div class="problem-header oily-skin-header">
                        <h3>Purificante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Arcilla Verde y Té Verde</h3>
                        <ul>
                            <li>2 cucharadas de arcilla verde</li>
                            <li>2 cucharadas de té verde frío</li>
                            <li>3 gotas de aceite de árbol de té</li>
                        </ul>
                        <p>Mezcla la arcilla con el té verde hasta formar una pasta. Añade el aceite de árbol de té. Aplica y deja secar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Matificante</span>
                        <span class="benefit-tag">Purificante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel grasa mascarilla yogur cúrcuma antibacterial">
                    <div class="problem-header oily-skin-header">
                        <h3>Antibacterial</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Yogur y Cúrcuma</h3>
                        <ul>
                            <li>2 cucharadas de yogur natural</li>
                            <li>1/2 cucharadita de cúrcuma</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica evitando el contorno de ojos. Deja actuar 15 minutos y enjuaga.</p>
                        <span class="benefit-tag">Antiséptica</span>
                        <span class="benefit-tag">Antiinflamatoria</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel grasa mascarilla carbón activado arcilla bentonita desintoxicante">
                    <div class="problem-header oily-skin-header">
                        <h3>Limpieza Profunda</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Carbón Activado</h3>
                        <ul>
                            <li>1 cápsula de carbón activado</li>
                            <li>1 cucharada de arcilla bentonita</li>
                            <li>2 cucharadas de agua de rosas</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro y deja secar 10-15 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Desintoxicante</span>
                        <span class="benefit-tag">Limpieza profunda</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (3) -->
                <div class="problem-card" data-category="exfoliantes" data-tags="piel grasa exfoliante carbón activado miel puntos negros">
                    <div class="problem-header oily-skin-header">
                        <h3>Limpieza de Poros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Carbón Activado y Miel</h3>
                        <ul>
                            <li>1 cápsula de carbón activado</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de azúcar moreno</li>
                        </ul>
                        <p>Mezcla el carbón con la miel y el azúcar. Aplica con suaves masajes circulares en la zona T. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Limpieza profunda</span>
                        <span class="benefit-tag">Puntos negros</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel grasa exfoliante avena miel limón suavizante">
                    <div class="problem-header oily-skin-header">
                        <h3>Suavizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Avena y Miel</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes suaves. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Suavizante</span>
                        <span class="benefit-tag">Equilibrante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel grasa exfoliante café jojoba revitalizante">
                    <div class="problem-header oily-skin-header">
                        <h3>Revitalizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Café</h3>
                        <ul>
                            <li>2 cucharadas de café molido usado</li>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>1 cucharadita de azúcar moreno</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes circulares suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Revitalizante</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (3) -->
                <div class="problem-card" data-category="tonicos" data-tags="piel grasa tónico agua rosas limón poros">
                    <div class="problem-header oily-skin-header">
                        <h3>Minimizador de Poros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Agua de Rosas y Limón</h3>
                        <ul>
                            <li>1/2 taza de agua de rosas</li>
                            <li>2 cucharadas de hamamelis</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Combina todos los ingredientes en una botella con spray. Aplica después de lavar tu rostro.</p>
                        <span class="benefit-tag">Minimiza poros</span>
                        <span class="benefit-tag">Astringente</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel grasa tónico aloe vera agua rosas refrescante">
                    <div class="problem-header oily-skin-header">
                        <h3>Refrescante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Aloe Vera</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>2 cucharadas de agua de rosas</li>
                            <li>1 cucharadita de hamamelis</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica con un algodón.</p>
                        <span class="benefit-tag">Refrescante</span>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel grasa tónico té verde menta equilibrante">
                    <div class="problem-header oily-skin-header">
                        <h3>Equilibrante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Té Verde y Menta</h3>
                        <ul>
                            <li>1/2 taza de té verde frío</li>
                            <li>2 cucharadas de hamamelis</li>
                            <li>5 hojas de menta fresca</li>
                        </ul>
                        <p>Tritura la menta en el té verde, añade el hamamelis. Filtra y aplica con un algodón.</p>
                        <span class="benefit-tag">Equilibrante</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <!-- ACNÉ (3) -->
                <div class="problem-card" data-category="acne" data-tags="piel grasa acné tratamiento árbol té antibacterial">
                    <div class="problem-header oily-skin-header">
                        <h3>Acné y Espinillas</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento de Ácido Salicílico Natural</h3>
                        <ul>
                            <li>1 cucharada de harina de avena</li>
                            <li>2 cucharadas de agua de hamamelis</li>
                            <li>5 gotas de aceite esencial de árbol de té</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica directamente sobre las áreas con acné. Deja actuar 20 minutos y enjuaga.</p>
                        <span class="benefit-tag">Antiacné</span>
                        <span class="benefit-tag">Antibacterial</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="acne" data-tags="piel grasa acné mascarilla arcilla tea tree">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla para Acné</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Arcilla y Tea Tree</h3>
                        <ul>
                            <li>2 cucharadas de arcilla verde</li>
                            <li>2 cucharadas de agua de hamamelis</li>
                            <li>5 gotas de aceite de árbol de té</li>
                        </ul>
                        <p>Mezcla la arcilla con hamamelis, añade el aceite. Aplica sobre zonas con acné. Deja secar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Purificante</span>
                        <span class="benefit-tag">Antiséptica</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="acne" data-tags="piel grasa acné tónico salicílico natural limón">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico para Acné</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Limón y Hamamelis</h3>
                        <ul>
                            <li>3 cucharadas de hamamelis</li>
                            <li>1 cucharada de jugo de limón</li>
                            <li>5 gotas de aceite esencial de árbol de té</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con algodón en las zonas afectadas dos veces al día.</p>
                        <span class="benefit-tag">Astringente</span>
                        <span class="benefit-tag">Antibacterial</span>
                    </div>
                </div>
                
                <!-- POROS DILATADOS (3) -->
                <div class="problem-card" data-category="poros" data-tags="piel grasa poros dilatados tratamiento arcilla">
                    <div class="problem-header oily-skin-header">
                        <h3>Poros Dilatados</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento de Arcilla para Poros</h3>
                        <ul>
                            <li>1 cucharada de arcilla verde</li>
                            <li>1 cucharada de agua de rosas</li>
                            <li>3 gotas de aceite esencial de menta</li>
                        </ul>
                        <p>Mezcla la arcilla con agua de rosas, añade aceite de menta. Aplica solo en zona T. Deja secar 10 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Minimiza poros</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="poros" data-tags="piel grasa poros dilatados tónico manzanilla limón">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico para Poros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Manzanilla y Limón</h3>
                        <ul>
                            <li>1/2 taza de infusión de manzanilla fría</li>
                            <li>1 cucharada de hamamelis</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con algodón después de limpiar el rostro.</p>
                        <span class="benefit-tag">Minimiza poros</span>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="poros" data-tags="piel grasa poros dilatados mascarilla clara huevo limón">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla para Poros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Clara de Huevo y Limón</h3>
                        <ul>
                            <li>1 clara de huevo</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Bate la clara a punto de nieve, añade limón y miel. Aplica en zona T. Deja secar 15 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Cierra poros</span>
                        <span class="benefit-tag">Tensora</span>
                    </div>
                </div>
                
                <!-- CONTROL DE BRILLO (3) -->
                <div class="problem-card" data-category="brillo" data-tags="piel grasa control brillo polvos té verde">
                    <div class="problem-header oily-skin-header">
                        <h3>Control de Brillo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Polvos Matificantes de Té Verde</h3>
                        <ul>
                            <li>2 cucharadas de arcilla blanca</li>
                            <li>1 cucharada de hojas de té verde molidas</li>
                            <li>1 cucharadita de canela en polvo (opcional)</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con una brocha grande sobre el rostro para controlar el brillo.</p>
                        <span class="benefit-tag">Matificante</span>
                        <span class="benefit-tag">Absorbente</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="brillo" data-tags="piel grasa control brillo tónico salvia menta">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico Matificante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Salvia y Menta</h3>
                        <ul>
                            <li>1/4 taza de hojas de salvia fresca</li>
                            <li>1/4 taza de hojas de menta fresca</li>
                            <li>1 taza de agua hirviendo</li>
                        </ul>
                        <p>Prepara una infusión con las hierbas. Cuando esté fría, cuela y usa como tónico facial.</p>
                        <span class="benefit-tag">Matificante</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="brillo" data-tags="piel grasa control brillo papel absorbente arroz">
                    <div class="problem-header oily-skin-header">
                        <h3>Papeles Absorbentes Caseros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Papeles de Arroz Naturales</h3>
                        <ul>
                            <li>Papel de arroz</li>
                            <li>1 cucharada de polvo de arcilla</li>
                            <li>1 cucharada de polvo de arrurruz</li>
                        </ul>
                        <p>Corta el papel de arroz en cuadrados. Mezcla los polvos y espolvorea ligeramente sobre los papeles.</p>
                        <span class="benefit-tag">Absorbente</span>
                        <span class="benefit-tag">Práctico</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Mixed Skin Page -->
    <section id="mixed-skin-page" class="remedies-page">
        <div class="container">
            <a href="#" class="back-btn" id="mixed-skin-back"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Mixta</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel mixta requiere un equilibrio perfecto entre hidratación en las zonas secas y control de sebo en la zona T. Estos tratamientos te ayudarán a balancear tu piel de manera natural.
            </p>
            
            <div class="search-results" id="mixed-skin-search-results">
                <h3>Resultados de búsqueda para: <span id="mixed-search-query"></span></h3>
                <div id="mixed-search-results-container"></div>
            </div>
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
                <button class="filter-btn" data-category="balance">Balance</button>
                <button class="filter-btn" data-category="zonal">Tratamiento Zonal</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (3) -->
                <div class="problem-card" data-category="hidratantes" data-tags="piel mixta hidratante aloe vera jojoba balance">
                    <div class="problem-header mixed-skin-header">
                        <h3>Balance Hidratante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Aloe Vera y Aceite de Jojoba</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>1 cucharadita de aceite de jojoba</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica como crema hidratante, usando menos cantidad en la zona T.</p>
                        <span class="benefit-tag">Hidratante balanceada</span>
                        <span class="benefit-tag">No comedogénica</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel mixta gel aloe vera pepino hidratación ligera">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratación Ligera</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel de Aloe Vera y Pepino</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>2 cucharadas de jugo de pepino</li>
                            <li>5 gotas de aceite esencial de neroli</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica una capa fina como hidratante diario.</p>
                        <span class="benefit-tag">Hidratante ligero</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes" data-tags="piel mixta suero jojoba tea tree equilibrante">
                    <div class="problem-header mixed-skin-header">
                        <h3>Suero Equilibrante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Jojoba y Tea Tree</h3>
                        <ul>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>3 gotas de aceite de árbol de té</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en rostro, evitando exceso en zona T.</p>
                        <span class="benefit-tag">Equilibrante</span>
                        <span class="benefit-tag">Regulador</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (3) -->
                <div class="problem-card" data-category="mascarillas" data-tags="piel mixta mascarilla plátano miel equilibrio">
                    <div class="problem-header mixed-skin-header">
                        <h3>Balance Natural</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Plátano y Miel</h3>
                        <ul>
                            <li>1/2 plátano maduro</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de jugo de limón (para zona T)</li>
                        </ul>
                        <p>Machaca el plátano y mezcla con miel. Aplica en todo el rostro, añadiendo un poco de limón solo en la zona T.</p>
                        <span class="benefit-tag">Equilibrante</span>
                        <span class="benefit-tag">Nutritiva</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel mixta mascarilla avena yogur multiusos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Multizona</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Avena y Yogur</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharada de yogur natural</li>
                            <li>1 cucharadita de miel (para zonas secas)</li>
                        </ul>
                        <p>Mezcla la avena con yogur. Aplica en todo el rostro, añadiendo un poco más de miel en las zonas secas.</p>
                        <span class="benefit-tag">Multiusos</span>
                        <span class="benefit-tag">Adaptable</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas" data-tags="piel mixta mascarilla arcilla aloe vera dual">
                    <div class="problem-header mixed-skin-header">
                        <h3>Purificante e Hidratante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Arcilla y Aloe Vera</h3>
                        <ul>
                            <li>1 cucharada de arcilla verde (para zona T)</li>
                            <li>2 cucharadas de gel de aloe vera (para mejillas)</li>
                            <li>1 cucharadita de miel (opcional para zonas secas)</li>
                        </ul>
                        <p>Aplica arcilla en zona T y aloe vera en mejillas. Deja actuar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Dual</span>
                        <span class="benefit-tag">Multizona</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (3) -->
                <div class="problem-card" data-category="exfoliantes" data-tags="piel mixta exfoliante azúcar miel adaptable">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliación Adaptada</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Azúcar y Miel</h3>
                        <ul>
                            <li>2 cucharadas de azúcar moreno</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharada de aceite de coco (para mejillas)</li>
                        </ul>
                        <p>Mezcla el azúcar con la miel. Añade más aceite de coco para las zonas secas. Exfolia con suaves movimientos circulares.</p>
                        <span class="benefit-tag">Adaptable</span>
                        <span class="benefit-tag">Personalizable</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel mixta exfoliante papaya avena suavizante">
                    <div class="problem-header mixed-skin-header">
                        <h3>Suavizante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Papaya</h3>
                        <ul>
                            <li>2 cucharadas de papaya madura triturada</li>
                            <li>1 cucharada de avena molida</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica suavemente con movimientos circulares. Deja actuar 10 minutos y enjuaga.</p>
                        <span class="benefit-tag">Suavizante</span>
                        <span class="benefit-tag">Enzimático</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes" data-tags="piel mixta exfoliante piña avena enzimático">
                    <div class="problem-header mixed-skin-header">
                        <h3>Enzimático</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Piña y Avena</h3>
                        <ul>
                            <li>2 cucharadas de piña triturada</li>
                            <li>1 cucharada de avena molida</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro con suaves movimientos. Deja actuar 5 minutos y enjuaga.</p>
                        <span class="benefit-tag">Enzimático</span>
                        <span class="benefit-tag">Suave</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (3) -->
                <div class="problem-card" data-category="tonicos" data-tags="piel mixta tónico té verde lavanda equilibrante">
                    <div class="problem-header mixed-skin-header">
                        <h3>Equilibrante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Té Verde y Lavanda</h3>
                        <ul>
                            <li>1/2 taza de té verde frío</li>
                            <li>1/4 taza de agua de hamamelis</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica con un algodón después de limpiar el rostro.</p>
                        <span class="benefit-tag">Balanceador</span>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel mixta tónico agua rosas pepino refrescante">
                    <div class="problem-header mixed-skin-header">
                        <h3>Refrescante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Agua de Rosas y Pepino</h3>
                        <ul>
                            <li>1/2 taza de agua de rosas</li>
                            <li>2 cucharadas de jugo de pepino</li>
                            <li>1 cucharadita de hamamelis</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica con un algodón por la mañana.</p>
                        <span class="benefit-tag">Refrescante</span>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos" data-tags="piel mixta tónico hamamelis menta minimizador poros">
                    <div class="problem-header mixed-skin-header">
                        <h3>Minimizador de Poros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Hamamelis y Menta</h3>
                        <ul>
                            <li>1/4 taza de hamamelis</li>
                            <li>1/4 taza de agua destilada</li>
                            <li>5 hojas de menta fresca</li>
                        </ul>
                        <p>Machaca las hojas de menta en el hamamelis, añade el agua. Filtra después de 24 horas. Aplica en zona T.</p>
                        <span class="benefit-tag">Minimizador</span>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <!-- BALANCE (3) -->
                <div class="problem-card" data-category="balance" data-tags="piel mixta balance mascarilla multitarea">
                    <div class="problem-header mixed-skin-header">
                        <h3>Balance Completo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla Multitarea</h3>
                        <ul>
                            <li>1 cucharada de arcilla verde (para zona T)</li>
                            <li>2 cucharadas de gel de aloe vera (para mejillas)</li>
                            <li>1 cucharadita de miel (para zonas secas)</li>
                        </ul>
                        <p>Aplica cada ingrediente según las necesidades de cada zona facial. Deja actuar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Multizona</span>
                        <span class="benefit-tag">Completo</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="balance" data-tags="piel mixta balance suero regulador">
                    <div class="problem-header mixed-skin-header">
                        <h3>Suero Regulador</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero Balanceador de Jojoba y Lavanda</h3>
                        <ul>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>3 gotas de aceite esencial de lavanda</li>
                            <li>2 gotas de aceite esencial de limón</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en todo el rostro, usando menos en zona T.</p>
                        <span class="benefit-tag">Regulador</span>
                        <span class="benefit-tag">Equilibrante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="balance" data-tags="piel mixta balance tratamiento nocturno">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tratamiento Nocturno</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tratamiento Nocturno de Balance</h3>
                        <ul>
                            <li>1 cucharadita de aceite de jojoba</li>
                            <li>2 gotas de aceite esencial de árbol de té (solo en zona T)</li>
                            <li>3 gotas de aceite de rosa mosqueta (solo en mejillas)</li>
                        </ul>
                        <p>Aplica los aceites específicos en cada zona según sus necesidades. No enjuagues.</p>
                        <span class="benefit-tag">Nocturno</span>
                        <span class="benefit-tag">Balanceador</span>
                    </div>
                </div>
                
                <!-- TRATAMIENTO ZONAL (3) -->
                <div class="problem-card" data-category="zonal" data-tags="piel mixta tratamiento zonal arcilla zona T">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tratamiento Zonal</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Arcilla para Zona T y Hidratante para Mejillas</h3>
                        <ul>
                            <li>Arcilla verde (para zona T)</li>
                            <li>Aceite de argán (para mejillas)</li>
                            <li>Agua de rosas (para todo el rostro)</li>
                        </ul>
                        <p>Aplica arcilla solo en la zona T. En las mejillas, usa aceite de argán. Termina rociando agua de rosas en todo el rostro.</p>
                        <span class="benefit-tag">Multizona</span>
                        <span class="benefit-tag">Personalizado</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="zonal" data-tags="piel mixta tratamiento zonal exfoliante adaptado">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliación Zonal</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliación Adaptada a Cada Zona</h3>
                        <ul>
                            <li>Exfoliante de azúcar y miel (para mejillas)</li>
                            <li>Exfoliante de avena y limón (para zona T)</li>
                            <li>Aceite de coco (para contorno de ojos)</li>
                        </ul>
                        <p>Utiliza diferentes exfoliantes según las necesidades de cada zona facial.</p>
                        <span class="benefit-tag">Adaptable</span>
                        <span class="benefit-tag">Personalizado</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="zonal" data-tags="piel mixta tratamiento zonal mascarilla dos en uno">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla Dos en Uno</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Dos Fases</h3>
                        <ul>
                            <li>Fase 1: Arcilla verde + té verde (para zona T)</li>
                            <li>Fase 2: Miel + aguacate (para mejillas y zonas secas)</li>
                        </ul>
                        <p>Prepara dos mezclas separadas. Aplica cada una en la zona correspondiente. Deja actuar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Dual</span>
                        <span class="benefit-tag">Completo</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script>
        // Datos de búsqueda para cada receta
        const recipeData = {
            'dry-skin': [],
            'oily-skin': [],
            'mixed-skin': []
        };

        // Función para mostrar la página seleccionada y ocultar las demás
        function showPage(pageId) {
            // Ocultar todas las páginas
            document.getElementById('home-page').style.display = 'none';
            document.getElementById('dry-skin-page').style.display = 'none';
            document.getElementById('oily-skin-page').style.display = 'none';
            document.getElementById('mixed-skin-page').style.display = 'none';
            
            // Remover clase active de todos los enlaces de navegación
            const navLinks = document.querySelectorAll('nav a');
            navLinks.forEach(link => link.classList.remove('active'));
            
            // Mostrar la página seleccionada
            document.getElementById(pageId + '-page').style.display = 'block';
            
            // Marcar como activo el enlace correspondiente
            document.getElementById(pageId + '-link').classList.add('active');
            
            // Scroll to top
            window.scrollTo(0, 0);
            
            // Activar filtro "Todos" por defecto
            document.querySelectorAll('.filter-btn').forEach(btn => {
                btn.classList.remove('active');
            });
            document.querySelectorAll(`#${pageId}-page .filter-btn[data-category="all"]`).forEach(btn => {
                btn.classList.add('active');
            });
            
            // Ocultar resultados de búsqueda
            document.getElementById(`${pageId}-skin-search-results`).style.display = 'none';
            
            // Mostrar todas las recetas
            filterRecipes('all', pageId);
        }
        
        // Función para filtrar recetas por categoría
        function filterRecipes(category, pageId) {
            const recipes = document.querySelectorAll(`#${pageId}-page .problem-card`);
            
            recipes.forEach(recipe => {
                if (category === 'all' || recipe.getAttribute('data-category') === category) {
                    recipe.style.display = 'block';
                } else {
                    recipe.style.display = 'none';
                }
            });
        }
        
        // Función para buscar recetas
        function searchRecipes(query, pageId) {
            const resultsContainer = document.getElementById(`${pageId}-search-results-container`);
            const searchQueryElement = document.getElementById(`${pageId}-search-query`);
            const searchResultsElement = document.getElementById(`${pageId}-skin-search-results`);
            
            // Limpiar resultados anteriores
            resultsContainer.innerHTML = '';
            
            // Mostrar el término de búsqueda
            searchQueryElement.textContent = query;
            
            // Si la query está vacía, ocultar resultados
            if (!query.trim()) {
                searchResultsElement.style.display = 'none';
                filterRecipes('all', pageId);
                return;
            }
            
            // Buscar recetas que coincidan
            const recipes = document.querySelectorAll(`#${pageId}-page .problem-card`);
            let foundResults = false;
            const searchTerms = query.toLowerCase().split(' ');
            
            recipes.forEach(recipe => {
                const tags = recipe.getAttribute('data-tags').toLowerCase();
                const title = recipe.querySelector('h3').textContent.toLowerCase();
                const header = recipe.querySelector('.problem-header h3').textContent.toLowerCase();
                const content = recipe.textContent.toLowerCase();
                
                // Verificar si todos los términos de búsqueda coinciden
                const matches = searchTerms.every(term => 
                    tags.includes(term) || title.includes(term) || header.includes(term) || content.includes(term)
                );
                
                if (matches) {
                    foundResults = true;
                    const clone = recipe.cloneNode(true);
                    resultsContainer.appendChild(clone);
                }
            });
            
            // Mostrar u ocultar resultados
            if (foundResults) {
                searchResultsElement.style.display = 'block';
                // Ocultar todas las recetas normales
                recipes.forEach(recipe => {
                    recipe.style.display = 'none';
                });
            } else {
                searchResultsElement.style.display = 'none';
                filterRecipes('all', pageId);
                alert('No se encontraron resultados para: ' + query);
            }
        }
        
        // Inicializar datos de búsqueda
        function initSearchData() {
            const skinTypes = ['dry', 'oily', 'mixed'];
            
            skinTypes.forEach(skinType => {
                const recipes = document.querySelectorAll(`#${skinType}-skin-page .problem-card`);
                recipes.forEach(recipe => {
                    const tags = recipe.getAttribute('data-tags');
                    const title = recipe.querySelector('h3').textContent;
                    const header = recipe.querySelector('.problem-header h3').textContent;
                    
                    recipeData[`${skinType}-skin`].push({
                        element: recipe,
                        tags: tags,
                        title: title,
                        header: header
                    });
                });
            });
        }
        
        // Inicializar la página mostrando la página de inicio
        document.addEventListener('DOMContentLoaded', function() {
            // Mostrar solo la página de inicio al cargar
            document.getElementById('home-page').style.display = 'block';
            document.getElementById('dry-skin-page').style.display = 'none';
            document.getElementById('oily-skin-page').style.display = 'none';
            document.getElementById('mixed-skin-page').style.display = 'none';
            
            // Inicializar datos de búsqueda
            initSearchData();
            
            // Añadir event listeners a los enlaces de navegación
            document.getElementById('home-link').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('home');
            });
            
            document.getElementById('dry-skin-link').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('dry-skin');
            });
            
            document.getElementById('oily-skin-link').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('oily-skin');
            });
            
            document.getElementById('mixed-skin-link').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('mixed-skin');
            });
            
            // Añadir event listeners a las tarjetas
            document.getElementById('dry-skin-card').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('dry-skin');
            });
            
            document.getElementById('oily-skin-card').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('oily-skin');
            });
            
            document.getElementById('mixed-skin-card').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('mixed-skin');
            });
            
            // Añadir event listeners a los botones de volver
            document.getElementById('dry-skin-back').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('home');
            });
            
            document.getElementById('oily-skin-back').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('home');
            });
            
            document.getElementById('mixed-skin-back').addEventListener('click', function(e) {
                e.preventDefault();
                showPage('home');
            });
            
            // Añadir event listeners a los enlaces del footer
            document.querySelectorAll('.footer-link').forEach(link => {
                link.addEventListener('click', function(e) {
                    e.preventDefault();
                    showPage(this.getAttribute('data-page'));
                });
            });
            
            // Añadir event listeners a los botones de filtro
            document.querySelectorAll('.filter-btn').forEach(button => {
                button.addEventListener('click', function() {
                    // Obtener la página actual
                    let currentPage = '';
                    if (document.getElementById('dry-skin-page').style.display === 'block') {
                        currentPage = 'dry-skin';
                    } else if (document.getElementById('oily-skin-page').style.display === 'block') {
                        currentPage = 'oily-skin';
                    } else if (document.getElementById('mixed-skin-page').style.display === 'block') {
                        currentPage = 'mixed-skin';
                    } else {
                        return;
                    }
                    
                    // Remover clase active de todos los botones de filtro
                    document.querySelectorAll(`#${currentPage}-page .filter-btn`).forEach(btn => {
                        btn.classList.remove('active');
                    });
                    
                    // Añadir clase active al botón clickeado
                    this.classList.add('active');
                    
                    // Ocultar resultados de búsqueda
                    document.getElementById(`${currentPage}-skin-search-results`).style.display = 'none';
                    
                    // Filtrar recetas
                    filterRecipes(this.getAttribute('data-category'), currentPage);
                });
            });
            
            // Añadir event listener al botón de búsqueda
            document.getElementById('search-button').addEventListener('click', function(e) {
                e.preventDefault();
                const searchQuery = document.getElementById('search-input').value.trim();
                
                // Determinar la página actual
                let currentPage = '';
                if (document.getElementById('dry-skin-page').style.display === 'block') {
                    currentPage = 'dry-skin';
                } else if (document.getElementById('oily-skin-page').style.display === 'block') {
                    currentPage = 'oily-skin';
                } else if (document.getElementById('mixed-skin-page').style.display === 'block') {
                    currentPage = 'mixed-skin';
                } else {
                    // Si estamos en la página de inicio, buscar en todas las páginas
                    if (searchQuery) {
                        alert('Por favor, selecciona un tipo de piel para buscar recetas específicas.');
                    }
                    return;
                }
                
                // Realizar la búsqueda
                searchRecipes(searchQuery, currentPage);
            });
            
            // Añadir event listener para la tecla Enter en el buscador
            document.getElementById('search-input').addEventListener('keypress', function(e) {
                if (e.key === 'Enter') {
                    e.preventDefault();
                    document.getElementById('search-button').click();
                }
            });
        });
    </script>
</body>
</html>
