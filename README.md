# -ALUR-HIJAU-OFFICIAL
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Alur Hijau - Dunia Bertani Milenial & Zoomers</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Montserrat:wght@400;500;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        :root {
            --primary: #2E8B57;
            --primary-dark: #1F6E4A;
            --primary-light: #3DAE6A;
            --accent: #FFD700;
            --text: #FFFFFF;
            --text-secondary: #E8F5E9;
            --card-bg: rgba(255, 255, 255, 0.1);
            --card-border: rgba(255, 255, 255, 0.2);
        }
        
        body {
            font-family: 'Poppins', sans-serif;
            color: var(--text);
            line-height: 1.6;
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), 
                        url('https://images.unsplash.com/photo-1625246333193-4c6b97888175?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=2000&q=80') no-repeat center center fixed;
            background-size: cover;
            min-height: 100vh;
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* ===== HEADER ===== */
        header {
            text-align: center;
            padding: 30px 20px 20px;
        }
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: 30px;
            background: linear-gradient(135deg, var(--card-bg), rgba(255, 255, 255, 0.05));
            border-radius: 20px;
            padding: 30px;
            backdrop-filter: blur(12px);
            border: 1px solid var(--card-border);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.2);
            max-width: 650px;
            margin-left: auto;
            margin-right: auto;
            transition: transform 0.3s ease;
        }
        
        .logo-circle {
            width: 200px;
            height: 200px;
            border-radius: 50%;
            background: linear-gradient(135deg, var(--primary), var(--primary-dark), var(--primary-light));
            display: flex;
            align-items: center;
            justify-content: center;
            margin-bottom: 25px;
            border: 5px solid rgba(255, 255, 255, 0.8);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            position: relative;
            overflow: hidden;
        }
        
        .logo-content {
            text-align: center;
            width: 100%;
        }
        
        .logo-line {
            display: block;
            font-weight: bold;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }
        
        .logo-line-1 {
            font-size: 30px;
            color: var(--text);
            margin-bottom: 8px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 500;
        }
        
        .logo-line-2 {
            font-size: 42px;
            color: var(--accent);
            margin-bottom: 8px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            letter-spacing: 1px;
        }
        
        .logo-line-3 {
            font-size: 28px;
            color: var(--text);
            margin-bottom: 15px;
            font-family: 'Montserrat', sans-serif;
            font-weight: 500;
        }
        
        .logo-quote {
            font-style: italic;
            font-size: 18px;
            color: var(--text-secondary);
            background: linear-gradient(to right, transparent, rgba(0, 100, 0, 0.6), transparent);
            padding: 12px 25px;
            border-radius: 30px;
            display: inline-block;
            margin-top: 15px;
            font-weight: 300;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .welcome-container {
            background: linear-gradient(135deg, var(--card-bg), rgba(255, 255, 255, 0.05));
            border-radius: 20px;
            padding: 30px;
            backdrop-filter: blur(10px);
            border: 1px solid var(--card-border);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
            max-width: 800px;
            margin: 0 auto 40px;
        }
        
        .welcome-title {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 2.4rem;
            text-align: center;
            margin-bottom: 15px;
            color: var(--accent);
            text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.5);
        }
        
        .welcome-subtitle {
            font-size: 1.2rem;
            text-align: center;
            color: var(--text-secondary);
            max-width: 600px;
            margin: 0 auto;
            font-weight: 300;
        }
        
        /* ===== NAVIGASI MOBILE ===== */
        .mobile-nav {
            display: none;
            position: fixed;
            bottom: 0;
            left: 0;
            width: 100%;
            background: var(--primary-dark);
            z-index: 1000;
            padding: 12px 0;
            box-shadow: 0 -2px 10px rgba(0, 0, 0, 0.2);
        }
        
        .nav-icons {
            display: flex;
            justify-content: space-around;
            align-items: center;
        }
        
        .nav-icon {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-decoration: none;
            color: white;
            font-size: 0.8rem;
        }
        
        .nav-icon i {
            font-size: 1.4rem;
            margin-bottom: 4px;
        }
        
        /* ===== BAGIAN KONTEN ===== */
        .section {
            background: linear-gradient(135deg, var(--card-bg), rgba(255, 255, 255, 0.05));
            border-radius: 20px;
            padding: 35px;
            margin-bottom: 40px;
            backdrop-filter: blur(10px);
            border: 1px solid var(--card-border);
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
        }
        
        .section-title {
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            font-size: 2rem;
            margin-bottom: 25px;
            text-align: center;
            padding-bottom: 15px;
            border-bottom: 2px solid rgba(255, 255, 255, 0.2);
            color: var(--accent);
        }
        
        .content-list {
            list-style-type: none;
            padding: 0 20px;
        }
        
        .content-list li {
            margin-bottom: 18px;
            padding-left: 35px;
            position: relative;
            font-size: 1.1rem;
        }
        
        .content-list li:before {
            content: "▸";
            color: var(--accent);
            font-size: 1.5rem;
            position: absolute;
            left: 0;
            top: -3px;
        }
        
        .videos-container {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 30px;
            margin-top: 30px;
        }
        
        .video-wrapper {
            position: relative;
            padding-bottom: 56.25%;
            height: 0;
            overflow: hidden;
            border-radius: 15px;
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
        }
        
        .video-wrapper iframe {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            border: none;
            border-radius: 15px;
        }
        
        .social-buttons {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            margin-top: 30px;
        }
        
        .social-button {
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(135deg, var(--card-bg), rgba(255, 255, 255, 0.05));
            border: 1px solid var(--card-border);
            border-radius: 12px;
            padding: 15px 20px;
            color: var(--text);
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            backdrop-filter: blur(5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .social-button:hover {
            background: rgba(255, 255, 255, 0.15);
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2);
        }
        
        .social-button i {
            margin-right: 12px;
            font-size: 1.5rem;
        }
        
        .youtube-button {
            background: linear-gradient(135deg, rgba(255, 0, 0, 0.15), rgba(255, 0, 0, 0.1));
        }
        
        .youtube-button:hover {
            background: rgba(255, 0, 0, 0.25);
        }
        
        footer {
            text-align: center;
            padding: 40px 0 80px;
            margin-top: 50px;
            font-size: 1rem;
            color: var(--text-secondary);
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        /* ===== TAMPILAN DESKTOP ===== */
        @media (min-width: 1025px) {
            .container {
                padding: 40px;
            }
            
            header {
                padding: 60px 20px 40px;
            }
            
            .logo-container:hover {
                transform: translateY(-5px);
            }
            
            .welcome-container:hover {
                transform: translateY(-3px);
            }
            
            .section:hover {
                transform: translateY(-3px);
            }
            
            .video-wrapper:hover {
                transform: scale(1.03);
                box-shadow: 0 12px 25px rgba(0, 0, 0, 0.4);
            }
            
            /* Layout grid untuk desktop */
            .desktop-grid {
                display: grid;
                grid-template-columns: 1fr 1fr;
                gap: 30px;
                align-items: start;
            }
            
            /* Animasi untuk desktop */
            @keyframes fadeIn {
                from { opacity: 0; transform: translateY(20px); }
                to { opacity: 1; transform: translateY(0); }
            }
            
            .logo-container, .welcome-container, .section {
                animation: fadeIn 0.8s ease-out forwards;
            }
            
            .section:nth-child(2) {
                animation-delay: 0.2s;
            }
            
            .section:nth-child(3) {
                animation-delay: 0.4s;
            }
            
            .section:nth-child(4) {
                animation-delay: 0.6s;
            }
            
            .section:nth-child(5) {
                animation-delay: 0.8s;
            }
        }
        
        /* ===== TAMPILAN MOBILE ===== */
        @media (max-width: 768px) {
            .container {
                padding: 15px;
            }
            
            header {
                padding: 20px 15px 15px;
            }
            
            .logo-container {
                padding: 20px 15px;
                margin-bottom: 20px;
                border-radius: 15px;
            }
            
            .logo-circle {
                width: 140px;
                height: 140px;
                margin-bottom: 15px;
                border-width: 4px;
            }
            
            .logo-line-1 {
                font-size: 20px;
            }
            
            .logo-line-2 {
                font-size: 28px;
            }
            
            .logo-line-3 {
                font-size: 20px;
            }
            
            .logo-quote {
                font-size: 14px;
                padding: 8px 15px;
                margin-top: 10px;
            }
            
            .welcome-container {
                padding: 20px;
                border-radius: 15px;
                margin-bottom: 25px;
            }
            
            .welcome-title {
                font-size: 1.6rem;
                margin-bottom: 10px;
            }
            
            .welcome-subtitle {
                font-size: 1rem;
            }
            
            .section {
                padding: 25px 20px;
                border-radius: 15px;
                margin-bottom: 30px;
            }
            
            .section-title {
                font-size: 1.6rem;
                margin-bottom: 20px;
                padding-bottom: 10px;
            }
            
            .content-list {
                padding: 0 10px;
            }
            
            .content-list li {
                font-size: 1rem;
                padding-left: 25px;
                margin-bottom: 15px;
            }
            
            .content-list li:before {
                font-size: 1.2rem;
                top: -2px;
            }
            
            .videos-container {
                grid-template-columns: 1fr;
                gap: 20px;
                margin-top: 20px;
            }
            
            .video-wrapper {
                border-radius: 12px;
            }
            
            .social-buttons {
                grid-template-columns: 1fr;
                gap: 15px;
                margin-top: 20px;
            }
            
            .social-button {
                padding: 12px 15px;
                border-radius: 10px;
            }
            
            .social-button i {
                font-size: 1.3rem;
                margin-right: 10px;
            }
            
            footer {
                padding: 30px 0 70px;
                margin-top: 30px;
                font-size: 0.9rem;
            }
            
            /* Tampilkan navigasi mobile */
            .mobile-nav {
                display: block;
            }
            
            /* Sembunyikan hover effects di mobile */
            .logo-container, .welcome-container, .section, .video-wrapper {
                transition: none;
            }
            
            .logo-container:hover, .welcome-container:hover, .section:hover, .video-wrapper:hover {
                transform: none;
            }
        }

        /* Tampilan untuk tablet */
        @media (min-width: 769px) and (max-width: 1024px) {
            .container {
                padding: 30px;
            }
            
            .videos-container {
                grid-template-columns: 1fr 1fr;
            }
            
            .social-buttons {
                grid-template-columns: 1fr 1fr;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <header>
            <div class="logo-container">
                <div class="logo-circle">
                    <div class="logo-content">
                        <span class="logo-line logo-line-1">Petani</span>
                        <span class="logo-line logo-line-2">Alur Hijau</span>
                        <span class="logo-line logo-line-3">Zoomers</span>
                    </div>
                </div>
                <div class="logo-quote">Bertani itu perjalanan, bukan tujuan.</div>
            </div>
            
            <div class="welcome-container">
                <h1 class="welcome-title">Selamat Datang di Komunitas Pertanian Modern</h1>
                <p class="welcome-subtitle">Temukan inspirasi, edukasi, dan kisah-kisah inspiratif seputar pertanian untuk generasi milenial dan zoomers</p>
            </div>
        </header>
        
        <main class="desktop-grid">
            <div>
                <section class="section">
                    <h2 class="section-title">Video Pilihan</h2>
                    <div class="videos-container">
                        <div class="video-wrapper">
                            <iframe src="https://www.youtube.com/embed/rMyjPbcSvYs" title="Video Pertanian 1" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                        <div class="video-wrapper">
                            <iframe src="https://www.youtube.com/embed/faEDY7qFjkk" title="Video Pertanian 2" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                        </div>
                    </div>
                </section>
                
                <section class="section">
                    <h2 class="section-title">Tentang Channel</h2>
                    <ul class="content-list">
                        <li>Konten-konten Inspirasi Pertanian</li>
                        <li>Menceritakan kisah-kisah inspiratif</li>
                        <li>Menjadi ruang suara bagi petani dan masyarakat kecil</li>
                        <li>Mengingatkan bahwa setiap aktivitas tani adalah ibadah</li>
                    </ul>
                </section>
            </div>
            
            <div>
                <section class="section">
                    <h2 class="section-title">Konten Pilihan</h2>
                    <ul class="content-list">
                        <li>Video edukasi bertani</li>
                        <li>Foto edukasi pertanian</li>
                        <li>Kisah Inspirasi</li>
                        <li>Tutorial pertanian modern</li>
                        <li>Tips bisnis hasil pertanian</li>
                    </ul>
                </section>
                
                <section class="section">
                    <h2 class="section-title">Ikuti Media Sosial Kita</h2>
                    <div class="social-buttons">
                        <a href="https://www.tiktok.com/@alurhijau?_t=ZS-8zI4qOeOVJw&_r=1" class="social-button" target="_blank">
                            <i class="fab fa-tiktok"></i> TikTok
                        </a>
                        <a href="https://www.instagram.com/abd.grace.bjr?igsh=MTJtc2JvNThkeHAyaQ==" class="social-button" target="_blank">
                            <i class="fab fa-instagram"></i> Instagram
                        </a>
                        <a href="https://www.facebook.com/share/1FpX2v64b8/" class="social-button" target="_blank">
                            <i class="fab fa-facebook"></i> Facebook
                        </a>
                        <a href="https://www.youtube.com/@alurhijaupetanizoomers" class="social-button youtube-button" target="_blank">
                            <i class="fab fa-youtube"></i> YouTube
                        </a>
                    </div>
                </section>
            </div>
        </main>
        
        <footer>
            <p>&copy; 2025 Alur Hijau - Dunia Bertani Milenial & Zoomers</p>
        </footer>
    </div>
    
    <!-- Navigasi Mobile -->
    <nav class="mobile-nav">
        <div class="nav-icons">
            <a href="#home" class="nav-icon">
                <i class="fas fa-home"></i>
                <span>Home</span>
            </a>
            <a href="#videos" class="nav-icon">
                <i class="fas fa-play-circle"></i>
                <span>Video</span>
            </a>
            <a href="#about" class="nav-icon">
                <i class="fas fa-info-circle"></i>
                <span>Tentang</span>
            </a>
            <a href="#social" class="nav-icon">
                <i class="fas fa-share-alt"></i>
                <span>Sosial</span>
            </a>
        </div>
    </nav>
</body>
</html>
