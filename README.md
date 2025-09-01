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
            overflow: hidden;
            height: 100vh;
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
        }
        
        nav ul li a:hover {
            color: var(--accent);
        }
        
        /* Main Content */
        .main-content {
            height: calc(100vh - 80px);
            overflow: hidden;
            position: relative;
        }
        
        /* Home Section */
        .home-section {
            height: 100%;
            display: flex;
            flex-direction: column;
        }
        
        .hero {
            background: linear-gradient(rgba(93, 138, 130, 0.8), rgba(58, 90, 83, 0.9)), url('https://images.unsplash.com/photo-1596462502278-27bfdc403348?ixlib=rb-4.0.3&auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
            color: white;
            padding: 40px 0;
            text-align: center;
            flex: 1;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .hero-content {
            max-width: 800px;
            margin: 0 auto;
        }
        
        .hero h1 {
            font-size: 36px;
            margin-bottom: 20px;
            line-height: 1.2;
        }
        
        .hero p {
            font-size: 18px;
            margin-bottom: 30px;
        }
        
        .btn {
            display: inline-block;
            background-color: var(--accent);
            color: #333;
            padding: 12px 25px;
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
            padding: 40px 0;
            background-color: white;
        }
        
        .section-title {
            text-align: center;
            margin-bottom: 30px;
            color: var(--primary);
            font-size: 28px;
        }
        
        .types-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        
        .type-card {
            background-color: var(--light);
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
            cursor: pointer;
        }
        
        .type-card:hover {
            transform: translateY(-5px);
        }
        
        .type-card i {
            font-size: 40px;
            margin-bottom: 15px;
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
            margin-bottom: 10px;
            color: var(--dark);
        }
        
        /* Remedies Sections (initially hidden) */
        .remedies-section {
            display: none;
            height: 100%;
            overflow-y: auto;
            padding: 20px 0;
            background-color: #f1f5f9;
        }
        
        .remedies-section.active {
            display: block;
        }
        
        .back-btn {
            display: inline-flex;
            align-items: center;
            color: var(--primary);
            text-decoration: none;
            font-weight: 600;
            margin-bottom: 20px;
            padding: 8px 16px;
            border-radius: 50px;
            background-color: white;
            box-shadow: 0 3px 10px rgba(0, 0, 0, 0.1);
            transition: all 0.3s;
        }
        
        .back-btn:hover {
            background-color: var(--primary);
            color: white;
        }
        
        .back-btn i {
            margin-right: 8px;
        }
        
        .problems-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
            margin-bottom: 30px;
        }
        
        .problem-card {
            background-color: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s;
        }
        
        .problem-card:hover {
            transform: translateY(-3px);
        }
        
        .problem-header {
            padding: 15px;
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
            padding: 20px;
        }
        
        .problem-content h3 {
            color: var(--primary);
            margin-bottom: 12px;
            font-size: 18px;
        }
        
        .problem-content ul {
            padding-left: 20px;
            margin-bottom: 15px;
        }
        
        .problem-content li {
            margin-bottom: 8px;
            font-size: 14px;
        }
        
        .problem-content p {
            font-size: 14px;
        }
        
        /* Responsive */
        @media (max-width: 768px) {
            .header-content {
                flex-direction: column;
                text-align: center;
            }
            
            nav ul {
                margin-top: 15px;
                justify-content: center;
                flex-wrap: wrap;
            }
            
            nav ul li {
                margin: 5px 10px;
            }
            
            .hero h1 {
                font-size: 28px;
            }
            
            .hero p {
                font-size: 16px;
            }
            
            .types-grid {
                grid-template-columns: 1fr;
            }
            
            .problems-grid {
                grid-template-columns: 1fr;
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
                    <i class="fas fa-leaf"></i>
                    <span>NaturalSkin</span>
                </div>
                <nav>
                    <ul>
                        <li><a href="#" onclick="showSection('home')">Inicio</a></li>
                        <li><a href="#" onclick="showSection('dry-skin')">Piel Seca</a></li>
                        <li><a href="#" onclick="showSection('oily-skin')">Piel Grasa</a></li>
                        <li><a href="#" onclick="showSection('mixed-skin')">Piel Mixta</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <div class="main-content">
        <!-- Home Section -->
        <section id="home-section" class="home-section">
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
                        <div class="type-card" onclick="showSection('dry-skin')">
                            <i class="fas fa-hand-holding-water dry-skin-icon"></i>
                            <h3>Piel Seca</h3>
                            <p>Remedios para hidratar, nutrir y rejuvenecer la piel seca.</p>
                        </div>
                        <div class="type-card" onclick="showSection('oily-skin')">
                            <i class="fas fa-oil-can oily-skin-icon"></i>
                            <h3>Piel Grasa</h3>
                            <p>Tratamientos para regular el sebo y combatir el acné.</p>
                        </div>
                        <div class="type-card" onclick="showSection('mixed-skin')">
                            <i class="fas fa-blender mixed-skin-icon"></i>
                            <h3>Piel Mixta</h3>
                            <p>Balancea las zonas grasas y secas de tu rostro.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Dry Skin Section -->
        <section id="dry-skin-section" class="remedies-section">
            <div class="container">
                <a href="#" class="back-btn" onclick="showSection('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
                <h2 class="section-title">Remedios Naturales para Piel Seca</h2>
                
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
                            <h3>Irritación</h3>
                        </div>
                        <div class="problem-content">
                            <h3>Compresas de Manzanilla</h3>
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
                </div>
            </div>
        </section>

        <!-- Oily Skin Section -->
        <section id="oily-skin-section" class="remedies-section">
            <div class="container">
                <a href="#" class="back-btn" onclick="showSection('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
                <h2 class="section-title">Remedios Naturales para Piel Grasa</h2>
                
                <div class="problems-grid">
                    <div class="problem-card">
                        <div class="problem-header oily-skin-header">
                            <h3>Control de Brillo</h3>
                        </div>
                        <div class="problem-content">
                            <h3>Mascarilla de Arcilla Verde</h3>
                            <ul>
                                <li>2 cucharadas de arcilla verde</li>
                                <li>2 cucharadas de té verde frío</li>
                                <li>3 gotas de aceite de árbol de té</li>
                            </ul>
                            <p>Mezcla la arcilla con el té verde hasta formar una pasta. Añade el aceite de árbol de té. Aplica sobre el rostro y deja secar 15 minutos.</p>
                        </div>
                    </div>
                    
                    <div class="problem-card">
                        <div class="problem-header oily-skin-header">
                            <h3>Acné y Espinillas</h3>
                        </div>
                        <div class="problem-content">
                            <h3>Tratamiento Natural</h3>
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
                            <h3>Exfoliante de Carbón Activado</h3>
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
                            <h3>Tónico de Agua de Rosas</h3>
                            <ul>
                                <li>1/2 taza de agua de rosas</li>
                                <li>2 cucharadas de hamamelis</li>
                                <li>1 cucharadita de jugo de limón</li>
                            </ul>
                            <p>Combina todos los ingredientes en una botella con spray. Aplica después de lavar tu rostro, por la mañana y noche.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Mixed Skin Section -->
        <section id="mixed-skin-section" class="remedies-section">
            <div class="container">
                <a href="#" class="back-btn" onclick="showSection('home')"><i class="fas fa-arrow-left"></i> Volver al Inicio</a>
                <h2 class="section-title">Remedios Naturales para Piel Mixta</h2>
                
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
                            <h3>Crema de Aloe Vera</h3>
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
                            <h3>Arcilla para Zona T</h3>
                            <ul>
                                <li>Arcilla verde (para zona T)</li>
                                <li>Aceite de argán (para mejillas)</li>
                                <li>Agua de rosas (para todo el rostro)</li>
                            </ul>
                            <p>Aplica arcilla solo en la zona T. En las mejillas, usa aceite de argán. Termina rociando agua de rosas en todo el rostro.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </div>

    <script>
        // Function to show the selected section and hide others
        function showSection(sectionId) {
            // Hide all sections
            document.getElementById('home-section').classList.remove('active');
            document.getElementById('dry-skin-section').classList.remove('active');
            document.getElementById('oily-skin-section').classList.remove('active');
            document.getElementById('mixed-skin-section').classList.remove('active');
            
            // Show the selected section
            if (sectionId === 'home') {
                document.getElementById('home-section').classList.add('active');
            } else if (sectionId === 'dry-skin') {
                document.getElementById('dry-skin-section').classList.add('active');
            } else if (sectionId === 'oily-skin') {
                document.getElementById('oily-skin-section').classList.add('active');
            } else if (sectionId === 'mixed-skin') {
                document.getElementById('mixed-skin-section').classList.add('active');
            }
        }
        
        // Initialize the page with home section visible
        document.addEventListener('DOMContentLoaded', function() {
            showSection('home');
        });
    </script>
</body>
</html>
