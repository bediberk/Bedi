<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Kendimi Tanıtıyorum</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        /* --- GENEL AYARLAR --- */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            overflow: hidden;
            /* Arka Plan Animasyonu */
            background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
            background-size: 400% 400%;
            animation: gradientAnimation 10s ease infinite;
        }

        @keyframes gradientAnimation {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* --- KARTIN KENDİSİ --- */
        .card {
            background: rgba(255, 255, 255, 0.15);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.18);
            border-radius: 20px;
            padding: 50px;
            width: 90%;
            max-width: 500px;
            text-align: center;
            color: white;
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
            /* Kartın Giriş Animasyonu */
            animation: cardIn 1s ease-out;
        }

        @keyframes cardIn {
            0% { transform: scale(0.8) translateY(50px); opacity: 0; }
            100% { transform: scale(1) translateY(0); opacity: 1; }
        }

        /* --- İÇERİK STİLLERİ --- */
        .profile-pic {
            width: 150px;
            height: 150px;
            border-radius: 50%;
            border: 5px solid rgba(255, 255, 255, 0.5);
            margin-bottom: 20px;
            object-fit: cover;
            box-shadow: 0 4px 15px rgba(0,0,0,0.2);
            transition: transform 0.3s ease;
        }

        .profile-pic:hover {
            transform: rotate(10deg) scale(1.05);
        }

        h1 {
            font-size: 2.5em;
            margin-bottom: 10px;
            text-shadow: 0 2px 5px rgba(0,0,0,0.3);
        }

        .tagline {
            font-size: 1.2em;
            color: #f0f0f0;
            margin-bottom: 20px;
            opacity: 0.9;
        }

        .bio {
            margin-bottom: 30px;
            line-height: 1.6;
            font-size: 1em;
            color: #e0e0e0;
        }

        /* --- SOSYAL MEDYA İKONLARI --- */
        .social-icons {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-bottom: 20px;
        }

        .social-icons a {
            font-size: 1.8em;
            color: white;
            text-decoration: none;
            transition: transform 0.3s ease, color 0.3s ease;
            opacity: 0.8;
        }

        .social-icons a:hover {
            transform: translateY(-5px) scale(1.1);
            opacity: 1;
            color: #ffeb3b; /* İkon hover rengi */
        }

        /* --- BUTON --- */
        .btn-contact {
            background: white;
            color: #e73c7e;
            border: none;
            padding: 12px 30px;
            font-size: 1.1em;
            font-weight: bold;
            border-radius: 30px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-decoration: none;
            display: inline-block;
        }

        .btn-contact:hover {
            background: #ffeb3b;
            color: #333;
            box-shadow: 0 5px 15px rgba(0,0,0,0.2);
        }

        /* --- MOBİL UYUMLULUK (Responsive) --- */
        @media (max-width: 600px) {
            .card { padding: 30px; }
            h1 { font-size: 2em; }
            .profile-pic { width: 120px; height: 120px; }
        }
    </style>
</head>
<body>

    <div class="card">
        <!-- BURAYI DEĞİŞTİR: Profil Fotoğrafın -->
        <!-- İstersen bir resim URL'si yapıştır, istersen boş bırak -->
        <img src="https://via.placeholder.com/150" alt="Profil Fotoğrafı" class="profile-pic">

        <!-- BURAYI DEĞİŞTİR: Adın Soyadın -->
        <h1>Adınız Soyadınız</h1>

        <!-- BURAYI DEĞİŞTİR: Kısa bir slogan -->
        <p class="tagline">Web Geliştirici / Tasarımcı / Öğrenci</p>

        <!-- BURAYI DEĞİŞTİR: Kendini anlatan yazı -->
        <p class="bio">
            Merhaba! Ben [Adınız]. Teknolojiye tutkulu biriyim ve kodlama dünyasında yeni şeyler öğrenmekten keyif alıyorum. Şu anda [Okul/İş] alanında kendimi geliştiriyorum. Bu sayfa benim ilk deneme sahalarımdan biri!
        </p>

        <!-- BURAYI DEĞİŞTİR: Sosyal Medya Linklerin -->
        <div class="social-icons">
            <a href="#" title="GitHub"><i class="fab fa-github"></i></a>
            <a href="#" title="LinkedIn"><i class="fab fa-linkedin"></i></a>
            <a href="#" title="Twitter"><i class="fab fa-twitter"></i></a>
            <a href="#" title="Instagram"><i class="fab fa-instagram"></i></a>
        </div>

        <!-- BURAYI DEĞİŞTİR: İletişim Butonu -->
        <a href="mailto:ornek@email.com" class="btn-contact">İletişime Geç</a>
    </div>

</body>
</html>
