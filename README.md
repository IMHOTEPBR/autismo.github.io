# autismo.github.io
inclusão utilitária para Autistas
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Colaboragens - Blog sobre Autismo</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --color-primary: #B5EAD7;
            --color-secondary: #FFDAC1;
            --color-accent: #C7CEEA;
            --color-text: #4A4A4A;
            --color-background: #FFFFFF;
            --color-light: #F9F9F9;
            --color-border: #E2E2E2;
            --font-main: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            --border-radius: 12px;
            --box-shadow: 0 8px 20px rgba(0, 0, 0, 0.08);
        }
        
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: var(--font-main);
            color: var(--color-text);
            background-color: var(--color-light);
            line-height: 1.6;
            padding-bottom: 60px;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        /* Header */
        header {
            background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-accent) 100%);
            padding: 30px 0;
            text-align: center;
            border-radius: 0 0 var(--border-radius) var(--border-radius);
            margin-bottom: 30px;
            box-shadow: var(--box-shadow);
        }
        
        .logo {
            font-size: 2.5rem;
            font-weight: bold;
            color: var(--color-text);
            margin-bottom: 15px;
            display: block;
        }
        
        .tagline {
            font-size: 1.2rem;
            color: var(--color-text);
            opacity: 0.9;
        }
        
        /* Navigation */
        nav {
            background-color: var(--color-background);
            border-radius: var(--border-radius);
            padding: 15px;
            margin: 20px auto;
            max-width: 800px;
            box-shadow: var(--box-shadow);
        }
        
        nav ul {
            display: flex;
            justify-content: center;
            list-style: none;
            flex-wrap: wrap;
        }
        
        nav ul li {
            margin: 5px 15px;
        }
        
        nav ul li a {
            text-decoration: none;
            color: var(--color-text);
            font-weight: 500;
            transition: color 0.3s;
            display: flex;
            align-items: center;
        }
        
        nav ul li a i {
            margin-right: 8px;
        }
        
        nav ul li a:hover {
            color: var(--color-accent);
        }
        
        /* Main Content Sections */
        .section {
            background: var(--color-background);
            border-radius: var(--border-radius);
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--box-shadow);
        }
        
        .section h2 {
            color: var(--color-text);
            margin-bottom: 20px;
            padding-bottom: 10px;
            border-bottom: 2px solid var(--color-primary);
            display: flex;
            align-items: center;
        }
        
        .section h2 i {
            margin-right: 10px;
        }
        
        /* About Section */
        .about-content {
            display: grid;
            grid-template-columns: 1fr 2fr;
            gap: 30px;
            align-items: center;
        }
        
        .profile-img {
            width: 100%;
            border-radius: 50%;
            background-color: var(--color-secondary);
            aspect-ratio: 1/1;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 5rem;
            color: var(--color-text);
        }
        
        /* Interests Section */
        .interests {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }
        
        .interest-card {
            background: var(--color-light);
            padding: 20px;
            border-radius: var(--border-radius);
            text-align: center;
        }
        
        .interest-card i {
            font-size: 2rem;
            color: var(--color-accent);
            margin-bottom: 15px;
        }
        
        /* E-commerce Section */
        .products {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 25px;
            margin-bottom: 30px;
        }
        
        .product-card {
            background: var(--color-light);
            border-radius: var(--border-radius);
            overflow: hidden;
            transition: transform 0.3s;
        }
        
        .product-card:hover {
            transform: translateY(-5px);
        }
        
        .product-image {
            height: 180px;
            background-color: var(--color-secondary);
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 3rem;
            color: var(--color-text);
        }
        
        .product-info {
            padding: 15px;
        }
        
        .product-title {
            font-size: 1.1rem;
            margin-bottom: 10px;
        }
        
        .product-price {
            font-weight: bold;
            color: var(--color-accent);
            margin-bottom: 15px;
        }
        
        .buy-btn {
            display: block;
            width: 100%;
            padding: 10px;
            background: var(--color-accent);
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 500;
            transition: background 0.3s;
        }
        
        .buy-btn:hover {
            background: #A5B6E8;
        }
        
        /* Shipping Calculator */
        .shipping-calculator {
            background: var(--color-light);
            padding: 20px;
            border-radius: var(--border-radius);
            margin-top: 20px;
        }
        
        .shipping-calculator h3 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
        }
        
        .shipping-calculator h3 i {
            margin-right: 10px;
        }
        
        .form-group {
            margin-bottom: 15px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
        }
        
        .form-group input {
            width: 100%;
            padding: 12px;
            border: 1px solid var(--color-border);
            border-radius: 5px;
            font-family: var(--font-main);
        }
        
        .calculate-btn {
            padding: 12px 25px;
            background: var(--color-primary);
            color: var(--color-text);
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-weight: 500;
            transition: background 0.3s;
            display: flex;
            align-items: center;
        }
        
        .calculate-btn i {
            margin-right: 8px;
        }
        
        .calculate-btn:hover {
            background: #A5D9C5;
        }
        
        .shipping-result {
            margin-top: 15px;
            padding: 15px;
            background: var(--color-background);
            border-radius: 5px;
            display: none;
        }
        
        /* Donation Section */
        .donation-options {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }
        
        .pix-donation, .qrcode-donation {
            background: var(--color-light);
            padding: 25px;
            border-radius: var(--border-radius);
            text-align: center;
        }
        
        .pix-donation h3, .qrcode-donation h3 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .pix-donation h3 i, .qrcode-donation h3 i {
            margin-right: 10px;
        }
        
        .pix-key {
            background: var(--color-background);
            padding: 15px;
            border-radius: 5px;
            margin: 15px 0;
            font-weight: 500;
            word-break: break-all;
            font-size: 1.1rem;
        }
        
        .copy-btn {
            padding: 12px 20px;
            background: var(--color-primary);
            border: none;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
            transition: background 0.3s;
            display: inline-flex;
            align-items: center;
        }
        
        .copy-btn i {
            margin-right: 8px;
        }
        
        .copy-btn:hover {
            background: #A5D9C5;
        }
        
        .qrcode-image {
            width: 200px;
            height: 200px;
            margin: 0 auto;
            background-color: #f5f5f5;
            display: flex;
            align-items: center;
            justify-content: center;
            border-radius: 5px;
            font-size: 0.9rem;
            color: #666;
            text-align: center;
            padding: 10px;
        }
        
        /* Favorites Section */
        .favorites {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 25px;
        }
        
        .favorite-category {
            background: var(--color-light);
            padding: 20px;
            border-radius: var(--border-radius);
        }
        
        .favorite-category h3 {
            margin-bottom: 15px;
            color: var(--color-accent);
            display: flex;
            align-items: center;
        }
        
        .favorite-category h3 i {
            margin-right: 10px;
        }
        
        .favorite-list {
            list-style: none;
        }
        
        .favorite-list li {
            padding: 8px 0;
            border-bottom: 1px solid var(--color-border);
        }
        
        .favorite-list li:last-child {
            border-bottom: none;
        }
        
        /* Footer */
        footer {
            background: linear-gradient(135deg, var(--color-primary) 0%, var(--color-accent) 100%);
            color: var(--color-text);
            padding: 30px 0;
            text-align: center;
            border-radius: var(--border-radius) var(--border-radius) 0 0;
            margin-top: 40px;
            box-shadow: var(--box-shadow);
        }
        
        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin: 20px 0;
        }
        
        .social-links a {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 50px;
            height: 50px;
            background: var(--color-background);
            border-radius: 50%;
            color: var(--color-text);
            font-size: 1.5rem;
            transition: transform 0.3s;
        }
        
        .social-links a:hover {
            transform: translateY(-5px);
        }
        
        .copyright {
            margin-top: 20px;
            font-size: 0.9rem;
        }
        
        /* Responsive */
        @media (max-width: 900px) {
            .about-content {
                grid-template-columns: 1fr;
                text-align: center;
            }
            
            .profile-img {
                max-width: 250px;
                margin: 0 auto;
            }
        }
        
        @media (max-width: 600px) {
            .logo {
                font-size: 2rem;
            }
            
            .tagline {
                font-size: 1rem;
            }
            
            nav ul {
                flex-direction: column;
                align-items: center;
            }
            
            nav ul li {
                margin: 10px 0;
            }
            
            .section {
                padding: 20px;
            }
            
            .donation-options {
                grid-template-columns: 1fr;
            }
        }

        /* Tutorial Section */
        .tutorial-section {
            background: var(--color-background);
            border-radius: var(--border-radius);
            padding: 30px;
            margin-bottom: 30px;
            box-shadow: var(--box-shadow);
        }
        
        .tutorial-step {
            margin-bottom: 25px;
            padding-bottom: 25px;
            border-bottom: 1px solid var(--color-border);
        }
        
        .tutorial-step:last-child {
            border-bottom: none;
            margin-bottom: 0;
            padding-bottom: 0;
        }
        
        .step-number {
            display: inline-block;
            width: 30px;
            height: 30px;
            background: var(--color-accent);
            color: white;
            border-radius: 50%;
            text-align: center;
            line-height: 30px;
            margin-right: 10px;
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <span class="logo">Colaboragens</span>
            <p class="tagline">Blog sobre Autismo e Inclusão</p>
        </div>
    </header>

    <div class="container">
        <nav>
            <ul>
                <li><a href="#about"><i class="fas fa-user"></i> Sobre Mim</a></li>
                <li><a href="#store"><i class="fas fa-store"></i> Loja Virtual</a></li>
                <li><a href="#donations"><i class="fas fa-donate"></i> Doações</a></li>
                <li><a href="#favorites"><i class="fas fa-star"></i> Favoritos</a></li>
                <li><a href="#tutorial"><i class="fas fa-graduation-cap"></i> Como Usar</a></li>
                <li><a href="#contact"><i class="fas fa-envelope"></i> Contato</a></li>
            </ul>
        </nav>

        <section id="about" class="section">
            <h2><i class="fas fa-user"></i> Sobre Mim</h2>
            <div class="about-content">
                <div class="profile-img">
                    <i class="fas fa-user"></i>
                </div>
                <div>
                    <p>"Fui diagnosticado com autismo e vejo o mundo de uma forma única – o que me ajuda a inovar em cada projeto." Olá! Sou Elizeu Souza, um criador autista multifacetado que transforma paixões em projetos concretos.</p>
                    <p>Como artesão de biojoias, dou vida a acessórios sustentáveis, unindo arte e natureza em peças únicas. Na música, encontro minha voz – seja compondo, tocando ou explorando sons que contam histórias.</p>
                    <p>Na tecnologia, trabalho como programador e analista técnico para projetos, desenvolvendo soluções digitais para causas sociais. Trabalho com ONGs como captador de recursos, ajudando a transformar ideias em impacto real.</p>
                    <p>Meu objetivo é usar a creatividade e a lógica para construir pontes entre pessoas, arte e tecnologia.</p>
                    
                    <h3 style="margin-top: 20px;">Interesses</h3>
                    <div class="interests">
                        <div class="interest-card">
                            <i class="fas fa-film"></i>
                            <h4>Edição Criativa e Audiovisual</h4>
                        </div>
                        <div class="interest-card">
                            <i class="fas fa-laptop"></i>
                            <h4>Freelancer e Dinheiro Online</h4>
                        </div>
                        <div class="interest-card">
                            <i class="fas fa-code"></i>
                            <h4>Tecnologia para Criadores</h4>
                        </div>
                        <div class="interest-card">
                            <i class="fas fa-music"></i>
                            <h4>Entretenimento Inteligente</h4>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <section id="store" class="section">
            <h2><i class="fas fa-store"></i> Loja Virtual</h2>
            <p>Confira meus produtos artesanais, e-books e softwares desenvolvidos para a comunidade autista.</p>
            
            <div class="products">
                <!-- Produto 1 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-book"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">E-book: Guia do Autismo</h3>
                        <p class="product-price">R$ 29,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>
                
                <!-- Produto 2 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-laptop-code"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Software Educacional</h3>
                        <p class="product-price">R$ 49,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>
                
                <!-- Produto 3 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-gem"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Biojoia Artesanal</h3>
                        <p class="product-price">R$ 39,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>
                
                <!-- Produto 4 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-puzzle-piece"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Kit de Artesanato</h3>
                        <p class="product-price">R$ 59,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>

                <!-- Produto 5 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-headphones"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Música Terapêutica</h3>
                        <p class="product-price">R$ 19,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>

                <!-- Produto 6 -->
                <div class="product-card">
                    <div class="product-image">
                        <i class="fas fa-palette"></i>
                    </div>
                    <div class="product-info">
                        <h3 class="product-title">Kit de Pintura</h3>
                        <p class="product-price">R$ 69,90</p>
                        <button class="buy-btn">Comprar</button>
                    </div>
                </div>
            </div>
            
            <div class="shipping-calculator">
                <h3><i class="fas fa-truck"></i> Calculadora de Frete</h3>
                <p>Dimensões padrão da embalagem: 24 x 16 x 8 cm | Preço da caixa: R$7,10</p>
                <div class="form-group">
                    <label for="cep">CEP de Destino:</label>
                    <input type="text" id="cep" placeholder="Digite o CEP (apenas números)" maxlength="8">
                </div>
                <button class="calculate-btn" onclick="calculateShipping()"><i class="fas fa-calculator"></i> Calcular Frete</button>
                
                <div class="shipping-result" id="shipping-result">
                    <h4>Opções de Frete:</h4>
                    <p>PAC: R$ <span id="pac-price">-</span> (Prazo: <span id="pac-deadline">-</span> dias)</p>
                    <p>SEDEX: R$ <span id="sedex-price">-</span> (Prazo: <span id="sedex-deadline">-</span> dias)</p>
                </div>
            </div>
        </section>

        <section id="donations" class="section">
            <h2><i class="fas fa-donate"></i> Apoie o Colaboragens</h2>
            <p>Seu apoio ajuda a manter este blog e a criar mais conteúdo sobre autismo.</p>
            
            <div class="donation-options">
                <div class="pix-donation">
                    <h3><i class="fas fa-money-bill-wave"></i> Doação via PIX</h3>
                    <p>Chave PIX (e-mail):</p>
                    <div class="pix-key">elizeu.souza@msn.com</div>
                    <button class="copy-btn" onclick="copyPixKey()"><i class="fas fa-copy"></i> Copiar Chave</button>
                </div>
                
                <div class="qrcode-donation">
                    <h3><i class="fas fa-qrcode"></i> QR Code para Pagamento</h3>
                    <div class="qrcode-image">
                        <!-- Aqui viria o QR code real -->
                        <div>
                            <i class="fas fa-qrcode" style="font-size: 40px; margin-bottom: 10px;"></i>
                            <p>Use o app do seu banco para escanear</p>
                        </div>
                    </div>
                    <p style="margin-top: 15px;">Escaneie com seu app de banco</p>
                </div>
            </div>
        </section>

        <section id="favorites" class="section">
            <h2><i class="fas fa-star"></i> Meus Favoritos</h2>
            
            <div class="favorites">
                <div class="favorite-category">
                    <h3><i class="fas fa-film"></i> Filmes Favoritos</h3>
                    <ul class="favorite-list">
                        <li>2001: A Space Odyssey</li>
                        <li>Blade Runner</li>
                        <li>Contact</li>
                        <li>The Thing</li>
                        <li>District 9</li>
                        <li>Arrival</li>
                        <li>Alien</li>
                        <li>Predator</li>
                        <li>Interstellar</li>
                        <li>Star Trek</li>
                    </ul>
                </div>
                
                <div class="favorite-category">
                    <h3><i class="fas fa-music"></i> Música Favorita</h3>
                    <ul class="favorite-list">
                        <li>Rock progressivo psicodélico dos anos 70</li>
                        <li>NWOBHM</li>
                        <li>Euro Dance</li>
                        <li>Música New Age</li>
                        <li>Música de Cura Binaural</li>
                        <li>Música Ambissônica</li>
                    </ul>
                </div>
                
                <div class="favorite-category">
                    <h3><i class="fas fa-book"></i> Livros Favoritos</h3>
                    <ul class="favorite-list">
                        <li>Coptic Bible</li>
                        <li>Gnostic Bible</li>
                        <li>Operating system books</li>
                        <li>Public notices for raising non-refundable funds for non-profit organizations</li>
                    </ul>
                </div>
            </div>
        </section>

        <section id="tutorial" class="tutorial-section">
            <h2><i class="fas fa-graduation-cap"></i> Como Criar seu Site no GitHub</h2>
            
            <div class="tutorial-step">
                <h3><span class="step-number">1</span> Criar um novo repositório</h3>
                <p>Faça login na sua conta GitHub, clique no ícone "+" no canto superior direito e selecione "New repository".</p>
                <p>Nomeie o repositório como <strong>seuusuario.github.io</strong> (substitua "seuusuario" pelo seu nome de usuário).</p>
            </div>
            
            <div class="tutorial-step">
                <h3><span class="step-number">2</span> Fazer upload dos arquivos</h3>
                <p>No repositório recém-criado, clique em "Add file" > "Upload files".</p>
                <p>Arraste este arquivo HTML ou clique em "choose your files" para selecioná-lo.</p>
            </div>
            
            <div class="tutorial-step">
                <h3><span class="step-number">3</span> Configurar o GitHub Pages</h3>
                <p>No repositório, clique na aba "Settings".</p>
                <p>No menu lateral esquerdo, clique em "Pages".</p>
                <p>Em "Source", selecione a branch "main" e a pasta "/ (root)".</p>
                <p>Clique em "Save".</p>
            </div>
            
            <div class="tutorial-step">
                <h3><span class="step-number">4</span> Acessar seu site</h3>
                <p>Seu site estará disponível em <strong>https://seuusuario.github.io</strong> em alguns minutos.</p>
                <p>Pronto! Seu site está no ar e pode ser compartilhado com todos.</p>
            </div>
        </section>

        <section id="contact" class="section">
            <h2><i class="fas fa-envelope"></i> Contato</h2>
            <p>Entre em contato comigo para colaborações, dúvidas ou sugestões.</p>
            <p><strong>Email:</strong> elizeu.souza@msn.com</p>
            <p><strong>Localização:</strong> Iranduba, AMAZONAS, Brasil</p>
            <p><strong>Setor:</strong> Comunicações ou mídia</p>
            <p><strong>Profissão:</strong> Technical analyst</p>
        </section>
    </div>

    <footer>
        <div class="container">
            <div class="social-links">
                <a href="#"><i class="fab fa-facebook-f"></i></a>
                <a href="#"><i class="fab fa-instagram"></i></a>
                <a href="#"><i class="fab fa-twitter"></i></a>
                <a href="#"><i class="fab fa-youtube"></i></a>
                <a href="#"><i class="fab fa-github"></i></a>
            </div>
            <p class="copyright">© 2023 Colaboragens - Blog sobre Autismo. Todos os direitos reservados.</p>
        </div>
    </footer>

    <script>
        // Função para copiar a chave PIX
        function copyPixKey() {
            const pixKey = "elizeu.souza@msn.com";
            navigator.clipboard.writeText(pixKey)
                .then(() => {
                    alert("Chave PIX copiada: " + pixKey);
                })
                .catch(err => {
                    console.error('Falha ao copiar: ', err);
                    // Fallback para dispositivos sem suporte a clipboard
                    const tempTextArea = document.createElement("textarea");
                    tempTextArea.value = pixKey;
                    document.body.appendChild(tempTextArea);
                    tempTextArea.select();
                    document.execCommand("copy");
                    document.body.removeChild(tempTextArea);
                    alert("Chave PIX copiada: " + pixKey);
                });
        }
        
        // Função para calcular o frete (simulação)
        function calculateShipping() {
            const cep = document.getElementById('cep').value;
            
            if (!cep || cep.length !== 8 || isNaN(cep)) {
                alert("Por favor, digite um CEP válido com 8 dígitos.");
                return;
            }
            
            // Simulação de cálculo de frete
            // Valores baseados nas dimensões fornecidas: 24x16x8 cm
            const basePacPrice = 15.50;
            const baseSedexPrice = 22.90;
            const boxPrice = 7.10;
            
            // Simula variação de preço por região (apenas para demonstração)
            const regionFactor = parseInt(cep.charAt(0)) * 0.1 + 1;
            
            const pacPrice = (basePacPrice * regionFactor + boxPrice).toFixed(2);
            const sedexPrice = (baseSedexPrice * regionFactor + boxPrice).toFixed(2);
            
            // Simula variação de prazo por região
            const pacDeadline = (7 + parseInt(cep.charAt(1))).toString();
            const sedexDeadline = (3 + parseInt(cep.charAt(1))).toString();
            
            document.getElementById('pac-price').textContent = pacPrice;
            document.getElementById('sedex-price').textContent = sedexPrice;
            document.getElementById('pac-deadline').textContent = pacDeadline;
            document.getElementById('sedex-deadline').textContent = sedexDeadline;
            
            document.getElementById('shipping-result').style.display = 'block';
        }
        
        // Validação do CEP para aceitar apenas números
        document.getElementById('cep').addEventListener('input', function() {
            this.value = this.value.replace(/\D/g, '');
        });
        
        // Smooth scroll para links de navegação
        document.querySelectorAll('nav a').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 20,
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
