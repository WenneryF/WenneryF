<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=5.0">
    <meta name="description" content="Py Tech - Soluções Tecnológicas em Porto Alegre. Manutenção preventiva, suporte técnico, consultoria e web design profissional para sua empresa.">
    <meta name="keywords" content="Py Tech, tecnologia, manutenção computadores, suporte técnico, web design, Porto Alegre, consultoria TI">
    <meta name="author" content="Py Tech">
    
    <!-- Open Graph / Facebook -->
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://pytech-solucoes.netlify.app/">
    <meta property="og:title" content="PY TECH - Soluções Tecnológicas em Porto Alegre">
    <meta property="og:description" content="Soluções tecnológicas completas: manutenção, suporte, consultoria e web design profissional.">
    <meta property="og:image" content="https://pytech-solucoes.netlify.app/images/og-image.jpg">
    
    <!-- Twitter -->
    <meta property="twitter:card" content="summary_large_image">
    <meta property="twitter:url" content="https://pytech-solucoes.netlify.app/">
    <meta property="twitter:title" content="PY TECH - Soluções Tecnológicas em Porto Alegre">
    <meta property="twitter:description" content="Soluções tecnológicas completas: manutenção, suporte, consultoria e web design profissional.">
    <meta property="twitter:image" content="https://pytech-solucoes.netlify.app/images/og-image.jpg">
    
    <title>PY TECH - Soluções Tecnológicas</title>
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Favicon -->
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22 fill=%22%2300FFFF%22>&lt;/&gt;</text></svg>">
    
    <!-- Fonts -->
    <style>
        @font-face {
            font-family: 'Montserrat';
            font-style: normal;
            font-weight: 400;
            src: local('Montserrat Regular'), local('Montserrat-Regular'), url('/fonts/montserrat-v15-latin-regular.woff2') format('woff2');
        }
        @font-face {
            font-family: 'Montserrat';
            font-style: normal;
            font-weight: 700;
            src: local('Montserrat Bold'), local('Montserrat-Bold'), url('/fonts/montserrat-v15-latin-700.woff2') format('woff2');
        }
        @font-face {
            font-family: 'Orbitron';
            font-style: normal;
            font-weight: 800;
            src: local('Orbitron ExtraBold'), local('Orbitron-ExtraBold'), url('/fonts/orbitron-v16-latin-800.woff2') format('woff2');
        }
    </style>
    
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #0A0A0A;
            color: white;
            overflow-x: hidden;
            position: relative;
        }
        
        .logo {
            font-family: 'Orbitron', sans-serif;
            background: linear-gradient(90deg, #00FFFF, #0088FF);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            transition: all 0.3s ease;
        }
        
        .logo:hover {
            filter: brightness(1.2);
        }
        
        .matrix-code {
            position: absolute;
            color: rgba(0, 255, 0, 0.2);
            font-family: monospace;
            z-index: 0;
            user-select: none;
        }
        
        .typing-text {
            font-family: 'Orbitron', sans-serif;
            font-weight: 800;
            border-right: 3px solid #00FFFF;
            white-space: nowrap;
            overflow: hidden;
            animation: typing 3s steps(40) 1s 1 normal both, blink-caret 0.75s step-end infinite;
        }
        
        @keyframes typing {
            from { width: 0 }
            to { width: 100% }
        }
        
        @keyframes blink-caret {
            from, to { border-color: transparent }
            50% { border-color: #00FFFF }
        }
        
        .slogan {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            color: #00FFFF;
            text-shadow: 0 0 5px rgba(0, 255, 255, 0.5);
        }
        
        .card {
            border: 1px solid #00FFFF;
            transition: all 0.3s ease;
        }
        
        .card:hover {
            transform: translateY(-5px);
            box-shadow: 0 0 15px #00FFFF;
            border-width: 3px;
        }
        
        .whatsapp-float {
            position: fixed;
            bottom: 20px;
            left: 20px;
            background-color: #25D366;
            color: white;
            border-radius: 50px;
            text-align: center;
            font-size: 30px;
            box-shadow: 0 0 15px rgba(37, 211, 102, 0.5);
            z-index: 100;
            display: flex;
            align-items: center;
            padding: 12px 20px;
            transition: all 0.3s ease;
            text-decoration: none;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0.7); }
            70% { box-shadow: 0 0 0 15px rgba(37, 211, 102, 0); }
            100% { box-shadow: 0 0 0 0 rgba(37, 211, 102, 0); }
        }
        
        .whatsapp-float:hover {
            background-color: #128C7E;
            transform: scale(1.05);
            animation: none;
        }
        
        .whatsapp-float span {
            font-size: 16px;
            margin-left: 10px;
            display: inline-block;
        }
        
        .loader {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: #0A0A0A;
            display: flex;
            justify-content: center;
            align-items: center;
            z-index: 9999;
        }
        
        .loader-spinner {
            width: 50px;
            height: 50px;
            border: 5px solid rgba(0, 255, 255, 0.3);
            border-radius: 50%;
            border-top-color: #00FFFF;
            animation: spin 1s ease-in-out infinite;
        }
        
        @keyframes spin {
            to { transform: rotate(360deg); }
        }
        
        .matrix-rain-container {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            overflow: hidden;
            z-index: -1;
        }
        
        .matrix-rain {
            position: absolute;
            color: #00FF00;
            font-family: monospace;
            font-size: 16px;
            text-align: center;
            opacity: 0.2;
            user-select: none;
        }
        
        .service-list {
            list-style-type: none;
            padding-left: 0;
            margin-top: 10px;
        }
        
        .service-list li {
            position: relative;
            padding-left: 20px;
            margin-bottom: 5px;
            color: #e0e0e0;
        }
        
        .service-list li:before {
            content: '>';
            position: absolute;
            left: 0;
            color: #00FFFF;
            font-weight: bold;
        }
        
        .about-text {
            max-width: 800px;
            margin: 0 auto;
            text-align: center;
            line-height: 1.8;
        }
        
        .about-text p {
            margin-bottom: 1.5rem;
        }
        
        .highlight {
            color: #00FFFF;
            font-weight: bold;
        }
        
        /* Form validation styles */
        .form-input.error {
            border-color: #ff3860;
        }
        
        .form-input.success {
            border-color: #00FFFF;
        }
        
        .error-message {
            color: #ff3860;
            font-size: 12px;
            margin-top: 5px;
            display: none;
        }
        
        /* Confirmation message */
        .confirmation-message {
            display: none;
            background-color: rgba(0, 255, 255, 0.1);
            border: 1px solid #00FFFF;
            padding: 15px;
            border-radius: 8px;
            margin-top: 20px;
            text-align: center;
        }
        
        /* Mobile optimizations */
        @media (max-width: 640px) {
            .typing-text {
                font-size: 1.5rem;
                white-space: normal;
                animation: none;
                border-right: none;
            }
            
            .card {
                margin-bottom: 1rem;
            }
            
            .whatsapp-float {
                bottom: 15px;
                left: 15px;
                font-size: 24px;
                padding: 10px 15px;
            }
            
            .whatsapp-float span {
                font-size: 14px;
            }
            
            section {
                padding: 40px 20px;
            }
            
            .hero-section {
                min-height: 80vh;
                padding-top: 80px;
            }
        }
        
        @media (max-width: 360px) {
            .typing-text {
                font-size: 1.3rem;
            }
            
            h2 {
                font-size: 1.5rem;
            }
            
            .whatsapp-float {
                font-size: 20px;
                padding: 8px 12px;
            }
            
            .whatsapp-float span {
                font-size: 12px;
            }
        }
        
        @media (min-width: 1440px) {
            .max-w-6xl {
                max-width: 1280px;
            }
        }
    </style>
</head>
<body>
    <!-- Loader -->
    <div class="loader" id="loader">
        <div class="loader-spinner"></div>
    </div>
    
    <!-- Matrix Code Rain Background -->
    <div id="matrix-container"></div>
    
    <!-- Navigation -->
    <nav class="relative z-10 py-4 px-6 md:px-12 flex justify-center items-center">
        <div class="text-2xl md:text-3xl font-bold">
            <span class="logo">&lt;/&gt; PY TECH</span>
        </div>
    </nav>
    
    <!-- Hero Section -->
    <section class="hero-section relative z-10 flex flex-col justify-center items-center px-6 md:px-12 text-center">
        <!-- Matrix Code Rain específico para área de boas-vindas -->
        <div class="matrix-rain-container" id="welcome-matrix-rain"></div>
        
        <div class="max-w-4xl mx-auto">
            <h1 class="typing-text text-3xl md:text-5xl mb-6">OLÁ, SEJA BEM-VINDO.<span style='color:#00FFFF'>PY TECH</span></h1>
            <p class="slogan text-xl md:text-2xl font-bold">Transformando desafios em oportunidades tecnológicas</p>
        </div>
    </section>
    
    <!-- About Section -->
    <section class="relative z-10 py-12 px-6 md:px-12 bg-black bg-opacity-50">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold mb-8 text-center" style="font-family: 'Orbitron', sans-serif;">SOBRE NÓS</h2>
            <div class="about-text">
                <p>A <span class="highlight">Py Tech</span> é uma empresa especializada em soluções tecnológicas, focada em oferecer serviços de alta qualidade para atender às necessidades dos nossos clientes.</p>
                <p>Nossa equipe é composta por profissionais altamente qualificados e apaixonados por tecnologia, prontos para transformar seus desafios em oportunidades.</p>
            </div>
        </div>
    </section>
    
    <!-- Services Preview -->
    <section id="services" class="relative z-10 py-12 px-6 md:px-12">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold mb-8 text-center" style="font-family: 'Orbitron', sans-serif;">NOSSOS SERVIÇOS</h2>
            <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Service Card 1 -->
                <div class="card p-6 rounded-lg bg-black bg-opacity-50">
                    <h3 class="text-xl md:text-2xl font-bold mb-4 text-cyan-500">Manutenção Preventiva</h3>
                    <p class="text-gray-300">Atualização de drivers, diagnóstico via HWMonitor/Speccy para garantir o melhor desempenho do seu equipamento.</p>
                </div>
                
                <!-- Service Card 2 -->
                <div class="card p-6 rounded-lg bg-black bg-opacity-50">
                    <h3 class="text-xl md:text-2xl font-bold mb-4 text-cyan-500">Suporte Técnico</h3>
                    <p class="text-gray-300">Formatação, dual boot, otimização de redes/VPN para resolver seus problemas técnicos com eficiência.</p>
                </div>
                
                <!-- Service Card 3 -->
                <div class="card p-6 rounded-lg bg-black bg-opacity-50">
                    <h3 class="text-xl md:text-2xl font-bold mb-4 text-cyan-500">Consultoria Tecnológica</h3>
                    <p class="text-gray-300">Soluções personalizadas para otimizar seus processos e infraestrutura tecnológica.</p>
                </div>
                
                <!-- Service Card 4 - Web Designer -->
                <div class="card p-6 rounded-lg bg-black bg-opacity-50">
                    <h3 class="text-xl md:text-2xl font-bold mb-4 text-cyan-500">Web Designer</h3>
                    <p class="text-gray-300">Criação de sites profissionais e responsivos para sua empresa ou projeto pessoal.</p>
                    <ul class="service-list">
                        <li>Blogs e sites institucionais</li>
                        <li>Páginas de vendas otimizadas</li>
                        <li>Landing pages para captura de leads</li>
                        <li>Lojas virtuais e e-commerce</li>
                        <li>Portfólios e sites pessoais</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="relative z-10 py-12 px-6 md:px-12 bg-black bg-opacity-50">
        <div class="max-w-6xl mx-auto">
            <h2 class="text-3xl md:text-4xl font-bold mb-8 text-center" style="font-family: 'Orbitron', sans-serif;">CONTATO</h2>
            <div class="grid md:grid-cols-2 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 text-cyan-500">Entre em contato conosco</h3>
                    <p class="mb-6">Estamos prontos para ajudar você com suas necessidades tecnológicas. Entre em contato para obter um orçamento ou tirar suas dúvidas.</p>
                    <div class="space-y-4">
                        <p><i class="fas fa-phone mr-2 text-cyan-500"></i> (51) 99533-5104</p>
                        <p><i class="fas fa-map-marker-alt mr-2 text-cyan-500"></i> Porto Alegre, RS</p>
                    </div>
                </div>
                <div>
                    <form id="contact-form" class="space-y-4">
                        <div>
                            <input type="text" id="name" name="nome" placeholder="Seu nome" class="form-input w-full px-4 py-3 bg-transparent border border-gray-700 rounded-lg focus:outline-none focus:border-cyan-500" required>
                            <div class="error-message" id="name-error">Por favor, insira seu nome</div>
                        </div>
                        <div>
                            <input type="email" id="email" name="email" placeholder="Seu e-mail" class="form-input w-full px-4 py-3 bg-transparent border border-gray-700 rounded-lg focus:outline-none focus:border-cyan-500" required>
                            <div class="error-message" id="email-error">Por favor, insira um e-mail válido</div>
                        </div>
                        <div>
                            <textarea id="message" name="mensagem" placeholder="Sua mensagem" rows="4" class="form-input w-full px-4 py-3 bg-transparent border border-gray-700 rounded-lg focus:outline-none focus:border-cyan-500" required></textarea>
                            <div class="error-message" id="message-error">Por favor, insira sua mensagem</div>
                        </div>
                        <input type="hidden" name="_subject" value="Novo contato do site Py Tech">
                        <div>
                            <button type="submit" class="w-full px-8 py-3 bg-cyan-500 text-black font-bold rounded-full hover:bg-cyan-600 transition duration-300">ENVIAR MENSAGEM</button>
                        </div>
                    </form>
                    <div id="confirmation-message" class="confirmation-message">
                        <p>Obrigado por entrar em contato! Sua mensagem foi enviada com sucesso. Retornaremos em breve.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer class="relative z-10 py-8 px-6 md:px-12 border-t border-gray-800">
        <div class="max-w-6xl mx-auto">
            <div class="flex flex-col md:flex-row justify-between items-center">
                <div class="text-2xl font-bold mb-4 md:mb-0">
                    <span class="logo">&lt;/&gt; PY TECH</span>
                </div>
                <div class="flex space-x-6">
                    <a href="#" class="text-gray-400 hover:text-cyan-500 transition duration-300">Termos de Serviço</a>
                    <a href="#" class="text-gray-400 hover:text-cyan-500 transition duration-300">Política de Privacidade</a>
                </div>
            </div>
            <div class="mt-8 text-center text-gray-500 text-sm">
                <p>&copy; 2023 Py Tech - Soluções Tecnológicas. Todos os direitos reservados.</p>
            </div>
        </div>
    </footer>
    
    <!-- WhatsApp Float -->
    <a href="https://wa.me/5551995335104?text=Olá,%20Py%20Tech!%20Gostaria%20de%20um%20orçamento." class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
        <span>Fale Conosco</span>
    </a>
    
    <!-- Icons (loaded locally) -->
    <script>
        // Create icon elements
        document.addEventListener('DOMContentLoaded', function() {
            // Phone icon
            const phoneIcons = document.querySelectorAll('.fa-phone');
            phoneIcons.forEach(icon => {
                icon.outerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16" class="inline mr-2 text-cyan-500"><path d="M11 1a1 1 0 0 1 1 1v12a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1V2a1 1 0 0 1 1-1h6zM5 0a2 2 0 0 0-2 2v12a2 2 0 0 0 2 2h6a2 2 0 0 0 2-2V2a2 2 0 0 0-2-2H5z"/><path d="M8 14a1 1 0 1 0 0-2 1 1 0 0 0 0 2z"/></svg>';
            });
            
            // Map marker icon
            const mapIcons = document.querySelectorAll('.fa-map-marker-alt');
            mapIcons.forEach(icon => {
                icon.outerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="currentColor" viewBox="0 0 16 16" class="inline mr-2 text-cyan-500"><path fill-rule="evenodd" d="M10.5 8a2.5 2.5 0 1 1-5 0 2.5 2.5 0 0 1 5 0z"/><path d="M8 0a6 6 0 0 0-6 6c0 1.955.62 3.903 1.742 5.68a.5.5 0 0 0 .868.43c.87-1.073 1.7-2.269 2.28-3.577C7.17 7.83 7.5 7.5 8 7.5s.83.33.11.933c.58 1.308 1.41 2.504 2.28 3.577a.5.5 0 0 0 .868-.43A11.26 11.26 0 0 0 14 6a6 6 0 0 0-6-6z"/></svg>';
            });
            
            // WhatsApp icon
            const whatsappIcon = document.querySelector('.fa-whatsapp');
            whatsappIcon.outerHTML = '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="currentColor" viewBox="0 0 16 16"><path d="M13.601 2.326A7.854 7.854 0 0 0 7.994 0C3.627 0 .068 3.558.064 7.926c0 1.399.366 2.76 1.057 3.965L0 16l4.204-1.102a7.933 7.933 0 0 0 3.79.965h.004c4.368 0 7.926-3.558 7.93-7.93A7.898 7.898 0 0 0 13.6 2.326zM7.994 14.521a6.573 6.573 0 0 1-3.356-.92l-.24-.144-2.494.654.666-2.433-.156-.251a6.56 6.56 0 0 1-1.007-3.505c0-3.626 2.957-6.584 6.591-6.584a6.56 6.56 0 0 1 4.66 1.931 6.557 6.557 0 0 1 1.928 4.66c-.004 3.639-2.961 6.592-6.592 6.592zm3.615-4.934c-.197-.099-1.17-.578-1.353-.646-.182-.065-.315-.099-.445.099-.133.197-.513.646-.627.775-.114.133-.232.148-.43.05-.197-.1-.836-.308-1.592-.985-.59-.525-.985-1.175-1.103-1.372-.114-.198-.011-.304.088-.403.087-.088.197-.232.296-.346.1-.114.133-.198.198-.33.065-.134.034-.248-.015-.347-.05-.099-.445-1.076-.612-1.47-.16-.389-.323-.335-.445-.34-.114-.007-.247-.007-.38-.007a.729.729 0 0 0-.529.247c-.182.198-.691.677-.691 1.654 0 .977.71 1.916.81 2.049.098.133 1.394 2.132 3.383 2.992.47.205.84.326 1.129.418.475.152.904.129 1.246.08.38-.058 1.171-.48 1.338-.943.164-.464.164-.86.114-.943-.049-.084-.182-.133-.38-.232z"/></svg>';
        });
    </script>
    
    <!-- Main Script -->
    <script>
        // Loader
        window.addEventListener('load', function() {
            setTimeout(function() {
                document.getElementById('loader').style.opacity = '0';
                setTimeout(function() {
                    document.getElementById('loader').style.display = 'none';
                }, 500);
            }, 1500);
        });
        
        // Matrix Code Rain
        function createMatrixCode() {
            const container = document.getElementById('matrix-container');
            const symbols = ['π', '0101', '{}', '[]', '()', '++', '==', '!=', '<=', '>=', '//', '/*', '*/', '0x', '0b'];
            
            // Ajusta a quantidade de símbolos com base no tamanho da tela
            const symbolCount = window.innerWidth < 768 ? 30 : 50;
            
            for (let i = 0; i < symbolCount; i++) {
                const code = document.createElement('div');
                code.className = 'matrix-code';
                code.textContent = symbols[Math.floor(Math.random() * symbols.length)];
                
                // Random position
                const left = Math.random() * 100;
                const top = Math.random() * 100;
                
                code.style.left = `${left}%`;
                code.style.top = `${top}%`;
                
                // Random font size - menor em dispositivos móveis
                const size = window.innerWidth < 768 ? 
                    (6 + Math.random() * 14) : 
                    (8 + Math.random() * 20);
                code.style.fontSize = `${size}px`;
                
                // Random opacity
                const opacity = 0.1 + Math.random() * 0.1;
                code.style.opacity = opacity;
                
                container.appendChild(code);
                
                // Animation
                animateCode(code);
            }
        }
        
        function animateCode(element) {
            let pos = parseFloat(element.style.top);
            const speed = 0.5 + Math.random() * 2;
            
            function frame() {
                if (pos > 100) {
                    pos = -10;
                    element.style.left = `${Math.random() * 100}%`;
                } else {
                    pos += speed;
                    element.style.top = `${pos}%`;
                }
                
                requestAnimationFrame(frame);
            }
            
            requestAnimationFrame(frame);
        }
        
        // Matrix Code Rain específico para área de boas-vindas
        function createWelcomeMatrixRain() {
            const container = document.getElementById('welcome-matrix-rain');
            const symbols = ['π', '0101', '{}', '[]', '()', '++', '==', '!=', '<=', '>=', '//', '/*', '*/', '0x', '0b'];
            
            // Ajusta a quantidade de símbolos com base no tamanho da tela
            const symbolCount = window.innerWidth < 768 ? 50 : 100;
            
            for (let i = 0; i < symbolCount; i++) {
                const code = document.createElement('div');
                code.className = 'matrix-rain';
                code.textContent = symbols[Math.floor(Math.random() * symbols.length)];
                
                // Random position
                const left = Math.random() * 100;
                const top = Math.random() * 100;
                
                code.style.left = `${left}%`;
                code.style.top = `${top}%`;
                
                // Random font size - menor em dispositivos móveis
                const size = window.innerWidth < 768 ? 
                    (8 + Math.random() * 16) : 
                    (12 + Math.random() * 24);
                code.style.fontSize = `${size}px`;
                
                // Random opacity
                const opacity = 0.1 + Math.random() * 0.1;
                code.style.opacity = opacity;
                
                container.appendChild(code);
                
                // Animation
                animateWelcomeCode(code);
            }
        }
        
        function animateWelcomeCode(element) {
            let pos = parseFloat(element.style.top);
            const speed = 0.5 + Math.random() * 2;
            
            function frame() {
                if (pos > 100) {
                    pos = -10;
                    element.style.left = `${Math.random() * 100}%`;
                } else {
                    pos += speed;
                    element.style.top = `${pos}%`;
                }
                
                requestAnimationFrame(frame);
            }
            
            requestAnimationFrame(frame);
        }
        
        // Form validation
        document.getElementById('contact-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Reset errors
            document.querySelectorAll('.error-message').forEach(el => el.style.display = 'none');
            document.querySelectorAll('.form-input').forEach(el => {
                el.classList.remove('error');
                el.classList.remove('success');
            });
            
            // Validate form
            let isValid = true;
            const name = document.getElementById('name');
            const email = document.getElementById('email');
            const message = document.getElementById('message');
            
            if (!name.value.trim()) {
                name.classList.add('error');
                document.getElementById('name-error').style.display = 'block';
                isValid = false;
            }
            
            if (!email.value.trim() || !/^[^\s@]+@[^\s@]+\.[^\s@]+$/.test(email.value)) {
                email.classList.add('error');
                document.getElementById('email-error').style.display = 'block';
                isValid = false;
            }
            
            if (!message.value.trim()) {
                message.classList.add('error');
                document.getElementById('message-error').style.display = 'block';
                isValid = false;
            }
            
            if (isValid) {
                // Submit form via Fetch API
                const formData = new FormData(this);
                
                fetch('https://formsubmit.co/ajax/wennerycreator@gmail.com', {
                    method: 'POST',
                    body: formData
                })
                .then(response => response.json())
                .then(data => {
                    if (data.success === 'true') {
                        // Show success message
                        document.getElementById('confirmation-message').style.display = 'block';
                        this.reset();
                        
                        // Mark fields as valid
                        name.classList.add('success');
                        email.classList.add('success');
                        message.classList.add('success');
                        
                        // Hide confirmation after 5 seconds
                        setTimeout(() => {
                            document.getElementById('confirmation-message').style.display = 'none';
                        }, 5000);
                    }
                })
                .catch(error => {
                    console.error('Error:', error);
                    alert('Ocorreu um erro ao enviar o formulário. Por favor, tente novamente mais tarde.');
                });
            }
        });
        
        // Initialize
        window.onload = function() {
            createMatrixCode();
            createWelcomeMatrixRain();
            
            // Set hero section height
            const heroSection = document.querySelector('.hero-section');
            heroSection.style.minHeight = window.innerHeight < 700 ? '80vh' : '100vh';
            
            // Check responsiveness on resize
            window.addEventListener('resize', function() {
                heroSection.style.minHeight = window.innerHeight < 700 ? '80vh' : '100vh';
            });
        };
    </script>
</body>
</html>