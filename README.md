<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NaturalSkin - Remedios Naturales para el Cuidado de tu Piel</title>
    <meta name="description" content="Descubre los mejores remedios naturales para el cuidado de la piel según tu tipo: seca, grasa, mixta. Soluciones para acné, puntos negros, manchas y más.">
    <meta name="keywords" content="remedios naturales, cuidado de la piel, piel seca, piel grasa, piel mixta, acné, puntos negros, manchas, belleza natural, skincare natural">
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
        @media (max-width: 768px) {
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
                margin: 0 10px;
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
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (8) -->
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratación con Aloe Vera</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel de Aloe Vera y Pepino</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>2 cucharadas de jugo de pepino</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica sobre la piel limpia mañana y noche.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Aceite Facial Nutritivo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mezcla de Aceites Esenciales</h3>
                        <ul>
                            <li>1 cucharada de aceite de argán</li>
                            <li>1 cucharada de aceite de rosa mosqueta</li>
                            <li>5 gotas de aceite esencial de geranio</li>
                        </ul>
                        <p>Combina los aceites en un frasco oscuro. Aplica 3-4 gotas en rostro y cuello con suaves movimientos ascendentes.</p>
                        <span class="benefit-tag">Antienvejecimiento</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratante de Cacao</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Manteca de Cacao</h3>
                        <ul>
                            <li>2 cucharadas de manteca de cacao</li>
                            <li>1 cucharada de aceite de almendras dulces</li>
                            <li>5 gotas de aceite esencial de naranja</li>
                        </ul>
                        <p>Derrite la manteca de cacao al baño maría. Retira del fuego y añade los aceites. Bate hasta enfriar y aplicar.</p>
                        <span class="benefit-tag">Protector</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratante de Caléndula</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Caléndula</h3>
                        <ul>
                            <li>2 cucharadas de infusión de caléndula concentrada</li>
                            <li>1 cucharada de aceite de almendras</li>
                            <li>1 cucharadita de cera de abejas</li>
                        </ul>
                        <p>Derrite la cera de abejas y mezcla con los demás ingredientes. Bate hasta obtener una crema. Aplica diariamente.</p>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratante de Rosa Mosqueta</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Rosa Mosqueta</h3>
                        <ul>
                            <li>2 cucharadas de aceite de rosa mosqueta</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                            <li>3 gotas de aceite esencial de manzanilla</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en el rostro por la noche. Ideal para pieles secas y maduras.</p>
                        <span class="benefit-tag">Regenerador</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (8) -->
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro durante 15 minutos. Enjuaga dengan agua tibia.</p>
                        <span class="benefit-tag">Revitalizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla de Avena</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Avena y Plátano</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1/2 plátano maduro</li>
                            <li>1 cucharada de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica durante 20 minutos y enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla de Miel y Canela</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla Nutritiva</h3>
                        <ul>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharadita de canela en polvo</li>
                            <li>1 cucharada de aceite de oliva</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro durante 15 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla de Aloe Vera</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla Hidratante</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>1 cucharada de miel</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica una capa generosa y deja actuar 20 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Regeneradora</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla de Aguacate y Avena</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla Nutritiva</h3>
                        <ul>
                            <li>1/4 aguacate maduro</li>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharada de miel</li>
                        </ul>
                        <p>Machaca el aguacate y mezcla con avena y miel. Aplica durante 20 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Nutritiva</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header dry-skin-header">
                        <h3>Mascarilla de Cúrcuma</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Cúrcuma y Miel</h3>
                        <ul>
                            <li>1 cucharadita de cúrcuma en polvo</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharadita de leche</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica durante 15 minutos. Enjuaga con agua tibia. Ideal para iluminar la piel.</p>
                        <span class="benefit-tag">Iluminadora</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (8) -->
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliante de Almendras</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Almendras y Miel</h3>
                        <ul>
                            <li>2 cucharadas de almendras molidas</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de aceite de jojoba</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes circulares suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Renovador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliante de Sal Marina</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante Corporal de Sal</h3>
                        <ul>
                            <li>1/2 taza de sal marina</li>
                            <li>1/4 taza de aceite de coco</li>
                            <li>10 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Usa en la ducha con masajes circulares. Enjuaga completamente.</p>
                        <span class="benefit-tag">Mineralizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliante de Papaya</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante Enzimático de Papaya</h3>
                        <ul>
                            <li>3 cucharadas de papaya madura triturada</li>
                            <li>1 cucharada de azúcar moreno</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con suaves movimientos circulares. Deja actuar 5 minutos y enjuaga.</p>
                        <span class="benefit-tag">Iluminador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliante de Arroz</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Harina de Arroz</h3>
                        <ul>
                            <li>2 cucharadas de harina de arroz</li>
                            <li>1 cucharada de miel</li>
                            <li>2 cucharadas de leche</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica con masajes suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Suavizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header dry-skin-header">
                        <h3>Exfoliante de Miel y Bicarbonato</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante Suave</h3>
                        <ul>
                            <li>1 cucharada de bicarbonato de sodio</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharadita de aceite de oliva</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con suaves movimientos circulares. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Suavizante</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (8) -->
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico de Manzana</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Vinagre de Manzana</h3>
                        <ul>
                            <li>1 cucharada de vinagre de manzana</li>
                            <li>1/2 taza de agua destilada</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con un algodón después de la limpieza. Ideal para equilibrar el pH.</p>
                        <span class="benefit-tag">Equilibrante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico de Caléndula</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Caléndula</h3>
                        <ul>
                            <li>2 cucharadas de pétalos de caléndula secos</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de hamamelis</li>
                        </ul>
                        <p>Infusiona los pétalos en agua hirviendo 15 minutos. Cuela y añade el hamamelis. Aplica con algodón.</p>
                        <span class="benefit-tag">Antiinflamatorio</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico de Té Verde</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico Antioxidante</h3>
                        <ul>
                            <li>1 bolsa de té verde</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>5 gotas de aceite esencial de neroli</li>
                        </ul>
                        <p>Prepara el té verde y deja enfriar. Añade el aceite esencial. Conserva en refrigeración y aplica con algodón.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico de Aloe Vera</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico Hidratante</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>1/2 taza de agua de rosas</li>
                            <li>1 cucharada de hamamelis</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica con algodón por la mañana y noche.</p>
                        <span class="benefit-tag">Hidratante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header dry-skin-header">
                        <h3>Tónico de Menta y Limón</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico Revitalizante</h3>
                        <ul>
                            <li>5 hojas de menta fresca</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 taza de agua destilada</li>
                        </ul>
                        <p>Machaca las hojas de menta y mezcla con los demás ingredientes. Filtra y aplica con algodón.</p>
                        <span class="benefit-tag">Revitalizante</span>
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
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (8) -->
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratación Balanceada</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Jojoba y Lavanda</h3>
                        <ul>
                            <li>2 cucharadas de aceite de jojoba</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                            <li>3 gotas de aceite esencial de limón</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en el rostro después de la limpieza.</p>
                        <span class="benefit-tag">Balanceador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratante de Pepino</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel Refrescante de Pepino</h3>
                        <ul>
                            <li>1/2 pepino mediano</li>
                            <li>2 cucharadas de gel de aloe vera</li>
                            <li>1 cucharadita de hamamelis</li>
                        </ul>
                        <p>Licúa el pepino y cuela el jugo. Mezcla con aloe vera y hamamelis. Aplica como hidratante.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratante de Té Verde</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Té Verde</h3>
                        <ul>
                            <li>1/4 taza de té verde frío</li>
                            <li>1 cucharada de aceite de jojoba</li>
                            <li>1 cucharadita de cera de abejas</li>
                        </ul>
                        <p>Derrite la cera de abejas y mezcla con los demás ingredientes. Bate hasta enfriar. Aplica diariamente.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratante de Rosa Mosqueta</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Suero de Rosa Mosqueta</h3>
                        <ul>
                            <li>2 cucharadas de aceite de rosa mosqueta</li>
                            <li>5 gotas de aceite esencial de limón</li>
                            <li>3 gotas de aceite esencial de árbol de té</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica 2-3 gotas en el rostro por la noche.</p>
                        <span class="benefit-tag">Regenerador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratante de Semilla de Uva</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Semilla de Uva</h3>
                        <ul>
                            <li>2 cucharadas de aceite de semilla de uva</li>
                            <li>3 gotas de aceite esencial de limón</li>
                            <li>2 gotas de aceite esencial de árbol de té</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en el rostro por la mañana. Ideal para piel grasa.</p>
                        <span class="benefit-tag">Seborregulador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Hidratante de Hamamelis</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel de Hamamelis y Aloe Vera</h3>
                        <ul>
                            <li>2 cucharadas de gel de aloe vera</li>
                            <li>1 cucharada de hamamelis</li>
                            <li>3 gotas de aceite esencial de menta</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica una capa fina como hidratante.</p>
                        <span class="benefit-tag">Astringente</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (8) -->
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla de Avena</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Avena y Limón</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>2 cucharadas de agua de rosas</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro y deja actuar 15 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Limpieza suave</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla de Clara de Huevo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Clara de Huevo</h3>
                        <ul>
                            <li>1 clara de huevo</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Bate la clara a punto de nieve. Añade el limón y la miel. Aplica sobre el rostro y deja secar 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Reafirmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla de Tomate</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Tomate</h3>
                        <ul>
                            <li>1 tomate mediano</li>
                            <li>1 cucharadita de azúcar</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Tritura el tomate y mezcla con los demás ingredientes. Aplica sobre el rostro 15 minutos. Enjuaga.</p>
                        <span class="benefit-tag">Astringente</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla de Menta</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Menta y Arcilla</h3>
                        <ul>
                            <li>2 cucharadas de arcilla verde</li>
                            <li>1 cucharada de hojas de menta trituradas</li>
                            <li>2 cucharadas de agua de hamamelis</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro y deja secar 15 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla de Cáscara de Naranja</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Cáscara de Naranja</h3>
                        <ul>
                            <li>2 cucharadas de cáscara de naranja molida</li>
                            <li>1 cucharada de arcilla verde</li>
                            <li>2 cucharadas de agua de rosas</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro y deja secar 15 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (8) -->
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Exfoliante de Sal del Himalaya</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Sal y Aceite de Jojoba</h3>
                        <ul>
                            <li>3 cucharadas de sal del Himalaya fina</li>
                            <li>2 cucharadas de aceite de jojoba</li>
                            <li>5 gotas de aceite esencial de menta</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con suaves masajes circulares. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Mineralizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Exfoliante de Cáscara de Naranja</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Cáscara de Naranja</h3>
                        <ul>
                            <li>2 cucharadas de cáscara de naranja molida</li>
                            <li>1 cucharada de yogur natural</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes suaves. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Vitamínico</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Exfoliante de Bicarbonato</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Bicarbonato</h3>
                        <ul>
                            <li>2 cucharadas de bicarbonato de sodio</li>
                            <li>1 cucharada de agua</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica con suaves masajes. Enjuaga inmediatamente.</p>
                        <span class="benefit-tag">Alcalinizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Exfoliante de Harina de Garbanzo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Harina de Garbanzo</h3>
                        <ul>
                            <li>2 cucharadas de harina de garbanzo</li>
                            <li>1 cucharada de agua de rosas</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica con masajes suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Limpieza profunda</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header oily-skin-header">
                        <h3>Exfoliante de Té Verde</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Té Verde y Azúcar</h3>
                        <ul>
                            <li>2 cucharadas de hojas de té verde molidas</li>
                            <li>1 cucharada de azúcar moreno</li>
                            <li>1 cucharada de gel de aloe vera</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes circulares suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (8) -->
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico de Romero</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Romero y Limón</h3>
                        <ul>
                            <li>2 ramitas de romero fresco</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de jugo de limón</li>
                        </ul>
                        <p>Infusiona el romero en el agua 15 minutos. Cuela y añade el limón. Aplica con algodón.</p>
                        <span class="benefit-tag">Estimulante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico de Menta y Pepino</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico Refrescante</h3>
                        <ul>
                            <li>1/4 pepino mediano</li>
                            <li>5 hojas de menta fresca</li>
                            <li>1/2 taza de agua de hamamelis</li>
                        </ul>
                        <p>Licúa el pepino con la menta. Cuela y mezcla con el hamamelis. Aplica con algodón.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico de Lavanda</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Lavanda</h3>
                        <ul>
                            <li>2 cucharadas de flores de lavanda secas</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de hamamelis</li>
                        </ul>
                        <p>Infusiona la lavanda 20 minutos. Cuela y añade el hamamelis. Conserva en refrigeración.</p>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico de Manzana</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Vinagre de Manzana</h3>
                        <ul>
                            <li>1 cucharada de vinagre de manzana</li>
                            <li>1/2 taza de agua destilada</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con algodón después de la limpieza. Equilibra el pH de la piel.</p>
                        <span class="benefit-tag">Equilibrante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header oily-skin-header">
                        <h3>Tónico de Té Negro</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Té Negro</h3>
                        <ul>
                            <li>1 bolsa de té negro</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de hamamelis</li>
                        </ul>
                        <p>Prepara el té negro y deja enfriar. Añade el hamamelis. Aplica con algodón para minimizar poros.</p>
                        <span class="benefit-tag">Minimizador de poros</span>
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
            
            <div class="category-filter">
                <button class="filter-btn active" data-category="all">Todos</button>
                <button class="filter-btn" data-category="hidratantes">Hidratantes</button>
                <button class="filter-btn" data-category="mascarillas">Mascarillas</button>
                <button class="filter-btn" data-category="exfoliantes">Exfoliantes</button>
                <button class="filter-btn" data-category="tonicos">Tónicos</button>
            </div>
            
            <div class="problems-grid">
                <!-- HIDRATANTES (8) -->
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratante de Rosa Mosqueta</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Rosa Mosqueta</h3>
                        <ul>
                            <li>2 cucharadas de aceite de rosa mosqueta</li>
                            <li>3 gotas de aceite esencial de lavanda</li>
                            <li>2 gotas de aceite esencial de manzanilla</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica 2-3 gotas en las zonas secas del rostro, evitando la zona T.</p>
                        <span class="benefit-tag">Regenerador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratante de Aguacate</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Aguacate</h3>
                        <ul>
                            <li>1/4 aguacate maduro</li>
                            <li>1 cucharada de gel de aloe vera</li>
                            <li>5 gotas de aceite esencial de incienso</li>
                        </ul>
                        <p>Machaca el aguacate y mezcla con el aloe vera y el aceite esencial. Aplica en zonas secas.</p>
                        <span class="benefit-tag">Nutritivo</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratante de Caléndula</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Caléndula</h3>
                        <ul>
                            <li>2 cucharadas de infusión de caléndula</li>
                            <li>1 cucharada de aceite de almendras</li>
                            <li>1 cucharadita de cera de abejas</li>
                        </ul>
                        <p>Derrite la cera de abejas y mezcla con los demás ingredientes. Bate hasta enfriar. Aplica según necesidad.</p>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratante de Semilla de Uva</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Semilla de Uva</h3>
                        <ul>
                            <li>2 cucharadas de aceite de semilla de uva</li>
                            <li>3 gotas de aceite esencial de lavanda</li>
                            <li>2 gotas de aceite esencial de árbol de té</li>
                        </ul>
                        <p>Mezcla los aceites. Aplica solo en la zona T para regular la producción de sebo.</p>
                        <span class="benefit-tag">Seborregulador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="hidratantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratante de Té Verde</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Gel de Té Verde</h3>
                        <ul>
                            <li>1/4 taza de té verde fuerte frío</li>
                            <li>2 cucharadas de gel de aloe vera</li>
                            <li>5 gotas de aceite esencial de menta</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Conserva en refrigeración. Aplica una capa fina como hidratante.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
                
                <!-- MASCARILLAS (8) -->
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla de Miel y Canela</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Miel y Canela</h3>
                        <ul>
                            <li>2 cucharadas de miel</li>
                            <li>1/2 cucharadita de canela en polvo</li>
                            <li>1 cucharadita de jugo de limón (solo para zona T)</li>
                        </ul>
                        <p>Mezcla miel y canela. Aplica en todo el rostro, añadiendo limón solo en la zona T. Deja 15 minutos.</p>
                        <span class="benefit-tag">Antibacterial</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla de Papaya</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Papaya y Avena</h3>
                        <ul>
                            <li>3 cucharadas de papaya triturada</li>
                            <li>1 cucharada de avena molida</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro y deja actuar 15 minutos. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Exfoliante suave</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla de Aguacate</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Aguacate y Miel</h3>
                        <ul>
                            <li>1/4 aguacate maduro</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de yogur natural</li>
                        </ul>
                        <p>Machaca el aguacate y mezcla con miel y yogur. Aplica especialmente en zonas secas. Deja 20 minutos.</p>
                        <span class="benefit-tag">Nutritiva</span>
                </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla de Té Verde</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Té Verde y Arcilla</h3>
                        <ul>
                            <li>2 cucharadas de arcilla verde</li>
                            <li>2 cucharadas de té verde frío</li>
                            <li>1 cucharadita de miel (para zonas secas)</li>
                        </ul>
                        <p>Mezcla la arcilla con el té verde. Aplica en zona T, añadiendo miel en zonas secas. Deja 15 minutos.</p>
                        <span class="benefit-tag">Purificante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="mascarillas">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla de Fresa</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Fresa y Miel</h3>
                        <ul>
                            <li>3 fresas maduras</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de yogur natural</li>
                        </ul>
                        <p>Tritura las fresas y mezcla con miel y yogur. Aplica sobre el rostro 15 minutos. Enjuaga con agua fría.</p>
                        <span class="benefit-tag">Antioxidante</span>
                    </div>
                </div>
                
                <!-- EXFOLIANTES (8) -->
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliante de Café</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Café y Miel</h3>
                        <ul>
                            <li>2 cucharadas de café molido</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharada de aceite de jojoba (para zonas secas)</li>
                        </ul>
                        <p>Mezcla café y miel. Añade aceite de jojoba para las zonas secas. Aplica con masajes suaves.</p>
                        <span class="benefit-tag">Energizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliante de Avena</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Avena y Leche</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharada de leche</li>
                            <li>1 cucharadita de miel</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con suaves movimientos circulares. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Suavizante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliante de Almendras</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Almendras y Miel</h3>
                        <ul>
                            <li>2 cucharadas de almendras molidas</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de aceite de argán</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes circulares suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Nutritivo</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliante de Sal Marina</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Sal y Aceite de Oliva</h3>
                        <ul>
                            <li>2 cucharadas de sal marina fina</li>
                            <li>1 cucharada de aceite de oliva</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con masajes suaves. Enjuaga con agua tibia. Usar solo 1 vez por semana.</p>
                        <span class="benefit-tag">Renovador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="exfoliantes">
                    <div class="problem-header mixed-skin-header">
                        <h3>Exfoliante de Harina de Arroz</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Harina de Arroz y Miel</h3>
                        <ul>
                            <li>2 cucharadas de harina de arroz</li>
                            <li>1 cucharada de miel</li>
                            <li>2 cucharadas de leche</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Aplica con masajes suaves. Enjuaga con agua tibia.</p>
                        <span class="benefit-tag">Suavizante</span>
                    </div>
                </div>
                
                <!-- TÓNICOS (8) -->
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Equilibrante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Té Verde y Lavanda</h3>
                        <ul>
                            <li>1/2 taza de té verde frío</li>
                            <li>1/4 taza de agua de hamamelis</li>
                            <li>5 gotas de aceite essential de lavanda</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica con un algodón después de limpiar el rostro.</p>
                        <span class="benefit-tag">Balanceador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
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
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico de Manzanilla</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Manzanilla</h3>
                        <ul>
                            <li>2 bolsitas de manzanilla</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de hamamelis</li>
                        </ul>
                        <p>Prepara una infusión fuerte de manzanilla. Cuando enfríe, añade el hamamelis. Aplica con algodón.</p>
                        <span class="benefit-tag">Calmante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico de Romero</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Romero</h3>
                        <ul>
                            <li>2 ramitas de romero fresco</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de vinagre de manzana</li>
                        </ul>
                        <p>Infusiona el romero 15 minutos. Cuela y añade el vinagre. Aplica especialmente en zona T.</p>
                        <span class="benefit-tag">Estimulante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico de Salvia</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Salvia</h3>
                        <ul>
                            <li>1 cucharada de hojas de salvia fresca</li>
                            <li>1 taza de agua hirviendo</li>
                            <li>1 cucharada de agua de hamamelis</li>
                        </ul>
                        <p>Infusiona la salvia 10 minutos. Cuela y añade el hamamelis. Conserva en refrigeración.</p>
                        <span class="benefit-tag">Regulador</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico de Lavanda y Manzana</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Lavanda y Vinagre de Manzana</h3>
                        <ul>
                            <li>1 cucharada de vinagre de manzana</li>
                            <li>1/2 taza de agua destilada</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica con algodón después de la limpieza. Equilibra el pH de la piel.</p>
                        <span class="benefit-tag">Equilibrante</span>
                    </div>
                </div>
                
                <div class="problem-card" data-category="tonicos">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico de Té Verde y Menta</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico Refrescante</h3>
                        <ul>
                            <li>1/2 taza de té verde frío</li>
                            <li>1/4 taza de hamamelis</li>
                            <li>5 hojas de menta fresca</li>
                        </ul>
                        <p>Machaca las hojas de menta y mezcla con los demás ingredientes. Filtra y aplica con algodón.</p>
                        <span class="benefit-tag">Refrescante</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script>
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
        
        // Inicializar la página mostrando la página de inicio
        document.addEventListener('DOMContentLoaded', function() {
            // Mostrar solo la página de inicio al cargar
            document.getElementById('home-page').style.display = 'block';
            document.getElementById('dry-skin-page').style.display = 'none';
            document.getElementById('oily-skin-page').style.display = 'none';
            document.getElementById('mixed-skin-page').style.display = 'none';
            
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
                    }
                    
                    // Remover clase active de todos los botones de filtro
                    document.querySelectorAll('.filter-btn').forEach(btn => {
                        btn.classList.remove('active');
                    });
                    
                    // Añadir clase active al botón clickeado
                    this.classList.add('active');
                    
                    // Filtrar recetas
                    filterRecipes(this.getAttribute('data-category'), currentPage);
                });
            });
        });
    </script>
</body>
</html>
