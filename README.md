<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>StairCase - Escadas Pre-moldadas.</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap');
        body {
            font-family: 'Poppins', sans-serif;
            background-color: #000000;
            color: #ffffff;
            min-height: 100vh;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
        }
        .profile-img {
            width: 120px;
            height: 120px;
            border-radius: 50%;
            object-fit: cover;
            border: 4px solid #333333;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s ease;
        }
        .profile-img:hover { transform: scale(1.05); }
        .link-card {
            background: rgba(255, 255, 255, 0.8);
            backdrop-filter: blur(10px);
            border-radius: 12px;
            padding: 16px;
            margin: 12px 0;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            transition: all 0.3s ease;
            border: 1px solid rgba(255, 255, 255, 0.2);
            display: flex;
            align-items: center;
            color: #333333;
            position: relative;
            text-decoration: none;
        }
        .link-card:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 15px rgba(0, 0, 0, 0.2);
            background: rgba(255, 255, 255, 0.95);
        }
        .link-icon { width: 24px; height: 24px; margin-right: 12px; filter: invert(0); }
        .social-icon {
            width: 32px;
            height: 32px;
            margin: 0 8px;
            transition: transform 0.3s ease;
            filter: brightness(1) invert(1);
        }
        .social-icon:hover { transform: scale(1.2); }
        .container { max-width: 480px; width: 100%; padding: 20px; }
        .card {
            background: rgba(0, 0, 0, 0.7);
            backdrop-filter: blur(10px);
            border-radius: 16px;
            padding: 25px;
            box-shadow: 0 8px 30px rgba(255, 255, 255, 0.05);
            border: 1px solid rgba(255, 255, 255, 0.1);
            text-align: center;
        }
        .countdown { font-weight: 600; color: #ffffff; font-size: 18px; margin: 15px 0; }
        .footer { margin-top: 20px; color: #aaaaaa; font-size: 12px; opacity: 0.8; }
        .badge {
            background: linear-gradient(90deg, #25D366 0%, #128C7E 100%);
            color: white;
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: 500;
            margin-left: 10px;
        }
        .whatsapp-card {
            background: linear-gradient(135deg, #25D366 0%, #128C7E 100%);
            color: white !important;
        }
        .whatsapp-card:hover {
            background: linear-gradient(135deg, #128C7E 0%, #25D366 100%);
        }
        .portfolio-modal {
            display: none;
            position: fixed;
            top: 0; left: 0;
            width: 100%; height: 100%;
            background: rgba(0,0,0,0.9);
            z-index: 100;
            overflow-y: auto;
        }
        .modal-content {
            background: #111;
            margin: 5% auto;
            padding: 30px;
            max-width: 900px;
            border-radius: 10px;
            box-shadow: 0 0 30px rgba(255,255,255,0.1);
        }
        .close-btn {
            color: #fff;
            font-size: 28px;
            font-weight: bold;
            position: absolute;
            right: 30px; top: 15px;
            cursor: pointer;
        }
        .product-grid { display: grid; grid-template-columns: repeat(auto-fill,minmax(250px,1fr)); gap:25px; margin-top:30px; }
        .product-card { background:#222; border-radius:8px; overflow:hidden; transition:transform 0.3s ease; }
        .product-card:hover { transform: translateY(-5px); box-shadow:0 10px 20px rgba(0,0,0,0.3); }
        .product-image { width:100%; height:600px; object-fit:cover; }
        .product-info { padding:15px; }
        .product-title { font-size:18px; margin-bottom:10px; color:#fff; }
        .product-description { font-size:14px; color:#aaa; margin-bottom:15px; }
        .product-badge { display:inline-block; background:#333; color:#fff; padding:3px 8px; border-radius:4px; font-size:12px; margin-right:5px; margin-bottom:5px; }
        .section-title { font-size:28px; margin-bottom:20px; color:#fff; text-align:center; position:relative; padding-bottom:10px; }
        .section-title::after { content:''; position:absolute; bottom:0; left:50%; transform:translateX(-50%); width:100px; height:3px; background:linear-gradient(90deg,#25D366,#128C7E);}
    </style>
</head>
<body>
    <div class="container">
        <div class="card">
            <div class="flex justify-center mb-4">
                <img src="https://i.imgur.com/VQB3JQb.jpg" alt="Foto de perfil" class="profile-img">
            </div>
            <h1 class="text-2xl font-bold mb-1">STAIRCASE</h1>
            <p class="mb-4">Escadas Pré-moldadas</p>
            <div class="flex justify-center mb-6">
                <a href="https://www.instagram.com/staircase.df?igsh=cGtvb2o1eXV5eGQ=" class="mx-2" target="_blank">
                    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/instagram.svg" alt="Instagram" class="social-icon">
                </a>
                <a href="https://www.facebook.com/share/16uqat6Umr/" class="mx-2" target="_blank">
                    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/facebook.svg" alt="Facebook" class="social-icon">
                </a>
 
            </div>
            <div class="mb-6">
                <a href="#" id="portfolio-btn" class="link-card">
                    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/bookstack.svg" alt="Ícone de catálogo" class="link-icon">
                    <span>Nossos Produtos</span>
                </a>
                <a href="https://w.app/3pskar" class="link-card whatsapp-card" target="_blank">
                    <img src="https://cdn.jsdelivr.net/gh/simple-icons/simple-icons/icons/whatsapp.svg" alt="WhatsApp" class="link-icon">
                    <span>Orçamento via WhatsApp</span>
                    <span class="badge">Online</span>
                </a>
            </div>
            <div class="countdown">
                Atendimento <span id="business-hours" style="color:#25D366">24h (ABERTO)</span>
            </div>
            <p class="footer">© 2025 StairCase Escadas Premoldadas. Todos os direitos reservados.</p>
        </div>
    </div>

    <!-- Modal de Produtos -->
    <div id="portfolio-modal" class="portfolio-modal">
        <div class="modal-content">
            <span class="close-btn">&times;</span>
            <h2 class="section-title">Nossas Escadas Pré-moldadas</h2>
            <p style="text-align:center; color:#ccc;">Soluções em concreto para todos os tipos de projetos</p>
            
            <div class="product-grid">
                <!-- Produto 1 -->
                <div class="product-card">
                    <img src="https://i.imgur.com/Vof5B7q.jpg" alt="Escada Reta" class="product-image">
                    <div class="product-info">
                        <h3 class="product-title">Escada Semi Caracol</h3>
                        <p class="product-description">Modelo linear ideal para projetos residenciais e comerciais.</p>
                    </div>
                </div>

                <!-- Produto 2 -->
                <div class="product-card">
                    <img src="https://i.imgur.com/kb6IBWm.jpeg" alt="Escada em L" class="product-image">
                    <div class="product-info">
                        <h3 class="product-title">Escada Caracol</h3>
                        <p class="product-description">Solução prática e elegante para quem deseja economia de espaço sem abrir mão do design.</p>
                    </div>
                </div>

                <!-- Produto 3 -->
                <div class="product-card">
                    <img src="https://i.imgur.com/xy3vHFC.jpeg" alt="Escada Caracol" class="product-image">
                    <div class="product-info">
                        <h3 class="product-title">Escada Reta</h3>
                        <p class="product-description">Design moderno e sofisticado, une praticidade e estilo para valorizar qualquer ambiente.</p>
                    </div>
                </div>

                <!-- Produto 4 -->
                <div class="product-card">
                    <img src="https://i.imgur.com/f6CLJKu.jpeg" alt="Escada Monumental" class="product-image">
                    <div class="product-info">
                        <h3 class="product-title">Escada em L</h3>
                        <p class="product-description">Escada robusta para projetos de destaque em grandes ambientes.</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        document.getElementById('portfolio-btn').addEventListener('click', function(e){
            e.preventDefault();
            document.getElementById('portfolio-modal').style.display = 'block';
        });
        document.querySelector('.close-btn').addEventListener('click', function(){
            document.getElementById('portfolio-modal').style.display = 'none';
        });
        window.addEventListener('click', function(e){
            if(e.target === document.getElementById('portfolio-modal')){
                document.getElementById('portfolio-modal').style.display = 'none';
            }
        });

        document.querySelectorAll('.link-card:not(#portfolio-btn)').forEach(link => {
            link.addEventListener('click', function(){
                this.style.transform = 'scale(0.95)';
                setTimeout(()=>{ this.style.transform = ''; },200);
            });
        });
    </script>
</body>
</html>
