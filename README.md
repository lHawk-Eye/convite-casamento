<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite de Casamento - Naiara & André</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@500;600;700&family=Montserrat:wght@400;500&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            background: #f5f0e5;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
            font-family: 'Montserrat', sans-serif;
        }
        
        .invitation-container {
            width: 100%;
            max-width: 500px;
            background: #f8f6f0;
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.15);
            overflow: hidden;
            text-align: center;
            position: relative;
            border: 2px solid #8d6e63;
            padding: 40px 30px;
        }
        
        .card-header {
            margin-bottom: 30px;
            padding-bottom: 20px;
            border-bottom: 2px dashed #8d6e63;
        }
        
        .bride-name {
            font-family: 'Cormorant Garamond', serif;
            font-size: 42px;
            color: #6d4c41;
            margin-bottom: 5px;
            font-weight: 700;
            letter-spacing: 2px;
        }
        
        .groom-name {
            font-family: 'Cormorant Garamond', serif;
            font-size: 36px;
            color: #6d4c41;
            margin-top: 5px;
            font-weight: 700;
            letter-spacing: 2px;
        }
        
        .and-text {
            font-family: 'Cormorant Garamond', serif;
            font-size: 24px;
            color: #7cb342;
            margin: 10px 0;
            font-style: italic;
        }
        
        .card-content {
            color: #5d4037;
            line-height: 1.6;
            margin: 25px 0;
            font-size: 18px;
        }
        
        .highlight {
            color: #7cb342;
            font-weight: bold;
        }
        
        .details {
            margin: 25px 0;
            color: #5d4037;
            text-align: left;
            padding: 0 15px;
        }
        
        .date, .location, .dress-code {
            margin-bottom: 15px;
            font-size: 18px;
            display: flex;
            align-items: center;
        }
        
        .date i, .location i, .dress-code i {
            margin-right: 15px;
            color: #7cb342;
            font-size: 22px;
            min-width: 30px;
        }
        
        .confirm-btn {
            display: block;
            width: 100%;
            padding: 18px;
            background: linear-gradient(135deg, #7cb342 0%, #558b2f 100%);
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 20px;
            font-weight: 600;
            cursor: pointer;
            margin: 35px 0 25px;
            box-shadow: 0 5px 20px rgba(124, 179, 66, 0.35);
            transition: all 0.3s ease;
            text-decoration: none;
            font-family: 'Montserrat', sans-serif;
        }
        
        .confirm-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(124, 179, 66, 0.5);
            background: linear-gradient(135deg, #558b2f 0%, #7cb342 100%);
        }
        
        .footer {
            margin-top: 25px;
            color: #8d6e63;
            font-size: 16px;
            font-style: italic;
        }
        
        .link-text {
            margin-top: 15px;
            font-size: 16px;
            color: #5d4037;
            background-color: #f1f8e9;
            padding: 12px;
            border-radius: 8px;
            border-left: 4px solid #7cb342;
            word-break: break-all;
        }
        
        .floral-border {
            position: absolute;
            width: 100%;
            height: 100%;
            top: 0;
            left: 0;
            pointer-events: none;
        }
        
        .corner {
            position: absolute;
            width: 60px;
            height: 60px;
        }
        
        .corner-top-left {
            top: 0;
            left: 0;
            border-top: 3px solid #7cb342;
            border-left: 3px solid #7cb342;
            border-top-left-radius: 15px;
        }
        
        .corner-top-right {
            top: 0;
            right: 0;
            border-top: 3px solid #7cb342;
            border-right: 3px solid #7cb342;
            border-top-right-radius: 15px;
        }
        
        .corner-bottom-left {
            bottom: 0;
            left: 0;
            border-bottom: 3px solid #7cb342;
            border-left: 3px solid #7cb342;
            border-bottom-left-radius: 15px;
        }
        
        .corner-bottom-right {
            bottom: 0;
            right: 0;
            border-bottom: 3px solid #7cb342;
            border-right: 3px solid #7cb342;
            border-bottom-right-radius: 15px;
        }
        
        .share-section {
            margin-top: 30px;
            padding-top: 20px;
            border-top: 1px dashed #8d6e63;
        }
        
        .share-btn {
            display: inline-block;
            padding: 12px 25px;
            background-color: #8d6e63;
            color: white;
            border: none;
            border-radius: 50px;
            font-size: 16px;
            cursor: pointer;
            margin: 10px 5px;
            transition: all 0.3s ease;
        }
        
        .share-btn:hover {
            background-color: #6d4c41;
            transform: translateY(-2px);
        }

        .github-guide {
            margin-top: 30px;
            padding: 20px;
            background-color: #f9f9f9;
            border-radius: 10px;
            border-left: 4px solid #8d6e63;
        }
        
        .github-guide h3 {
            color: #6d4c41;
            margin-bottom: 15px;
        }
        
        .github-guide ol {
            text-align: left;
            padding-left: 20px;
        }
        
        .github-guide li {
            margin-bottom: 10px;
            color: #5d4037;
        }
        
        @media (max-width: 480px) {
            .invitation-container {
                padding: 30px 20px;
            }
            
            .bride-name {
                font-size: 36px;
            }
            
            .groom-name {
                font-size: 30px;
            }
            
            .card-content {
                font-size: 16px;
            }
            
            .date, .location, .dress-code {
                font-size: 16px;
            }
            
            .confirm-btn {
                padding: 15px;
                font-size: 18px;
            }
        }
    </style>
</head>
<body>
    <div class="invitation-container">
        <div class="floral-border">
            <div class="corner corner-top-left"></div>
            <div class="corner corner-top-right"></div>
            <div class="corner corner-bottom-left"></div>
            <div class="corner corner-bottom-right"></div>
        </div>
        
        <div class="card-header">
            <div class="bride-name">NAIARA</div>
            <div class="and-text">e</div>
            <div class="groom-name">ANDRE</div>
        </div>
        
        <div class="card-content">
            Comemore conosco enquanto trocamos alianças! Nosso casamento será no dia <span class="highlight">31 de Outubro</span> às <span class="highlight">13h</span>, no <span class="highlight">Inconfidência Mineira</span>. Venha com o seu melhor <span class="highlight">traje formal vintage</span>!
        </div>
        
        <div class="details">
            <div class="date">
                <i class="far fa-calendar-alt"></i>
                <span>31 de Outubro de 2026</span>
            </div>
            <div class="location">
                <i class="fas fa-map-marker-alt"></i>
                <span>Restaurante Inconfidência Mineira</span>
            </div>
            <div class="dress-code">
                <i class="fas fa-tshirt"></i>
                <span>Traje formal vintage</span>
            </div>
        </div>
        
        <a href="https://www.casamentos.com.br/web/naiara-and-andre/confirmcasuapresenca-3" class="confirm-btn">
            <i class="fas fa-check-circle"></i> Confirmar Presença
        </a>
        
        <div class="footer">
            Não se esqueça de confirmar presença através do link abaixo:
        </div>
        
        <div class="link-text">
            https://www.casamentos.com.br/web/naiara-and-andre/confirmcasuapresenca-3
        </div>
        
        <div class="share-section">
            <p>Compartilhe este convite:</p>
            <button class="share-btn" onclick="shareOnWhatsApp()">
                <i class="fab fa-whatsapp"></i> WhatsApp
            </button>
            <button class="share-btn" onclick="copyLink()">
                <i class="fas fa-link"></i> Copiar Link
            </button>
        </div>

        <div class="github-guide">
            <h3>Como hospedar este convite no GitHub:</h3>
            <ol>
                <li>Crie uma conta gratuita no <a href="https://github.com/" target="_blank">GitHub</a></li>
                <li>Crie um novo repositório com o nome "convite-casamento"</li>
                <li>Faça upload deste arquivo HTML</li>
                <li>Ative o GitHub Pages nas configurações</li>
                <li>Compartilhe o link gerado com seus convidados!</li>
            </ol>
        </div>
    </div>

    <script>
        // Função para compartilhar via WhatsApp
        function shareOnWhatsApp() {
            const text = "Você está convidado para o nosso casamento! Acesse o convite em: ";
            const url = window.location.href;
            const whatsappUrl = `https://wa.me/?text=${encodeURIComponent(text + url)}`;
            window.open(whatsappUrl, '_blank');
        }
        
        // Função para copiar o link do convite
        function copyLink() {
            const url = window.location.href;
            navigator.clipboard.writeText(url).then(() => {
                alert('Link copiado para a área de transferência!');
            }).catch(err => {
                console.error('Erro ao copiar o link: ', err);
            });
        }
        
        // Adicionando algum interatividade adicional
        document.addEventListener('DOMContentLoaded', function() {
            const confirmBtn = document.querySelector('.confirm-btn');
            
            confirmBtn.addEventListener('click', function(e) {
                e.preventDefault();
                const confirmed = confirm('Você será redirecionado para confirmar sua presença. Deseja continuar?');
                if (confirmed) {
                    window.open(this.href, '_blank');
                }
            });
        });
    </script>
</body>
</html>
