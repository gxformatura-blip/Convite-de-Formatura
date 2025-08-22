<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Convite de Formatura - Medicina UNISUL 2025</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Montserrat', 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        :root {
            --accent-color: #1a5f7a;
            --accent-light: #4da6cc;
            --dark-blue: #0a2840;
            --gold: #d4af37;
            --light-bg: #f8f9fa;
            --text-dark: #333;
            --text-light: #fff;
            --shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }

        body {
            background-color: var(--light-bg);
            color: var(--text-dark);
            line-height: 1.6;
            background-image: linear-gradient(to bottom, #f0f8ff, #e6f7ff);
            padding: 20px;
            min-height: 100vh;
        }

        .container {
            max-width: 1000px;
            width: 100%;
            margin: 0 auto;
        }

        /* Estilos do convite principal */
        .invitation-page {
            display: block;
        }

        .confirmation-page {
            display: none;
        }

        header {
            text-align: center;
            padding: 30px 0;
            background: linear-gradient(135deg, var(--accent-color), var(--dark-blue));
            color: var(--text-light);
            border-radius: 10px;
            margin-bottom: 30px;
            box-shadow: var(--shadow);
            position: relative;
            overflow: hidden;
        }

        header::before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 5px;
            background: var(--gold);
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 10px;
            font-weight: 300;
            letter-spacing: 2px;
        }

        header p {
            font-size: 1.2rem;
            opacity: 0.9;
        }

        .card {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            margin-bottom: 30px;
            position: relative;
        }

        .logo-section {
            text-align: center;
            padding: 20px;
            background: linear-gradient(to right, var(--dark-blue), var(--accent-color));
            color: white;
        }

        .logo-container {
            display: flex;
            justify-content: center;
            align-items: center;
            margin-bottom: 15px;
        }

        .logo {
            font-size: 2.2rem;
            font-weight: bold;
            color: var(--gold);
            text-align: center;
            line-height: 1.2;
            padding: 15px;
            border: 2px solid var(--gold);
            border-radius: 10px;
            background: rgba(0, 0, 0, 0.2);
        }

        .logo-text {
            font-size: 1rem;
            margin-top: 10px;
            font-style: italic;
            color: var(--gold);
        }

        .hero {
            position: relative;
            height: 400px;
            background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.7)), url('https://images.unsplash.com/photo-1588776814546-ec1aeb0bc9c4?ixlib=rb-4.0.3&auto=format&fit=crop&w=1400&q=80');
            background-size: cover;
            background-position: center;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-align: center;
        }

        .hero-content {
            max-width: 700px;
            padding: 20px;
            z-index: 2;
        }

        .hero-content h2 {
            font-size: 2.2rem;
            margin-bottom: 15px;
            font-weight: 400;
            line-height: 1.3;
        }

        .hero-content p {
            font-size: 1.4rem;
            margin-bottom: 20px;
        }

        .honoree {
            font-size: 2rem;
            font-weight: 500;
            margin: 15px 0;
            color: var(--text-light);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .course {
            font-size: 1.5rem;
            margin-bottom: 25px;
            color: var(--text-light);
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .details {
            padding: 30px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }

        .detail-card {
            background: var(--light-bg);
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s ease;
            border-left: 4px solid var(--accent-color);
        }

        .detail-card:hover {
            transform: translateY(-5px);
        }

        .detail-card i {
            font-size: 2.2rem;
            color: var(--accent-color);
            margin-bottom: 12px;
        }

        .detail-card h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
            color: var(--dark-blue);
        }

        .detail-card p {
            font-size: 1.1rem;
            color: var(--text-dark);
        }

        .timeline {
            padding: 30px;
            background: linear-gradient(to right, var(--accent-color), var(--dark-blue));
            color: white;
        }

        .timeline h2 {
            text-align: center;
            margin-bottom: 30px;
            font-size: 2rem;
            font-weight: 400;
        }

        .timeline-items {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .timeline-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 20px;
            border-radius: 8px;
            text-align: center;
            flex: 1;
            min-width: 200px;
        }

        .timeline-time {
            font-size: 1.8rem;
            font-weight: 500;
            margin-bottom: 10px;
        }

        .timeline-label {
            font-size: 1.1rem;
        }

        .actions {
            padding: 30px;
            text-align: center;
        }

        .actions h2 {
            margin-bottom: 25px;
            color: var(--dark-blue);
            font-size: 2rem;
            font-weight: 400;
        }

        .action-buttons {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 15px;
        }

        .btn {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            padding: 12px 25px;
            background: var(--accent-color);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            background: var(--dark-blue);
            transform: translateY(-3px);
        }

        .btn i {
            font-size: 1.2rem;
        }

        .btn-outline {
            background: transparent;
            border: 2px solid var(--accent-color);
            color: var(--accent-color);
        }

        .btn-outline:hover {
            background: var(--accent-color);
            color: white;
        }

        .location-link {
            display: block;
            margin-top: 10px;
            color: var(--accent-light);
            text-decoration: none;
            font-weight: 500;
        }

        .location-link:hover {
            text-decoration: underline;
        }

        footer {
            text-align: center;
            padding: 30px;
            margin-top: 40px;
            background: var(--dark-blue);
            color: white;
            border-radius: 10px;
        }

        .footer-content {
            max-width: 600px;
            margin: 0 auto;
        }

        .footer-content p {
            margin: 10px 0;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
        }

        .social-links a {
            color: white;
            font-size: 1.5rem;
            transition: transform 0.3s ease;
        }

        .social-links a:hover {
            transform: translateY(-5px);
        }

        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            z-index: 1000;
            justify-content: center;
            align-items: center;
        }

        .modal-content {
            background-color: white;
            padding: 30px;
            border-radius: 10px;
            text-align: center;
            max-width: 400px;
            width: 90%;
        }

        .modal-close {
            position: absolute;
            top: 15px;
            right: 15px;
            font-size: 1.5rem;
            cursor: pointer;
            color: #333;
        }

        .qrcode {
            width: 200px;
            height: 200px;
            margin: 0 auto 20px;
            background-color: #f0f0f0;
            display: flex;
            justify-content: center;
            align-items: center;
            font-weight: bold;
            color: #333;
        }

        /* Estilos da página de confirmação */
        .confirmation-container {
            background: white;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            margin-bottom: 30px;
        }

        .confirmation-header {
            text-align: center;
            padding: 30px;
            background: linear-gradient(to right, var(--dark-blue), var(--accent-color));
            color: white;
        }

        .confirmation-header h2 {
            font-size: 2.2rem;
            margin-bottom: 15px;
        }

        .confirmation-content {
            padding: 30px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 500;
            color: var(--dark-blue);
        }

        .form-group input,
        .form-group select,
        .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
            transition: border-color 0.3s;
        }

        .form-group input:focus,
        .form-group select:focus,
        .form-group textarea:focus {
            border-color: var(--accent-color);
            outline: none;
        }

        .checkbox-group {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
        }

        .checkbox-group input {
            width: auto;
            margin-right: 10px;
        }

        .confirmation-btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            padding: 15px 30px;
            background: var(--accent-color);
            color: white;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 500;
            transition: all 0.3s ease;
            border: none;
            cursor: pointer;
            font-size: 1.1rem;
            width: 100%;
            margin-top: 20px;
        }

        .confirmation-btn:hover {
            background: var(--dark-blue);
            transform: translateY(-3px);
        }

        .confirmation-btn i {
            font-size: 1.2rem;
        }

        .event-info {
            background: var(--light-bg);
            padding: 20px;
            border-radius: 8px;
            margin-bottom: 30px;
            border-left: 4px solid var(--accent-color);
        }

        .event-info h3 {
            color: var(--dark-blue);
            margin-bottom: 15px;
            font-size: 1.4rem;
        }

        .info-item {
            display: flex;
            margin-bottom: 10px;
        }

        .info-item i {
            color: var(--accent-color);
            margin-right: 10px;
            margin-top: 4px;
            min-width: 20px;
        }

        .success-message {
            display: none;
            text-align: center;
            padding: 40px;
            background: #f0f9f0;
            border-radius: 8px;
            border-left: 4px solid #4caf50;
            margin-top: 20px;
        }

        .success-message i {
            font-size: 3rem;
            color: #4caf50;
            margin-bottom: 20px;
        }

        .success-message h3 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #2e7d32;
        }

        .back-btn {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            margin-bottom: 20px;
            color: var(--accent-color);
            text-decoration: none;
            font-weight: 500;
            cursor: pointer;
        }

        .back-btn:hover {
            text-decoration: underline;
        }

        .loading {
            display: none;
            text-align: center;
            margin-top: 20px;
        }

        .loading i {
            font-size: 2rem;
            color: var(--accent-color);
            animation: spin 1s linear infinite;
        }

        @keyframes spin {
            0% { transform: rotate(0deg); }
            100% { transform: rotate(360deg); }
        }

        @media (max-width: 768px) {
            .hero {
                height: 500px;
            }
            
            .hero-content h2 {
                font-size: 1.8rem;
            }
            
            .honoree {
                font-size: 1.5rem;
            }
            
            .action-buttons {
                flex-direction: column;
                align-items: center;
            }
            
            .btn {
                width: 100%;
                justify-content: center;
            }
            
            .details {
                grid-template-columns: 1fr;
            }
            
            .logo {
                font-size: 1.8rem;
                padding: 10px;
            }
            
            .timeline-items {
                flex-direction: column;
            }
            
            .confirmation-header h2 {
                font-size: 1.8rem;
            }
            
            .confirmation-btn {
                padding: 12px 20px;
                font-size: 1rem;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Página principal do convite -->
        <div class="invitation-page">
            <header>
                <h1>Convite de Formatura</h1>
                <p>Celebre conosco esta conquista tão especial</p>
            </header>

            <div class="card">
                <div class="logo-section">
                    <div class="logo-container">
                        <div class="logo">
                            <div>MEDICINA UNISUL</div>
                            <div>2025</div>
                            <div class="logo-text">uma jornada de transformações e conquistas</div>
                        </div>
                    </div>
                </div>

                <div class="hero">
                    <div class="hero-content">
                        <h2>É com grande alegria que convidamos você para a recepção de formatura de</h2>
                        <p class="honoree">Guilherme Xavier Wensing</p>
                        <p class="course">Medicina – Unisul, Turma 2025</p>
                    </div>
                </div>

                <div class="details">
                    <div class="detail-card">
                        <i class="fas fa-calendar-alt"></i>
                        <h3>Data</h3>
                        <p>12 de Dezembro de 2025</p>
                    </div>
                    
                    <div class="detail-card">
                        <i class="fas fa-clock"></i>
                        <h3>Horário</h3>
                        <p>21:00 (Recepção)</p>
                    </div>
                    
                    <div class="detail-card">
                        <i class="fas fa-map-marker-alt"></i>
                        <h3>Local</h3>
                        <p>Espaço Celebrar Festas e Eventos Laguna</p>
                        <a href="https://share.google/UyMc4H259J9zuk6Zm" class="location-link" target="_blank">
                            <i class="fas fa-link"></i> Ver localização
                        </a>
                    </div>
                    
                    <div class="detail-card">
                        <i class="fas fa-tshirt"></i>
                        <h3>Traje</h3>
                        <p>Esporte fino</p>
                    </div>
                </div>

                <div class="timeline">
                    <h2>Programação do Evento</h2>
                    <div class="timeline-items">
                        <div class="timeline-item">
                            <div class="timeline-time">21:00</div>
                            <div class="timeline-label">Recepção</div>
                        </div>
                        <div class="timeline-item">
                            <div class="timeline-time">23:00</div>
                            <div class="timeline-label">Coquetel de Confraternização</div>
                        </div>
                    </div>
                </div>

                <div class="actions">
                    <h2>Ações</h2>
                    <div class="action-buttons">
                        <button class="btn" onclick="downloadInvite()">
                            <i class="fas fa-download"></i> Baixar Convite
                        </button>
                        <button class="btn" onclick="shareInvite()">
                            <i class="fas fa-share-alt"></i> Compartilhar
                        </button>
                        <button class="btn" onclick="showQRCode()">
                            <i class="fas fa-qrcode"></i> Ver QR Code
                        </button>
                        <button class="btn btn-outline" onclick="showConfirmationPage()">
                            <i class="fas fa-reply"></i> Confirmar Presença
                        </button>
                    </div>
                </div>
            </div>

            <footer>
                <div class="footer-content">
                    <p>Turma de Medicina – Unisul 2025</p>
                    <p>Sua presença tornará este momento ainda mais especial!</p>
                    <div class="social-links">
                        <a href="#"><i class="fab fa-whatsapp"></i></a>
                        <a href="#"><i class="fab fa-instagram"></i></a>
                        <a href="#"><i class="fab fa-facebook"></i></a>
                    </div>
                </div>
            </footer>
        </div>

        <!-- Página de confirmação de presença -->
        <div class="confirmation-page">
            <a class="back-btn" onclick="showInvitationPage()">
                <i class="fas fa-arrow-left"></i> Voltar para o convite
            </a>

            <header>
                <h1>Confirmação de Presença</h1>
                <p>Formatura em Medicina - UNISUL 2025</p>
            </header>

            <div class="confirmation-container">
                <div class="confirmation-header">
                    <h2>Confirmar Presença</h2>
                    <p>Sua confirmação é importante para nós!</p>
                </div>

                <div class="confirmation-content">
                    <div class="event-info">
                        <h3>Informações do Evento</h3>
                        <div class="info-item">
                            <i class="fas fa-user-graduate"></i>
                            <div>Formatura de <strong>Guilherme Xavier Wensing</strong> - Medicina UNISUL</div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-calendar-alt"></i>
                            <div>Data: <strong>12 de Dezembro de 2025</strong></div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-clock"></i>
                            <div>Horário: <strong>21:00h (Recepção)</strong></div>
                        </div>
                        <div class="info-item">
                            <i class="fas fa-map-marker-alt"></i>
                            <div>Local: <strong>Espaço Celebrar Festas e Eventos Laguna</strong></div>
                        </div>
                    </div>

                    <form id="confirmation-form">
                        <div class="form-group">
                            <label for="name">Nome Completo *</label>
                            <input type="text" id="name" name="name" required>
                        </div>

                        <div class="form-group">
                            <label for="email">E-mail *</label>
                            <input type="email" id="email" name="email" required>
                        </div>

                        <div class="form-group">
                            <label for="phone">Telefone/WhatsApp *</label>
                            <input type="tel" id="phone" name="phone" required>
                        </div>

                        <div class="form-group">
                            <label for="guests">Número de Acompanhantes *</label>
                            <select id="guests" name="guests" required>
                                <option value="">Selecione...</option>
                                <option value="0">Nenhum</option>
                                <option value="1">1 acompanhante</option>
                                <option value="2">2 acompanhantes</option>
                                <option value="3">3 acompanhantes</option>
                                <option value="4">4 acompanhantes</option>
                                <option value="5">5 ou mais acompanhantes</option>
                            </select>
                        </div>

                        <div class="form-group">
                            <label for="guest_names">Nomes dos Acompanhantes</label>
                            <textarea id="guest_names" name="guest_names" rows="3" placeholder="Liste os nomes dos acompanhantes, se houver"></textarea>
                        </div>

                        <div class="form-group">
                            <label for="message">Mensagem (opcional)</label>
                            <textarea id="message" name="message" rows="3" placeholder="Deixe uma mensagem para o formando"></textarea>
                        </div>

                        <div class="checkbox-group">
                            <input type="checkbox" id="confirm-presence" name="confirm-presence" required>
                            <label for="confirm-presence">Confirmo minha presença na formatura</label>
                        </div>

                        <button type="submit" class="confirmation-btn">
                            <i class="fas fa-check-circle"></i> Confirmar Presença
                        </button>
                    </form>

                    <div class="loading" id="loading">
                        <i class="fas fa-spinner"></i>
                        <p>Enviando confirmação...</p>
                    </div>

                    <div class="success-message" id="success-message">
                        <i class="fas fa-check-circle"></i>
                        <h3>Confirmação enviada com sucesso!</h3>
                        <p>Obrigado por confirmar sua presença. Estamos ansiosos para celebrar este momento especial com você!</p>
                    </div>
                </div>
            </div>
        </div>

        <!-- Modal para QR Code -->
        <div id="qrcode-modal" class="modal">
            <div class="modal-content">
                <span class="modal-close" onclick="closeModal('qrcode-modal')">&times;</span>
                <h2>QR Code do Convite</h2>
                <div class="qrcode">
                    <!-- QR Code será gerado aqui -->
                    <span>QR Code</span>
                </div>
                <p>Use a câmera do seu celular para escanear este código</p>
            </div>
        </div>
    </div>

    <script>
        // Função para mostrar a página de confirmação
        function showConfirmationPage() {
            document.querySelector('.invitation-page').style.display = 'none';
            document.querySelector('.confirmation-page').style.display = 'block';
            window.scrollTo(0, 0);
        }

        // Função para mostrar a página principal do convite
        function showInvitationPage() {
            document.querySelector('.confirmation-page').style.display = 'none';
            document.querySelector('.invitation-page').style.display = 'block';
            window.scrollTo(0, 0);
        }

        // Função para simular o download do convite
        function downloadInvite() {
            alert('Funcionalidade de download será implementada aqui!');
            // Em uma implementação real, aqui seria o código para gerar o PDF
        }

        // Função para compartilhar o convite
        function shareInvite() {
            if (navigator.share) {
                navigator.share({
                    title: 'Convite de Formatura - Medicina Unisul 2025',
                    text: 'Convite para formatura de Medicina da Unisul, Turma 2025',
                    url: window.location.href
                })
                .then(() => console.log('Compartilhado com sucesso'))
                .catch((error) => console.log('Erro ao compartilhar:', error));
            } else {
                alert('Seu navegador não suporta a funcionalidade de compartilhamento. Você pode copiar o link manualmente.');
            }
        }

        // Função para mostrar QR Code
        function showQRCode() {
            document.getElementById('qrcode-modal').style.display = 'flex';
        }

        // Função para fechar modal
        function closeModal(modalId) {
            document.getElementById(modalId).style.display = 'none';
        }

        // Fechar modal clicando fora dele
        window.onclick = function(event) {
            if (event.target.classList.contains('modal')) {
                event.target.style.display = 'none';
            }
        }

        // Validação do formulário de confirmação
        document.getElementById('confirmation-form').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Mostrar loading
            document.getElementById('loading').style.display = 'block';
            document.getElementById('success-message').style.display = 'none';
            
            // Coletar dados do formulário
            const formData = new FormData(e.target);
            const data = Object.fromEntries(formData.entries());
            
            // Enviar email de confirmação
            sendConfirmationEmail(data);
        });

        // Função para enviar email de confirmação
        function sendConfirmationEmail(data) {
            // Configurações do email (em produção, isso deve ser feito no servidor)
            const serviceID = 'default_service';
            const templateID = 'template_confirmacao';
            
            // Simulação do envio do email (em um ambiente real, isso seria feito com uma API)
            setTimeout(() => {
                // Esconder loading
                document.getElementById('loading').style.display = 'none';
                
                // Mostrar mensagem de sucesso
                document.getElementById('success-message').style.display = 'block';
                
                // Limpar formulário
                document.getElementById('confirmation-form').reset();
                
                // Rolar para a mensagem de sucesso
                document.getElementById('success-message').scrollIntoView({ behavior: 'smooth' });
                
                // Log para demonstração (em produção, isso enviaria um email real)
                console.log('Dados da confirmação:', data);
                console.log('Email de confirmação enviado para: guixavier1284@gmail.com');
                
            }, 2000); // Simula um tempo de envio
        }

        // Validação do campo de telefone
        document.getElementById('phone').addEventListener('input', function(e) {
            e.target.value = e.target.value.replace(/\D/g, '');
        });

        // Mostrar/ocultar campo de nomes dos acompanhantes baseado na seleção
        document.getElementById('guests').addEventListener('change', function(e) {
            const guestsValue = parseInt(e.target.value);
            const guestNamesField = document.getElementById('guest_names');
            
            if (guestsValue > 0) {
                guestNamesField.closest('.form-group').style.display = 'block';
                guestNamesField.setAttribute('required', 'required');
            } else {
                guestNamesField.closest('.form-group').style.display = 'none';
                guestNamesField.removeAttribute('required');
            }
        });

        // Inicialmente esconder o campo de nomes dos acompanhantes
        document.getElementById('guest_names').closest('.form-group').style.display = 'none';

        // Inicialização
        document.addEventListener('DOMContentLoaded', function() {
            console.log('Convite de formatura carregado!');
        });
    </script>

    <!-- EmailJS para envio de emails -->
    <script src="https://cdn.jsdelivr.net/npm/emailjs-com@3.2.0/dist/email.min.js"></script>
    <script>
        // Inicializar EmailJS (substitua com seu User ID)
        // emailjs.init("SEU_USER_ID_AQUI");
        
        // Em um ambiente real, descomente a linha acima e adicione seu User ID do EmailJS
        // Para mais informações: https://www.emailjs.com/
    </script>
</body>
</html>
