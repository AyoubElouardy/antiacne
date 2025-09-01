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
                        <li><a href="#" class="active" onclick="showPage('home')">Inicio</a></li>
                        <li><a href="#" onclick="showPage('dry-skin')">Piel Seca</a></li>
                        <li><a href="#" onclick="showPage('oily-skin')">Piel Grasa</a></li>
                        <li><a href="#" onclick="showPage('mixed-skin')">Piel Mixta</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Home Page -->
    <section id="home-page" class="active">
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
                    <a href="#" onclick="showPage('dry-skin')" class="type-card">
                        <i class="fas fa-hand-holding-water dry-skin-icon"></i>
                        <h3>Piel Seca</h3>
                        <p>Remedios para hidratar, nutrir y rejuvenecer la piel seca. Soluciones para descamación, irritación y sensibilidad.</p>
                    </a>
                    <a href="#" onclick="showPage('oily-skin')" class="type-card">
                        <i class="fas fa-tint oily-skin-icon"></i>
                        <h3>Piel Grasa</h3>
                        <p>Tratamientos para regular el sebo, minimizar poros y combatir el acné. Soluciones para brillos y puntos negros.</p>
                    </a>
                    <a href="#" onclick="showPage('mixed-skin')" class="type-card">
                        <i class="fas fa-adjust mixed-skin-icon"></i>
                        <h3>Piel Mixta</h3>
                        <p>Balancea las zonas grasas y secas de tu rostro con estos remedios naturales. Equilibrio perfecto para tu piel.</p>
                    </a>
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
                            <li><a href="#" onclick="showPage('home')">Inicio</a></li>
                            <li><a href="#" onclick="showPage('dry-skin')">Piel Seca</a></li>
                            <li><a href="#" onclick="showPage('oily-skin')">Piel Grasa</a></li>
                            <li><a href="#" onclick="showPage('mixed-skin')">Piel Mixta</a></li>
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
            <a href="#" class="back-btn" onclick="showPage('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Seca</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel seca necesita hidratación intensa y nutrición profunda. Descubre estos remedios naturales para restaurar la humedad natural de tu piel y lograr un aspecto radiante.
            </p>
            
            <div class="problems-grid">
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Hidratación Intensa</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Aguacate y Miel</h3>
                        <ul>
                            <li>1/2 aguacate maduro</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharada de aceite de oliva</li>
                        </ul>
                        <p>Machaca el aguacate y mezcla con miel y aceite. Aplica sobre el rostro durante 20 minutos. Enjuaga con agua tibia.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Descamación</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Avena y Miel</h3>
                        <ul>
                            <li>3 cucharadas de avena molida</li>
                            <li>2 cucharadas de miel</li>
                            <li>1 cucharada de yogurt natural</li>
                        </ul>
                        <p>Mezcla todos los ingredientes hasta formar una pasta. Masajea suavemente sobre la piel durante 3 minutos. Enjuaga con agua fría.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Irritación y Enrojecimiento</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Compresas de Manzanilla y Aloe Vera</h3>
                        <ul>
                            <li>1 bolsa de té de manzanilla</li>
                            <li>2 cucharadas de gel de aloe vera</li>
                            <li>1 taza de agua caliente</li>
                        </ul>
                        <p>Prepara una infusión con la manzanilla. Cuando esté tibia, añade el aloe vera. Aplica con compresas sobre las zonas irritadas.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Nutrición Profunda</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Aceite de Coco y Vitamina E</h3>
                        <ul>
                            <li>2 cucharadas de aceite de coco</li>
                            <li>1 cápsula de vitamina E</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro con suaves masajes circulares antes de dormir. No enjuagues.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Limpieza Suave</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Leche de Avena Limpiadora</h3>
                        <ul>
                            <li>4 cucharadas de avena</li>
                            <li>1 taza de agua</li>
                            <li>1 cucharada de miel</li>
                        </ul>
                        <p>Deja la avena en remojo durante 2 horas. Cuela y añade la miel. Usa como leche limpiadora por las mañanas y noches.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header dry-skin-header">
                        <h3>Tonificación</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Rosas Hidratante</h3>
                        <ul>
                            <li>1 puñado de pétalos de rosa</li>
                            <li>1 taza de agua mineral</li>
                            <li>2 cucharadas de agua de hamamelis</li>
                        </ul>
                        <p>Hierve los pétalos de rosa en el agua durante 5 minutos. Deja enfriar, cuela y añade el hamamelis. Aplica con un algodón.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Oily Skin Page -->
    <section id="oily-skin-page" class="remedies-page">
        <div class="container">
            <a href="#" class="back-btn" onclick="showPage('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Grasa</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel grasa requiere regulación del sebo, limpieza profunda y minimización de poros. Estos tratamientos naturales te ayudarán a controlar el brillo y prevenir imperfecciones.
            </p>
            
            <div class="problems-grid">
                <div class="problem-card">
                    <div class="problem-header oily-skin-header">
                        <h3>Control de Brillo</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Arcilla Verde y Té Verde</h3>
                        <ul>
                            <li>2 cucharadas de arcilla verde</li>
                            <li>2 cucharadas de té verde frío</li>
                            <li>3 gotas de aceite de árbol de té</li>
                        </ul>
                        <p>Mezcla la arcilla con el té verde hasta formar una pasta. Añade el aceite de árbol de té. Aplica sobre el rostro y deja secar 15 minutos. Enjuaga con agua fría.</p>
                    </div>
                </div>
                
                <div class="problem-card">
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
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header oily-skin-header">
                        <h3>Puntos Negros</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Exfoliante de Carbón Activado y Miel</h3>
                        <ul>
                            <li>1 cápsula de carbón activado</li>
                            <li>1 cucharada de miel</li>
                            <li>1 cucharadita de azúcar moreno</li>
                        </ul>
                        <p>Mezcla el carbón con la miel y el azúcar. Aplica con suaves masajes circulares en la zona T. Enjuaga con agua tibia.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header oily-skin-header">
                        <h3>Poros Dilatados</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Agua de Rosas y Limón</h3>
                        <ul>
                            <li>1/2 taza de agua de rosas</li>
                            <li>2 cucharadas de hamamelis</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Combina todos los ingredientes en una botella con spray. Aplica después de lavar tu rostro, por la mañana y noche.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header oily-skin-header">
                        <h3>Limpieza Profunda</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Limpiador de Miel y Limón</h3>
                        <ul>
                            <li>3 cucharadas de miel</li>
                            <li>1 cucharadita de jugo de limón</li>
                            <li>1 cucharadita de aceite de jojoba</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica sobre el rostro húmedo masajeando suavemente. Enjuaga con agua tibia.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header oily-skin-header">
                        <h3>Mascarilla Purificante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Yogur y Cúrcuma</h3>
                        <ul>
                            <li>2 cucharadas de yogur natural</li>
                            <li>1/2 cucharadita de cúrcuma</li>
                            <li>1 cucharadita de jugo de limón</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica sobre el rostro evitando el contorno de ojos. Deja actuar 15 minutos y enjuaga.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Mixed Skin Page -->
    <section id="mixed-skin-page" class="remedies-page">
        <div class="container">
            <a href="#" class="back-btn" onclick="showPage('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
            <h2 class="section-title">Remedios Naturales para Piel Mixta</h2>
            <p class="section-description" style="text-align: center; margin-bottom: 40px; max-width: 800px; margin-left: auto; margin-right: auto;">
                La piel mixta requiere un equilibrio perfecto entre hidratación en las zonas secas y control de sebo en la zona T. Estos tratamientos te ayudarán a balancear tu piel de manera natural.
            </p>
            
            <div class="problems-grid">
                <div class="problem-card">
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
                        <p>Machaca el plátano y mezcla con miel. Aplica en todo el rostro, añadiendo un poco de limón solo en la zona T. Deja actuar 20 minutos.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header mixed-skin-header">
                        <h3>Hidratación Equilibrada</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Crema de Aloe Vera y Aceite de Jojoba</h3>
                        <ul>
                            <li>3 cucharadas de gel de aloe vera</li>
                            <li>1 cucharadita de aceite de jojoba</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Mezcla todos los ingredientes. Aplica como crema hidratante día y noche, usando menos cantidad en la zona T.</p>
                    </div>
                </div>
                
                <div class="problem-card">
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
                    </div>
                </div>
                
                <div class="problem-card">
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
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header mixed-skin-header">
                        <h3>Tónico Equilibrante</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Tónico de Té Verde y Lavanda</h3>
                        <ul>
                            <li>1/2 taza de té verde frío</li>
                            <li>1/4 taza de agua de hamamelis</li>
                            <li>5 gotas de aceite esencial de lavanda</li>
                        </ul>
                        <p>Combina todos los ingredientes. Aplica con un algodón después de limpiar el rostro, prestando especial atención a la zona T.</p>
                    </div>
                </div>
                
                <div class="problem-card">
                    <div class="problem-header mixed-skin-header">
                        <h3>Mascarilla Multizona</h3>
                    </div>
                    <div class="problem-content">
                        <h3>Mascarilla de Avena y Yogur</h3>
                        <ul>
                            <li>2 cucharadas de avena molida</li>
                            <li>1 cucharada de yogur natural</li>
                            <li>1 cucharadita de miel (para zonas secas)</li>
                        </ul>
                        <p>Mezcla la avena con yogur. Aplica en todo el rostro, añadiendo un poco más de miel en las zonas secas. Deja actuar 15 minutos.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <script>
        // Function to show the selected page and hide others
        function showPage(pageId) {
            // Hide all pages
            document.getElementById('home-page').classList.remove('active');
            document.getElementById('dry-skin-page').classList.remove('active');
            document.getElementById('oily-skin-page').classList.remove('active');
            document.getElementById('mixed-skin-page').classList.remove('active');
            
            // Remove active class from all nav links
            const navLinks = document.querySelectorAll('nav a');
            navLinks.forEach(link => link.classList.remove('active'));
            
            // Show the selected page
            if (pageId === 'home') {
                document.getElementById('home-page').classList.add('active');
                navLinks[0].classList.add('active');
                window.scrollTo(0, 0);
            } else if (pageId === 'dry-skin') {
                document.getElementById('dry-skin-page').classList.add('active');
                navLinks[1].classList.add('active');
                window.scrollTo(0, 0);
            } else if (pageId === 'oily-skin') {
                document.getElementById('oily-skin-page').classList.add('active');
                navLinks[2].classList.add('active');
                window.scrollTo(0, 0);
            } else if (pageId === 'mixed-skin') {
                document.getElementById('mixed-skin-page').classList.add('active');
                navLinks[3].classList.add('active');
                window.scrollTo(0, 0);
            }
        }
        
        // Initialize the page with home page visible
        document.addEventListener('DOMContentLoaded', function() {
            showPage('home');
        });
    </script>
</body>
</html>
