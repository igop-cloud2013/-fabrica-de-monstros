<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Academia Fábrica de Monstros CT Guarulhos</title>
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            line-height: 1.6;
            color: #333;
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }

        /* Header */
        header {
            background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
            color: white;
            padding: 1rem 0;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.3);
        }

        nav {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.8rem;
            font-weight: 700;
            color: #ff6b35;
            text-decoration: none;
        }

        .nav-links {
            display: flex;
            list-style: none;
            gap: 2rem;
        }

        .nav-links a {
            color: white;
            text-decoration: none;
            font-weight: 500;
            transition: color 0.3s;
        }

        .nav-links a:hover {
            color: #ff6b35;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 600"><rect fill="%231a1a1a" width="1200" height="600"/><path fill="%23ff6b35" opacity="0.1" d="M0 300 Q300 0 600 300 T1200 300 V600 H0 Z"/></svg>');
            background-size: cover;
            background-position: center;
            height: 100vh;
            display: flex;
            align-items: center;
            text-align: center;
            color: white;
            margin-top: 80px;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .rating {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 0.5rem;
            font-size: 1.2rem;
            margin-bottom: 2rem;
            color: #ff6b35;
        }

        .cta-button {
            display: inline-block;
            background: #ff6b35;
            color: white;
            padding: 1rem 2.5rem;
            text-decoration: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 1.1rem;
            transition: all 0.3s;
            box-shadow: 0 5px 15px rgba(255,107,53,0.4);
        }

        .cta-button:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 25px rgba(255,107,53,0.6);
        }

        /* Section */
        section {
            padding: 5rem 0;
        }

        .section-title {
            text-align: center;
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: #1a1a1a;
        }

        /* Info Cards */
        .info-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin-bottom: 3rem;
        }

        .info-card {
            background: white;
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s;
        }

        .info-card:hover {
            transform: translateY(-10px);
        }

        .info-icon {
            font-size: 3rem;
            color: #ff6b35;
            margin-bottom: 1rem;
        }

        /* Reviews */
        .reviews-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
            gap: 2rem;
        }

        .review-card {
            background: linear-gradient(135deg, #f8f9fa 0%, #e9ecef 100%);
            padding: 2rem;
            border-radius: 20px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.1);
        }

        .stars {
            color: #ff6b35;
            font-size: 1.2rem;
            margin-bottom: 1rem;
        }

        .review-author {
            font-weight: 600;
            color: #1a1a1a;
            margin-bottom: 0.5rem;
        }

        /* Contact */
        .contact {
            background: linear-gradient(135deg, #1a1a1a 0%, #2d2d2d 100%);
            color: white;
        }

        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 2rem;
            text-align: center;
        }

        /* Footer */
        footer {
            background: #1a1a1a;
            color: white;
            text-align: center;
            padding: 2rem 0;
        }

        /* Mobile */
        @media (max-width: 768px) {
            .nav-links {
                display: none;
            }

            .hero-content h1 {
                font-size: 2.5rem;
            }

            .section-title {
                font-size: 2rem;
            }
        }

        /* Animations */
        @keyframes fadeInUp {
            from {
                opacity: 0;
                transform: translateY(30px);
            }
            to {
                opacity: 1;
                transform: translateY(0);
            }
        }

        .fade-in {
            animation: fadeInUp 0.8s ease-out;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <nav class="container">
            <a href="#" class="logo">🏋️ Fábrica de Monstros</a>
            <ul class="nav-links">
                <li><a href="#home">Início</a></li>
                <li><a href="#sobre">Sobre</a></li>
                <li><a href="#avaliacoes">Avaliações</a></li>
                <li><a href="#contato">Contato</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero -->
    <section id="home" class="hero">
        <div class="container hero-content fade-in">
            <h1>Fábrica de Monstros CT Guarulhos</h1>
            <div class="rating">
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <i class="fas fa-star"></i>
                <span>4.7 (110 avaliações)</span>
            </div>
            <a href="#contato" class="cta-button">Matricule-se Agora</a>
        </div>
    </section>

    <!-- Informações -->
    <section id="sobre" class="container fade-in">
        <h2 class="section-title">Sobre a Academia</h2>
        <div class="info-grid">
            <div class="info-card">
                <div class="info-icon">
                    <i class="fas fa-clock"></i>
                </div>
                <h3>Aberto 24 Horas</h3>
                <p>Treine quando quiser, no seu horário!</p>
            </div>
            <div class="info-card">
                <div class="info-icon">
                    <i class="fas fa-map-marker-alt"></i>
                </div>
                <h3>Localização</h3>
                <p>Jardim Pres. Dutra, Guarulhos - SP<br>07210-000</p>
            </div>
            <div class="info-card">
                <div class="info-icon">
                    <i class="fas fa-phone"></i>
                </div>
                <h3>Contato</h3>
                <p>(11) 97697-9900</p>
            </div>
            <div class="info-card">
                <div class="info-icon">
                    <i class="fas fa-parking"></i>
                </div>
                <h3>Estacionamento</h3>
                <p>Estacionamento gratuito e fácil acesso pela Dutra</p>
            </div>
        </div>
    </section>

    <!-- Avaliações -->
    <section id="avaliacoes">
        <div class="container">
            <h2 class="section-title">O que nossos alunos dizem</h2>
            <div class="reviews-grid">
                <div class="review-card fade-in">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="review-author">Nick - Local Guide</div>
                    <p>"A academia é bonita, espaçosa, limpa e possui um ótimo atendimento. Há boas opções de aparelhos, mas o diferencial são os aparelhos exclusivos!"</p>
                </div>
                <div class="review-card fade-in">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="review-author">Jennyfer Milleni</div>
                    <p>"Academia bem equipada, muito organizada e os professores são ótimos!"</p>
                </div>
                <div class="review-card fade-in">
                    <div class="stars">
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                        <i class="fas fa-star"></i>
                    </div>
                    <div class="review-author">Débora Lemes Dias</div>
                    <p>"A alguns anos procurei a academia como uma válvula de escape para ajudar na depressão e crises constantes de ansiedade... Hoje percebo que as coisas mudaram completamente!"</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contato -->
    <section id="contato" class="contact">
        <div class="container">
            <h2 class="section-title" style="color: white;">Entre em Contato</h2>
            <div class="contact-grid fade-in">
                <div>
                    <i class="fas fa-phone" style="font-size: 2rem; color: #ff6b35; margin-bottom: 1rem;"></i>
                    <h3>(11) 97697-9900</h3>
                </div>
                <div>
                    <i class="fas fa-map-marker-alt" style="font-size: 2rem; color: #ff6b35; margin-bottom: 1rem;"></i>
                    <h3>Jardim Pres. Dutra<br>Guarulhos - SP</h3>
                </div>
                <div>
                    <i class="fas fa-clock" style="font-size: 2rem; color: #ff6b35; margin-bottom: 1rem;"></i>
                    <h3>Aberto 24 horas</h3>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="container">
            <p>&copy; 2024 Fábrica de Monstros CT Guarulhos. Todos os direitos reservados.</p>
        </div>
    </footer>

    <script>
        // Smooth scroll
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Fade in on scroll
        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('fade-in');
                }
            });
        });

        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
</html>
