<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Recursos de Marketing - Enter</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600;700;800&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Open Sans', sans-serif;
            min-height: 100vh;
            background: url('data:image/jpeg;base64,/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAMCAgMCAgMDAwMEAwMEBQgFBQQEBQoHBwYIDAoMDAsKCwsNDhIQDQ4RDgsLEBYQERMUFRUVDA8XGBYUGBIUFRT/2wBDAQMEBAUEBQkFBQkUDQsNFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBQUFBT/wAARCABkAGQDASIAAhEBAxEB/8QAHwAAAQUBAQEBAQEAAAAAAAAAAAECAwQFBgcICQoL/8QAtRAAAgEDAwIEAwUFBAQAAAF9AQIDAAQRBRIhMUEGE1FhByJxFDKBkaEII0KxwRVS0fAkM2JyggkKFhcYGRolJicoKSo0NTY3ODk6Q0RFRkdISUpTVFVWV1hZWmNkZWZnaGlqc3R1dnd4eXqDhIWGh4iJipKTlJWWl5iZmqKjpKWmp6ipqrKztLW2t7i5usLDxMXGx8jJytLT1NXW19jZ2uHi4+Tl5ufo6erx8vP09fb3+Pn6/8QAHwEAAwEBAQEBAQEBAQAAAAAAAAECAwQFBgcICQoL/8QAtREAAgECBAQDBAcFBAQAAQJ3AAECAxEEBSExBhJBUQdhcRMiMoEIFEKRobHBCSMzUvAVYnLRChYkNOEl8RcYGRomJygpKjU2Nzg5OkNERUZHSElKU1RVVldYWVpjZGVmZ2hpanN0dXZ3eHl6goOEhYaHiImKkpOUlZaXmJmaoqOkpaanqKmqsrO0tba3uLm6wsPExcbHyMnK0tPU1dbX2Nna4uPk5ebn6Onq8vP09fb3+Pn6/9oADAMBAAIRAxEAPwD9/KKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigAooooAKKKKACiiigD//Z') no-repeat center center fixed;
            background-size: cover;
            position: relative;
            overflow-x: hidden;
        }

        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background: linear-gradient(135deg, #1e2bff 0%, #3633d4 25%, #7b1eff 75%, #8732ff 100%);
            opacity: 0.88;
            z-index: 1;
        }

        .main-container {
            position: relative;
            z-index: 2;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 60px 40px;
            color: white;
        }

        .hero-section {
            text-align: center;
            margin-bottom: 60px;
            animation: fadeInUp 1s ease-out;
        }

        .main-title {
            font-size: 10rem;
            font-weight: 800;
            margin-bottom: 50px;
            color: white;
            letter-spacing: -2px;
        }

        .header-image {
            max-width: 250px;
            width: 100%;
            height: auto;
            margin: 0 auto;
            display: block;
            border-radius: 15px;
            animation: fadeInUp 1.3s ease-out;
        }

        .resources-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(380px, 1fr));
            gap: 30px;
            max-width: 1400px;
            width: 100%;
            animation: fadeInUp 1.2s ease-out;
        }

        .resource-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(20px);
            border-radius: 20px;
            padding: 30px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: all 0.4s cubic-bezier(0.4, 0, 0.2, 1);
            position: relative;
            overflow: hidden;
        }

        .resource-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.1), transparent);
            transition: left 0.6s;
        }

        .resource-card:hover::before {
            left: 100%;
        }

        .resource-card:hover {
            transform: translateY(-10px);
            background: rgba(255, 255, 255, 0.15);
            border-color: rgba(255, 255, 255, 0.3);
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
        }

        .card-title {
            font-size: 1.6rem;
            font-weight: 700;
            margin-bottom: 15px;
            color: white;
            display: flex;
            align-items: center;
            gap: 12px;
        }

        .card-description {
            font-size: 1rem;
            opacity: 0.9;
            margin-bottom: 25px;
            line-height: 1.5;
        }

        .resource-links {
            display: flex;
            flex-direction: column;
            gap: 12px;
        }

        .resource-link {
            display: flex;
            align-items: center;
            gap: 12px;
            padding: 15px 20px;
            background: rgba(255, 255, 255, 0.1);
            border: 1px solid rgba(255, 255, 255, 0.2);
            border-radius: 12px;
            color: white;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.95rem;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .resource-link::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent);
            transition: left 0.5s;
        }

        .resource-link:hover::before {
            left: 100%;
        }

        .resource-link:hover {
            background: rgba(255, 255, 255, 0.2);
            border-color: rgba(255, 255, 255, 0.4);
            transform: translateX(5px);
        }

        .link-icon {
            font-size: 1.2rem;
            flex-shrink: 0;
        }

        .floating-elements {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .floating-shape {
            position: absolute;
            background: rgba(255, 255, 255, 0.05);
            border-radius: 50%;
            animation: float 8s ease-in-out infinite;
        }

        .floating-shape:nth-child(1) {
            width: 100px;
            height: 100px;
            top: 10%;
            left: 10%;
            animation-delay: 0s;
        }

        .floating-shape:nth-child(2) {
            width: 150px;
            height: 150px;
            top: 60%;
            right: 15%;
            animation-delay: 3s;
        }

        .floating-shape:nth-child(3) {
            width: 80px;
            height: 80px;
            bottom: 20%;
            left: 20%;
            animation-delay: 6s;
        }

        .floating-shape:nth-child(4) {
            width: 120px;
            height: 120px;
            top: 30%;
            right: 30%;
            animation-delay: 2s;
        }

        @keyframes float {
            0%, 100% { 
                transform: translateY(0px) rotate(0deg); 
                opacity: 0.3;
            }
            33% { 
                transform: translateY(-20px) rotate(120deg); 
                opacity: 0.7;
            }
            66% { 
                transform: translateY(-10px) rotate(240deg); 
                opacity: 0.5;
            }
        }

        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(50px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .footer {
            margin-top: 40px;
            text-align: center;
            font-size: 0.9rem;
            opacity: 0.7;
            animation: fadeInUp 1.8s ease-out;
        }

        @media (max-width: 1200px) {
            .resources-grid {
                grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            }
        }

        @media (max-width: 768px) {
            .main-title {
                font-size: 6rem;
            }
            
            .resources-grid {
                grid-template-columns: 1fr;
                gap: 20px;
            }
            
            .main-container {
                padding: 40px 20px;
            }

            .header-image {
                max-width: 200px;
            }
        }
    </style>
</head>
<body>
    <div class="floating-elements">
        <div class="floating-shape"></div>
        <div class="floating-shape"></div>
        <div class="floating-shape"></div>
        <div class="floating-shape"></div>
    </div>

    <div class="main-container">
        <div class="hero-section">
            <h2 class="main-title">Algunos recursos de Marketing para Enter ;)</h2>
            <img src="https://camo.githubusercontent.com/d271e289c17ffea98e27321213e389a1734b66ca381dd105dc8b65985e2ceb5f/68747470733a2f2f64726976652e676f6f676c652e636f6d2f75633f6578706f72743d766965772669643d3141514366504876415167424d627651396b6d735051317851626c54764e37782d" 
                 alt="Enter Tech School" 
                 class="header-image">
        </div>

        <div class="resources-grid">
            <!-- PLANTILLAS -->
            <div class="resource-card">
                <h3 class="card-title">📋 Plantillas de Diseño</h3>
                <p class="card-description">Plantillas editables en Canva para presentaciones, eventos y comunicaciones.</p>
                <div class="resource-links">
                    <a href="https://www.canva.com/design/DAGyfrzcF4w/pSB8_5Rh_wC3g_E8OLNb0Q/edit?utm_content=DAGyfrzcF4w&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">🎨</span>
                        PPT
                    </a>
                    <a href="https://www.canva.com/design/DAG0YdvlzUg/QufZjITNLzHDIa4d3szuQQ/edit?utm_content=DAG0YdvlzUg&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">🚀</span>
                        KICK OFF
                    </a>
                    <a href="https://www.canva.com/design/DAGzvu2UTgU/3HwpNxIW3EpzOGlP_QjGCQ/edit?utm_content=DAGzvu2UTgU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">🎤</span>
                        DEMO DAY
                    </a>
                    <a href="https://www.canva.com/design/DAGRx-FfqHk/3tbD72N1suo28G2IBd0KgA/edit?utm_content=DAGRx-FfqHk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">📧</span>
                        Flyers / Correos
                    </a>
                    <a href="https://www.canva.com/design/DAGQAcdy16Q/L9bZURo1dgQ7xkV3lpiF4w/edit?utm_content=DAGQAcdy16Q&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">📬</span>
                        Cabeceras para Correo
                    </a>
                    <a href="https://www.canva.com/design/DAGnQAJst2s/cn0pLUCeXhnOhkHI-jzq8w/edit?utm_content=DAGnQAJst2s&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">📱</span>
                        Paid Media
                    </a>
                </div>
            </div>

            <!-- BROCHURES -->
            <div class="resource-card">
                <h3 class="card-title">📄 Brochures</h3>
                <p class="card-description">Brochures digitales de nuestros programas educativos.</p>
                <div class="resource-links">
                    <a href="https://landing.enter.edu.pe/brochure-fullstack" class="resource-link" target="_blank">
                        <span class="link-icon">💻</span>
                        Desarrollo Web
                    </a>
                    <a href="https://landing.enter.edu.pe/brochure-cybersecurity" class="resource-link" target="_blank">
                        <span class="link-icon">🔐</span>
                        Ciberseguridad
                    </a>
                    <a href="https://landing.enter.edu.pe/brochure-data-analytics" class="resource-link" target="_blank">
                        <span class="link-icon">📊</span>
                        Análisis de Datos
                    </a>
                </div>
            </div>

            <!-- BROCHURES EDITABLES -->
            <div class="resource-card">
                <h3 class="card-title">✏️ Brochures Editables</h3>
                <p class="card-description">Versiones editables de los brochures en Canva para personalización.</p>
                <div class="resource-links">
                    <a href="https://www.canva.com/design/DAGqJ56KIQ0/ccjcEGwcYIJxOxMwuQQS2A/edit?utm_content=DAGqJ56KIQ0&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">💻</span>
                        Desarrollo Web - Editable
                    </a>
                    <a href="https://www.canva.com/design/DAGplh84ty8/2gL25wvXHdg_vy_43Ixk0Q/edit?utm_content=DAGplh84ty8&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">🔐</span>
                        Ciberseguridad - Editable
                    </a>
                    <a href="https://www.canva.com/design/DAGuPMfMffw/0aEmLLeukLV4T_lXYU2csw/edit?utm_content=DAGuPMfMffw&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">📊</span>
                        Análisis de Datos - Editable
                    </a>
                </div>
            </div>

            <!-- RECURSOS DE MARCA -->
            <div class="resource-card">
                <h3 class="card-title">🎯 Recursos de Marca</h3>
                <p class="card-description">Guía de identidad visual, logos, colores y elementos de marca.</p>
                <div class="resource-links">
                    <a href="https://landing.enter.edu.pe/brandbook" class="resource-link" target="_blank">
                        <span class="link-icon">📘</span>
                        Brandbook
                    </a>
                    <a href="https://www.canva.com/design/DAGeQRFkLWU/WWlA_pnlet-faX-I1A67Kg/edit?utm_content=DAGeQRFkLWU&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton" class="resource-link" target="_blank">
                        <span class="link-icon">🎨</span>
                        Recursos y Gráficos
                    </a>
                </div>
            </div>

            <!-- ENTERS BENEFITS -->
            <div class="resource-card">
                <h3 class="card-title">🌟 Enters Benefits</h3>
                <p class="card-description">Información sobre beneficios exclusivos y rankings de estudiantes.</p>
                <div class="resource-links">
                    <a href="https://landing.enter.edu.pe/enters-benefits" class="resource-link" target="_blank">
                        <span class="link-icon">🎓</span>
                        Benefits - Estudiantes
                    </a>
                    <a href="https://landing.enter.edu.pe/beneficios" class="resource-link" target="_blank">
                        <span class="link-icon">✨</span>
                        Benefits - Leads
                    </a>
                    <a href="https://www.canva.com/design/DAGquDebgBM/H0Bw9JxL1dE1xHkwRBkZWA/edit" class="resource-link" target="_blank">
                        <span class="link-icon">🏆</span>
                        Ranking
                    </a>
                </div>
            </div>
        </div>

        <div class="footer">
            <p>💜 Enter Tech School - Esa gente, hablen pes</p>
        </div>
    </div>
</body>
</html>
