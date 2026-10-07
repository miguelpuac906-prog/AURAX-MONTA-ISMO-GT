<p align="center">
  <img src="assets/logo.png" alt="AURAX Logo" width="200"/>
</p>
<img width="1200" height="630" alt="image" src="https://github.com/user-attachments/assets/9608a093-5d0f-4bfa-bfe4-fb05d0002e9a" />
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AURAX MONTAÑISMO GT | Historia, Expediciones & Merch</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            scroll-behavior: smooth;
        }

        body {
            background-color: #0A0A0A;
            color: #FFFFFF;
            line-height: 1.6;
            padding-top: 70px;
        }

        /* Header Navigation */
        header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(18, 18, 18, 0.95);
            backdrop-filter: blur(8px);
            border-bottom: 2px solid #5CE1E6;
            padding: 10px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
        }

        .header-brand {
            display: flex;
            align-items: center;
            gap: 12px;
            cursor: pointer;
        }

        /* Espacio para el Logotipo */
        .header-logo {
            height: 45px;
            width: auto;
            max-width: 50px;
            object-fit: contain;
            /* Si la imagen no carga, muestra un estilo reservado limpio */
            background-color: #1A1A1A;
            border-radius: 6px;
        }

        .logo-badge {
            font-size: 1.8rem;
            font-weight: 900;
            color: #FFFFFF;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        .logo-badge span {
            color: #5CE1E6;
        }

        nav ul {
            display: flex;
            list-style: none;
            gap: 20px;
        }

        nav a {
            color: #FFFFFF;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            font-size: 0.85rem;
            transition: color 0.3s ease;
        }

        nav a:hover {
            color: #5CE1E6;
        }

        .cart-trigger {
            background-color: #5CE1E6;
            color: #000000;
            padding: 8px 18px;
            border-radius: 20px;
            cursor: pointer;
            font-weight: bold;
            transition: transform 0.2s ease, background-color 0.2s ease;
        }

        .cart-trigger:hover {
            transform: scale(1.05);
            background-color: #4ac8cc;
        }

        .cart-count {
            background-color: #FF4D4D;
            color: #FFFFFF;
            padding: 2px 7px;
            border-radius: 50%;
            font-size: 0.8rem;
            margin-left: 5px;
        }

        /* Hero Section */
        .hero {
            text-align: center;
            padding: 80px 20px;
            background: linear-gradient(180deg, #121212 0%, #0A0A0A 100%);
            border-bottom: 1px solid #222222;
        }

        .hero h1 {
            font-size: 3rem;
            color: #FFFFFF;
            margin-bottom: 10px;
            font-weight: 800;
        }

        .hero h1 span {
            color: #5CE1E6;
        }

        .hero-subtitle {
            font-size: 1.5rem;
            color: #5CE1E6;
            font-weight: 600;
            margin-bottom: 8px;
        }

        .hero-slogan {
            font-size: 1.1rem;
            color: #B0B0B0;
            font-style: italic;
            margin-bottom: 30px;
        }

        .btn {
            display: inline-block;
            background-color: #5CE1E6;
            color: #000000;
            padding: 12px 25px;
            border-radius: 25px;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            margin: 5px;
            border: none;
            cursor: pointer;
            transition: all 0.3s ease;
            font-size: 0.9rem;
        }

        .btn:hover {
            opacity: 0.9;
            transform: translateY(-2px);
        }

        .btn-ws {
            background-color: #25D366;
            color: #FFFFFF;
        }

        .btn-social {
            background-color: #1A1A1A;
            color: #5CE1E6;
            border: 1px solid #5CE1E6;
        }

        /* Secciones */
        section {
            padding: 60px 5%;
        }

        .section-title {
            text-align: center;
            font-size: 2rem;
            color: #5CE1E6;
            text-transform: uppercase;
            margin-bottom: 35px;
            border-bottom: 2px solid #5CE1E6;
            padding-bottom: 10px;
            max-width: 600px;
            margin-left: auto;
            margin-right: auto;
        }

        /* Grid de Servicios y Productos */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 25px;
        }

        .product-card {
            background-color: #141414;
            border: 1px solid #282828;
            border-radius: 12px;
            padding: 25px;
            text-align: center;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
            transition: border-color 0.3s ease, transform 0.3s ease;
        }

        .product-card:hover {
            border-color: #5CE1E6;
            transform: translateY(-5px);
        }

        .product-icon {
            font-size: 3.2rem;
            margin-bottom: 15px;
        }

        .product-title {
            font-size: 1.25rem;
            color: #FFFFFF;
            margin-bottom: 10px;
            font-weight: bold;
        }

        .product-price {
            font-size: 1.4rem;
            color: #5CE1E6;
            font-weight: bold;
            margin-bottom: 15px;
        }

        /* Mascota Section */
        .mascot-box {
            background-color: #141414;
            border: 2px solid #5CE1E6;
            border-radius: 12px;
            padding: 30px;
            margin-bottom: 40px;
            display: flex;
            align-items: center;
            gap: 25px;
        }

        .mascot-icon {
            font-size: 4.5rem;
            line-height: 1;
        }

        .mascot-text h3 {
            color: #5CE1E6;
            font-size: 1.6rem;
            margin-bottom: 8px;
        }

        /* Historia & Expediciones Timeline */
        .history-box {
            background-color: #141414;
            border-left: 4px solid #5CE1E6;
            border-radius: 8px;
            padding: 25px 30px;
            margin-bottom: 30px;
        }

        .history-box p {
            font-size: 1.05rem;
            color: #DDDDDD;
            margin-bottom: 15px;
        }

        .expeditions-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 20px;
            margin-top: 25px;
        }

        .expedition-card {
            background-color: #121212;
            border: 1px solid #282828;
            border-radius: 10px;
            padding: 20px;
            border-top: 3px solid #5CE1E6;
        }

        .expedition-card h4 {
            color: #5CE1E6;
            font-size: 1.15rem;
            margin-bottom: 8px;
        }

        .expedition-badge {
            display: inline-block;
            background-color: rgba(92, 225, 230, 0.15);
            color: #5CE1E6;
            font-size: 0.8rem;
            font-weight: bold;
            padding: 3px 10px;
            border-radius: 12px;
            margin-bottom: 10px;
        }

        /* Estrategia & Objetivos */
        .card-box {
            background-color: #141414;
            border: 1px solid #5CE1E6;
            border-radius: 10px;
            padding: 30px;
            margin-bottom: 25px;
        }

        .card-box h3 {
            color: #5CE1E6;
            margin-bottom: 12px;
            font-size: 1.5rem;
        }

        .obj-list {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 15px;
            margin-top: 20px;
        }

        .obj-item {
            background-color: #0A0A0A;
            padding: 15px;
            border-left: 4px solid #5CE1E6;
            border-radius: 4px;
            font-size: 0.95rem;
        }

        /* Social Bar */
        .social-links {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 20px;
        }

        /* Carrito Sidebar */
        .cart-sidebar {
            position: fixed;
            top: 0;
            right: -400px;
            width: 360px;
            max-width: 100%;
            height: 100%;
            background-color: #121212;
            border-left: 2px solid #5CE1E6;
            z-index: 2000;
            padding: 25px;
            transition: right 0.3s ease;
            display: flex;
            flex-direction: column;
        }

        .cart-sidebar.active {
            right: 0;
        }

        .cart-items-container {
            flex-grow: 1;
            overflow-y: auto;
            margin-top: 15px;
        }

        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid #282828;
            font-size: 0.95rem;
        }

        .cart-item-details {
            display: flex;
            flex-direction: column;
            gap: 4px;
        }

        .remove-btn {
            background: none;
            border: none;
            color: #FF4D4D;
            cursor: pointer;
            font-weight: bold;
            font-size: 1.1rem;
            margin-left: 10px;
        }

        footer {
            text-align: center;
            padding: 25px;
            background-color: #050505;
            color: #888888;
            font-size: 0.85rem;
            border-top: 1px solid #1A1A1A;
        }

        @media (max-width: 768px) {
            header { 
                flex-direction: column; 
                gap: 12px; 
                padding: 12px 5%;
            }
            body { 
                padding-top: 130px; 
            }
            .hero h1 { 
                font-size: 2.2rem; 
            }
            .hero-subtitle { 
                font-size: 1.2rem; 
            }
            .mascot-box {
                flex-direction: column;
                text-align: center;
            }
        }
    </style>
</head>
<body>

    <!-- Header Navigation con Logotipo -->
    <header>
        <div class="header-brand" onclick="window.scrollTo({top: 0, behavior: 'smooth'})">
            <!-- Reemplaza 'assets/logo.png' por la ruta o URL de tu logo -->
            <img src="assets/logo.png" alt="AURAX Logo" class="header-logo" onerror="this.style.display='none'">
            <div class="logo-badge">AURA<span>X</span> GT</div>
        </div>
        <nav>
            <ul>
                <li><a href="#inicio">Inicio</a></li>
                <li><a href="#historia">Nuestra Historia</a></li>
                <li><a href="#servicios">Expediciones & Merch</a></li>
                <li><a href="#estrategia">Nosotros</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
        <div class="cart-trigger" onclick="toggleCart()">
            🛒 Solicitud (<span id="cartCount">0</span>)
        </div>
    </header>

    <!-- Hero Section -->
    <section id="inicio" class="hero">
        <h1>AURAX <span>MONTAÑISMO GT</span></h1>
        <div class="hero-subtitle">"Más que caminar, vivir la montaña"</div>
        <div class="hero-slogan">"Conquistando a Guate desde lo alto."</div>
        
        <div>
            <a href="#servicios" class="btn">Ver Expediciones & Merch</a>
            <a href="https://wa.me/50254342015?text=Hola%20AuraX%20Monta%C3%B1ismo!%20Quiero%20m%C3%A1s%20informaci%C3%B3n." target="_blank" class="btn btn-ws">
                📱 WhatsApp (5434-2015)
            </a>
        </div>
    </section>

    <!-- SECCIÓN HISTORIA Y EXPEDICIONES REALIZADAS -->
    <section id="historia">
        <h2 class="section-title">Nuestra Historia</h2>
        
        <div class="history-box">
            <p><strong>AURAX MONTAÑISMO GT</strong> nació en la ciudad de Quetzaltenango a partir de la pasión compartida por el entrenamiento funcional, el acondicionamiento físico y el amor por las cumbres. Lo que comenzó en septiembre de 2025 como caminatas de entrenamiento al aire libre con alumnos y amigos del gimnasio, pronto se transformó en una verdadera vocación por guiar y compartir la majestuosidad de nuestras montañas.</p>
            <p>Para <strong>noviembre de 2025</strong>, el proyecto tomó forma oficial bajo el nombre de <strong>AURAX GT</strong>, estableciendo una propuesta de aventuras seguras, técnica profesional y un fuerte sentido de comunidad donde cada participante es parte indispensable de la manada.</p>
        </div>

        <h3 style="color: #5CE1E6; font-size: 1.5rem; text-align: center; margin-top: 40px; margin-bottom: 20px;">
            🌋 Expediciones Emblemáticas Que Hemos Conquistado
        </h3>

        <div class="expeditions-grid">
            <div class="expedition-card">
                <span class="expedition-badge">Tradición & Cumbre</span>
                <h4>Volcán Santa María</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Icono de Xela. Hemos realizado múltiples ascensos grupales en diferentes épocas del año, celebrando cumbres con paisajes inolvidables de la sierra occidental.</p>
            </div>

            <div class="expedition-card">
                <span class="expedition-badge">Noche & Fuego</span>
                <h4>Nocturna a Volcán Pacaya</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Una caminata bajo las estrellas apreciando el resplandor de la lava y concluyendo con la visita cultural por Antigua Guatemala.</p>
            </div>

            <div class="expedition-card">
                <span class="expedition-badge">Internacional</span>
                <h4>Volcán Ilamatepec (El Salvador)</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Expedición express internacional hacia la impresionante laguna de azufre del cráter de Santa Ana y el Sunset Park en la costa salvadoreña.</p>
            </div>

            <div class="expedition-card">
                <span class="expedition-badge">Amanecer Mágico</span>
                <h4>Rostro Maya (San Juan La Laguna)</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Ascenso matutino para apreciar uno de los amaneceres más espectaculares sobre el majestuoso Lago de Atitlán.</p>
            </div>

            <div class="expedition-card">
                <span class="expedition-badge">Cultura & Altura</span>
                <h4>Todos Santos Cuchumatán</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Aventura en la sierra de los Cuchumatanes, Huehuetenango, explorando senderos entre campos fríos y tradiciones vivas.</p>
            </div>

            <div class="expedition-card">
                <span class="expedition-badge">Comunidad & Empoderamiento</span>
                <h4>Mujer en la Cumbre (Cuxliquel)</h4>
                <p style="font-size: 0.88rem; color: #BBB;">Evento enfocado en inspirar y motivar la participación femenina en el senderismo y montañismo nacional.</p>
            </div>
        </div>
    </section>

    <!-- SERVICIOS Y MERCHANDISING SECTION -->
    <section id="servicios">
        <!-- Mascota Oficial -->
        <div class="mascot-box">
            <div class="mascot-icon">🐺</div>
            <div class="mascot-text">
                <h3>Nuestra Mascota: Lobo AURAX</h3>
                <p>El lobo representa la fuerza de la manada, la resistencia en el camino y el espíritu indomable de explorar la cumbre. Caminamos juntos y cuidamos de cada integrante en cada ascenso.</p>
            </div>
        </div>

        <h2 class="section-title">Expediciones, Alquiler y Merch Oficial</h2>
        <div class="products-grid" id="productsGrid"></div>
    </section>

    <!-- ESTRATEGIA Y OBJETIVOS -->
    <section id="estrategia">
        <h2 class="section-title">Pilares Estratégicos</h2>
        
        <div class="card-box">
            <h3>🧭 Misión</h3>
            <p>Brindar experiencias de montañismo, senderismo y ascenso de volcanes que inspiren a las personas a conectar con la naturaleza, superar sus propios límites y crear vínculos a través de la aventura, promoviendo siempre la seguridad, el respeto por el medio ambiente y el compañerismo en cada expedición.</p>
        </div>

        <div class="card-box">
            <h3>🏔️ Visión</h3>
            <p>Ser la comunidad líder de montañismo y aventura en Guatemala, reconocida por ofrecer experiencias auténticas, seguras y memorables, promoviendo una cultura de exploración responsable y convirtiéndose en un referente para quienes buscan descubrir nuevas cimas y vivir la montaña con pasión.</p>
        </div>

        <div class="card-box">
            <h3>🎯 Objetivo General</h3>
            <p>Consolidar a Aurax Montañismo GT como una comunidad líder en montañismo y senderismo, ofreciendo experiencias seguras, memorables y responsables que fortalezcan la conexión entre las personas y la naturaleza.</p>

            <h4 style="color: #5CE1E6; margin-top: 25px; margin-bottom: 10px;">Objetivos Específicos:</h4>
            <div class="obj-list">
                <div class="obj-item">1. Organizar expediciones con altos estándares de seguridad y planificación.</div>
                <div class="obj-item">2. Fomentar el respeto por el medio ambiente y el turismo responsable.</div>
                <div class="obj-item">3. Promover el compañerismo y la convivencia en la comunidad.</div>
                <div class="obj-item">4. Desarrollar una marca reconocida por su calidad y profesionalismo en Guatemala.</div>
            </div>
        </div>
    </section>

    <!-- CONTACTO Y REDES SOCIALES -->
    <section id="contacto">
        <h2 class="section-title">Contacto Directo & Redes</h2>
        <div style="text-align: center;">
            <p style="font-size: 1.2rem; margin-bottom: 20px;">¿Dudas sobre próximos viajes, alquiler de equipo o nuestro merch oficial? ¡Escríbenos!</p>
            
            <a href="https://wa.me/50254342015?text=Hola%20AuraX%20Monta%C3%B1ismo!" target="_blank" class="btn btn-ws" style="font-size: 1.1rem; padding: 15px 30px;">
                💬 Contactar por WhatsApp (5434-2015)
            </a>

            <div class="social-links">
                <a href="https://www.instagram.com/aurax_gt" target="_blank" class="btn btn-social">
                    📸 Instagram @aurax_gt
                </a>
                <a href="https://www.tiktok.com/@aurax546" target="_blank" class="btn btn-social">
                    🎵 TikTok @aurax546
                </a>
            </div>

            <p style="margin-top: 25px; color: #777777; font-size: 0.9rem;">Operamos de manera digital con entregas coordinadas y puntos de encuentro para las expediciones.</p>
        </div>
    </section>

    <!-- CARRITO SIDEBAR -->
    <div class="cart-sidebar" id="cartSidebar">
        <h3 style="color: #5CE1E6; margin-bottom: 10px;">🛒 Tu Reserva / Pedido</h3>
        <p style="font-size: 0.85rem; color: #AAA;">Revisa tus expediciones, alquileres o souvenirs seleccionados:</p>
        
        <div class="cart-items-container" id="cartItems"></div>
        
        <div style="margin-top: 20px; border-top: 1px solid #333; padding-top: 15px;">
            <h4 style="margin-bottom: 15px; font-size: 1.2rem;">Total Estimado: Q<span id="cartTotal">0.00</span></h4>
            <button class="btn btn-ws" style="width: 100%; font-size: 1rem; margin: 0 0 10px 0;" onclick="checkoutWhatsApp()">
                Confirmar por WhatsApp
            </button>
            <button class="btn" style="width: 100%; background-color: #FF4D4D; color: #FFF; margin: 0;" onclick="toggleCart()">
                Cerrar
            </button>
        </div>
    </div>

    <footer>
        <p>&copy; 2026 AURAX MONTAÑISMO GT | Conquistando a Guate desde lo alto.</p>
    </footer>

    <script>
        const services = [
            // Expediciones & Servicios
            { id: 1, name: "Próxima Expedición a Volcán", price: 250.00, emoji: "🏔️", desc: "Incluye guía, logística y fotografía digital." },
            { id: 2, name: "Servicio de Guía Privado", price: 400.00, emoji: "🧭", desc: "Ruta personalizada para grupos o familias." },
            { id: 3, name: "Alquiler de Carpa 2/4 Personas", price: 75.00, emoji: "⛺", desc: "Resistente y lista para la intemperie." },
            { id: 4, name: "Alquiler de Sleeping Bag (-5°C)", price: 50.00, emoji: "🛌", desc: "Alta resistencia térmica." },
            
            // Merchandising Oficial AURAX
            { id: 5, name: "Gorra Oficial AURAX GT", price: 85.00, emoji: "🧢", desc: "Diseño exclusivo de montaña con el lobo oficial." },
            { id: 6, name: "Pachón Térmico AURAX", price: 95.00, emoji: "🥤", desc: "Mantiene tus bebidas frías o calientes en el ascenso." },
            { id: 7, name: "Llavero Conmemorativo AURAX", price: 35.00, emoji: "🔑", desc: "El detalle perfecto para llevar la pasión a todos lados." },
            { id: 8, name: "Combo Explorer (Gorra + Pachón + Llavero)", price: 195.00, emoji: "🎒", desc: "Ahorra llevando el paquete completo de la marca." }
        ];

        let cart = [];

        function renderServices() {
            const grid = document.getElementById('productsGrid');
            grid.innerHTML = '';
            services.forEach(s => {
                grid.innerHTML += `
                    <div class="product-card">
                        <div>
                            <div class="product-icon">${s.emoji}</div>
                            <div class="product-title">${s.name}</div>
                            <p style="font-size:0.85rem; color:#AAA; margin-bottom:12px;">${s.desc}</p>
                        </div>
                        <div>
                            <div class="product-price">Q${s.price.toFixed(2)}</div>
                            <button class="btn" onclick="addToCart(${s.id})">+ Agregar al Pedido</button>
                        </div>
                    </div>
                `;
            });
        }

        function addToCart(id) {
            const item = services.find(s => s.id === id);
            cart.push(item);
            updateCart();
            toggleCart(true);
        }

        function removeFromCart(index) {
            cart.splice(index, 1);
            updateCart();
        }

        function updateCart() {
            document.getElementById('cartCount').innerText = cart.length;
            const container = document.getElementById('cartItems');
            let total = 0;
            container.innerHTML = '';
            
            if (cart.length === 0) {
                container.innerHTML = '<p style="color:#888; margin-top:20px; text-align:center;">No has seleccionado ninguna expedición o artículo.</p>';
            } else {
                cart.forEach((item, index) => {
                    total += item.price;
                    container.innerHTML += `
                        <div class="cart-item">
                            <div class="cart-item-details">
                                <span><b>${item.emoji} ${item.name}</b></span>
                                <span style="color:#5CE1E6;">Q${item.price.toFixed(2)}</span>
                            </div>
                            <button class="remove-btn" onclick="removeFromCart(${index})" title="Eliminar">✕</button>
                        </div>
                    `;
                });
            }
            document.getElementById('cartTotal').innerText = total.toFixed(2);
        }

        function toggleCart(forceOpen = false) {
            const sidebar = document.getElementById('cartSidebar');
            if (forceOpen || !sidebar.classList.contains('active')) {
                sidebar.classList.add('active');
            } else {
                sidebar.classList.remove('active');
            }
        }

        function checkoutWhatsApp() {
            if (cart.length === 0) return alert("Agrega al menos una expedición, servicio o artículo.");
            let msg = "Hola AuraX Montañismo, quiero hacer el siguiente pedido/reserva:%0A%0A";
            let total = 0;
            cart.forEach(item => {
                msg += `• ${item.name} (Q${item.price.toFixed(2)})%0A`;
                total += item.price;
            });
            msg += `%0ATotal estimado: Q${total.toFixed(2)}%0A%0A¿Me confirman disponibilidad y pasos para la entrega o reserva?`;
            window.open(`https://wa.me/50254342015?text=${msg}`, '_blank');
        }

        renderServices();
    </script>
</body>
</html>

