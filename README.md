<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>Hialdev • Semua Link</title>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Google Font - Poppins (biar aesthetic) -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: linear-gradient(145deg, #0f0c29, #302b63, #24243e);
            background-attachment: fixed;
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
            color: #fff;
        }

        .container {
            max-width: 500px;
            width: 100%;
            margin: 0 auto;
        }

        /* Card utama dengan efek glassmorphism */
        .bio-card {
            background: rgba(255, 255, 255, 0.1);
            backdrop-filter: blur(15px);
            -webkit-backdrop-filter: blur(15px);
            border-radius: 40px;
            padding: 30px 25px;
            box-shadow: 0 25px 50px -8px rgba(0, 0, 0, 0.4), 0 0 0 1px rgba(255, 255, 255, 0.2) inset;
            border: 1px solid rgba(255, 255, 255, 0.2);
            animation: fadeIn 0.8s ease;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        /* Profile Section */
        .profile {
            text-align: center;
            margin-bottom: 30px;
        }

        .profile-pic {
            width: 110px;
            height: 110px;
            border-radius: 50%;
            background: linear-gradient(135deg, #667eea, #764ba2);
            margin: 0 auto 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            border: 4px solid rgba(255, 255, 255, 0.5);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
        }

        .profile-pic-inner {
            font-size: 3.5rem;
            font-weight: 600;
            color: white;
            text-shadow: 2px 2px 10px rgba(0,0,0,0.3);
        }

        .profile h1 {
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 5px;
            background: linear-gradient(135deg, #fff, #e0e0ff);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }

        .profile p {
            font-size: 1rem;
            opacity: 0.9;
            margin-bottom: 10px;
            color: #ddd;
        }

        .profile-badge {
            display: inline-block;
            background: rgba(255, 255, 255, 0.15);
            padding: 8px 20px;
            border-radius: 50px;
            font-size: 0.9rem;
            border: 1px solid rgba(255, 255, 255, 0.3);
            backdrop-filter: blur(5px);
        }

        .profile-badge i {
            margin-right: 5px;
            color: #ffd700;
        }

        /* Stats Counter */
        .stats {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 30px;
            flex-wrap: wrap;
        }

        .stat-item {
            background: rgba(255, 255, 255, 0.1);
            padding: 10px 20px;
            border-radius: 30px;
            border: 1px solid rgba(255, 255, 255, 0.2);
            text-align: center;
            min-width: 80px;
        }

        .stat-number {
            font-size: 1.5rem;
            font-weight: 700;
            color: white;
        }

        .stat-label {
            font-size: 0.7rem;
            opacity: 0.7;
            text-transform: uppercase;
            letter-spacing: 1px;
        }

        /* Links Section - INI YANG UTAMA */
        .links {
            display: flex;
            flex-direction: column;
            gap: 15px;
            margin-bottom: 30px;
        }

        .link-btn {
            display: flex;
            align-items: center;
            padding: 16px 25px;
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            border-radius: 60px;
            text-decoration: none;
            color: white;
            font-weight: 500;
            font-size: 1.1rem;
            border: 1px solid rgba(255, 255, 255, 0.25);
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        .link-btn:hover {
            transform: scale(1.03);
            background: rgba(255, 255, 255, 0.25);
            border-color: rgba(255, 255, 255, 0.5);
            box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.5);
        }

        .link-btn i {
            font-size: 1.8rem;
            width: 40px;
            text-align: center;
            margin-right: 15px;
        }

        .link-btn .btn-text {
            flex: 1;
        }

        .link-btn .btn-desc {
            font-size: 0.8rem;
            opacity: 0.7;
            display: block;
        }

        .link-btn .arrow {
            font-size: 1.2rem;
            opacity: 0.5;
            transition: 0.3s;
        }

        .link-btn:hover .arrow {
            opacity: 1;
            transform: translateX(5px);
        }

        /* Warna spesifik untuk setiap platform */
        .tiktok { background: linear-gradient(145deg, #000000, #1a1a1a); }
        .facebook { background: linear-gradient(145deg, #1877f2, #0d5ab9); }
        .discord-profile { background: linear-gradient(145deg, #5865F2, #404eed); }
        .discord-server { background: linear-gradient(145deg, #5865F2, #2c3b8f); }
        .sociabuzz { background: linear-gradient(145deg, #FF5E5B, #d43f3c); }
        .whatsapp { background: linear-gradient(145deg, #25D366, #128C7E); }
        .github { background: linear-gradient(145deg, #333, #24292e); }

        /* Featured Section (Server Anomali) */
        .featured {
            background: linear-gradient(145deg, rgba(88, 101, 242, 0.3), rgba(64, 78, 237, 0.3));
            border-radius: 30px;
            padding: 20px;
            margin-bottom: 25px;
            border: 2px solid rgba(88, 101, 242, 0.5);
            text-align: center;
        }

        .featured h3 {
            font-size: 1.3rem;
            margin-bottom: 10px;
        }

        .featured .server-link {
            display: inline-block;
            background: #5865F2;
            color: white;
            padding: 12px 30px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: 600;
            margin-top: 10px;
            border: 1px solid rgba(255,255,255,0.3);
        }

        /* Footer */
        .footer {
            text-align: center;
            margin-top: 20px;
            opacity: 0.6;
            font-size: 0.8rem;
        }

        .footer i {
            color: #ff6b6b;
        }

        /* Responsive */
        @media (max-width: 400px) {
            .bio-card { padding: 20px 15px; }
            .profile h1 { font-size: 1.7rem; }
            .link-btn { padding: 14px 20px; }
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="bio-card">
            <!-- Profile Section -->
            <div class="profile">
                <div class="profile-pic">
                    <div class="profile-pic-inner">Hd</div>
                </div>
                <h1>Hialdev</h1>
                <p>⚡ Content Creator | Developer | Gamer</p>
                <span class="profile-badge">
                    <i class="fas fa-star"></i> 2.5K Followers
                </span>
            </div>

            <!-- Stats Counter (biar hidup) -->
            <div class="stats">
                <div class="stat-item">
                    <div class="stat-number">23</div>
                    <div class="stat-label">Projects</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">1.2K</div>
                    <div class="stat-label">Likes</div>
                </div>
                <div class="stat-item">
                    <div class="stat-number">580</div>
                    <div class="stat-label">Friends</div>
                </div>
            </div>

            <!-- FEATURED: Discord Server Anomali (ditampilkan khusus) -->
            <div class="featured">
                <i class="fab fa-discord" style="font-size: 2.5rem; margin-bottom: 5px;"></i>
                <h3>🎮 JOIN SERVER ANOMALI</h3>
                <p>Gaming Community • Hangout • Kolaborasi • 24/7 Active</p>
                <a href="https://discord.gg/ws4aVYDecJ" target="_blank" class="server-link">
                    <i class="fab fa-discord"></i> Join Sekarang
                </a>
            </div>

            <!-- ALL LINKS - SEMUA LINK KAMU -->
            <div class="links">
                <!-- TikTok -->
                <a href="https://www.tiktok.com/@hialdev01" target="_blank" class="link-btn tiktok">
                    <i class="fab fa-tiktok"></i>
                    <span class="btn-text">
                        TikTok
                        <span class="btn-desc">@hialdev01</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- Facebook -->
                <a href="https://www.facebook.com/share/1HJk7o76T7/" target="_blank" class="link-btn facebook">
                    <i class="fab fa-facebook-f"></i>
                    <span class="btn-text">
                        Facebook
                        <span class="btn-desc">Lal Kimochi</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- Discord Profile -->
                <a href="https://discord.com/users/1460940712131563664" target="_blank" class="link-btn discord-profile">
                    <i class="fab fa-discord"></i>
                    <span class="btn-text">
                        Discord Profile
                        <span class="btn-desc">Hialdev#xxxx</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- Discord Server Anomali (lagi, tapi versi link biasa) -->
                <a href="https://discord.gg/ws4aVYDecJ" target="_blank" class="link-btn discord-server">
                    <i class="fab fa-discord"></i>
                    <span class="btn-text">
                        Server Anomali
                        <span class="btn-desc">Join Discord Server</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- Sociabuzz Donate -->
                <a href="https://sociabuzz.com/lalzyx_/tribe" target="_blank" class="link-btn sociabuzz">
                    <i class="fas fa-coffee"></i>
                    <span class="btn-text">
                        Traktir Kopi
                        <span class="btn-desc">Support via Sociabuzz</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- WhatsApp Group -->
                <a href="https://chat.whatsapp.com/LDKBiA1mf24BB7jKUkYVDV" target="_blank" class="link-btn whatsapp">
                    <i class="fab fa-whatsapp"></i>
                    <span class="btn-text">
                        WA Group SRRVER PT PT X8
                        <span class="btn-desc">Join grup WhatsApp</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>

                <!-- GitHub -->
                <a href="https://github.com/Hialdev" target="_blank" class="link-btn github">
                    <i class="fab fa-github"></i>
                    <span class="btn-text">
                        GitHub
                        <span class="btn-desc">@Hialdev</span>
                    </span>
                    <span class="arrow"><i class="fas fa-chevron-right"></i></span>
                </a>
            </div>

            <!-- Additional Info -->
            <div style="text-align: center; margin-bottom: 15px;">
                <a href="https://discord.gg/ws4aVYDecJ" style="color: #5865F2; text-decoration: none; font-weight: 500;">
                    ⚡ discord.gg/ws4aVYDecJ ⚡
                </a>
            </div>

            <!-- Footer -->
            <div class="footer">
                <p><i class="fas fa-heart"></i> Semua link Hialdev • Updated 2026</p>
                <p style="margin-top: 5px;">Click any link to connect!</p>
            </div>
        </div>
    </div>
</body>
</html>
