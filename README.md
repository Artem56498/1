<!DOCTYPE html>
<html lang="uk">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Овруцький ЗДО №8 Ластівка Овруцької міської ради</title>
    <meta name="description" content="Офіційний сайт ЗДО «Садочок Ластівка». Дитячий садок для гармонійного розвитку дітей від 2 до 7 років. Якісна дошкільна освіта, інклюзивне навчання, досвідчені педагоги.">
    <meta name="keywords" content="ЗДО Ластівка, Садочок Ластівка, ЗДО Садочок Ластівка, дитячий садок, дошкільна освіта, дитячий сад Україна, виховання дітей, інклюзивна освіта">
    <meta name="author" content="Овруцький ЗДО №8 Ластівка Овруцької міської ради">
    <meta name="google-site-verification" content="L3aMoZRFZU0pbWwUjJfPDd5h7hcqdM3p3z4dfj7Qqo4" />
    
    <!-- Firebase SDK -->
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-app-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-auth-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-firestore-compat.js"></script>
    <script src="https://www.gstatic.com/firebasejs/10.7.1/firebase-storage-compat.js"></script>
    
    <!-- Google Analytics -->
    <script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
    <script>
      window.dataLayer = window.dataLayer || [];
      function gtag(){dataLayer.push(arguments);}
      gtag('js', new Date());
      gtag('config', 'G-XXXXXXXXXX');
    </script>
    
    <!-- Structured Data -->
    <script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "EducationalOrganization",
  "name": "ЗДО №8 Ластівка Овруцької міської ради",
  "description": "Дитячий садок для дошкільної освіти дітей віком від 1 до 6 років",
  "address": {
    "@type": "PostalAddress",
    "streetAddress": "вул. Прикордонна",
    "addressLocality": "Овруч",
    "addressRegion": "Житомирська область",
    "addressCountry": "UA"
  },
  "telephone": "",
  "email": "",
  "url": "https://lastivkadev.github.io/Lastivka_zdo_/",
  "openingHours": "Mo-Fr 07:30-18:30"
}
    </script>
    
    <link rel="icon" href="data:image/svg+xml,<svg xmlns=%22http://www.w3.org/2000/svg%22 viewBox=%220 0 100 100%22><text y=%22.9em%22 font-size=%2290%22>👶</text></svg>">
    
    <style>
    /* БАЗОВІ СТИЛІ */
    :root {
        --primary: #4a6fa5;
        --primary-dark: #385d8a;
        --accent: #6dbfb8;
        --light: #ffffff;
        --light-gray: #f5f7fa;
        --dark: #343a40;
        --shadow: 0 5px 15px rgba(0,0,0,0.1);
        --radius: 12px;
        --bg-color: #ffffff;
        --text-color: #343a40;
        --card-bg: #ffffff;
    }

    /* Темна тема */
    .dark-theme {
        --bg-color: #1a1a1a;
        --text-color: #f0f0f0;
        --card-bg: #2a2a2a;
        --light-gray: #333333;
        --dark: #f0f0f0;
        --light: #2a2a2a;
    }
    
    * {
        box-sizing: border-box;
        margin: 0;
        padding: 0;
    }
    
    body {
        font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        background: var(--bg-color);
        color: var(--text-color);
        line-height: 1.6;
        transition: background 0.3s, color 0.3s;
    }
    
    /* HEADER */
    header {
        background: linear-gradient(135deg, var(--primary), var(--primary-dark));
        color: rgb(255, 255, 255);
        padding: 25px 20px;
        text-align: center;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
        position: relative;
    }
    
    header h1 {
        font-size: 2.2rem;
        margin-bottom: 10px;
        font-weight: 700;
    }
    
    header p {
        font-size: 1.1rem;
        opacity: 0.9;
    }
    
    .header-buttons {
        margin-top: 20px;
        display: flex;
        justify-content: center;
        gap: 15px;
        align-items: center;
    }
    
    .header-btn {
        background: rgba(255, 255, 255, 0.2);
        border: 2px solid rgba(255,255,255,0.3);
        color: #ffffff;
        padding: 12px 25px;
        border-radius: 50px;
        font-size: 1rem;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        display: inline-flex;
        align-items: center;
        gap: 10px;
    }
    
    .header-btn:hover {
        background: rgba(255,255,255,0.3);
        transform: translateY(-2px);
    }
    
    /* Профіль користувача в хедері */
    .user-profile-header {
        display: flex;
        align-items: center;
        gap: 15px;
        background: rgba(255, 255, 255, 0.15);
        padding: 10px 20px;
        border-radius: 50px;
        cursor: pointer;
        transition: all 0.3s;
    }
    
    .user-profile-header:hover {
        background: rgba(255, 255, 255, 0.25);
    }
    
    .user-avatar {
        width: 40px;
        height: 40px;
        border-radius: 50%;
        object-fit: cover;
        border: 2px solid white;
    }
    
    .user-name {
        font-weight: 600;
        font-size: 1rem;
    }
    
    /* NAVIGATION */
    nav {
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 10px;
        padding: 20px;
        background: var(--card-bg);
        margin: 20px auto;
        max-width: 1200px;
        border-radius: var(--radius);
        box-shadow: var(--shadow);
        transition: background 0.3s;
    }
    
    .nav-btn {
        background: var(--card-bg);
        border: 2px solid var(--light-gray);
        color: var(--primary);
        padding: 12px 20px;
        border-radius: 50px;
        font-weight: 600;
        cursor: pointer;
        transition: all 0.3s;
        display: flex;
        align-items: center;
        gap: 8px;
    }
    
    .nav-btn:hover {
        background: var(--light-gray);
        transform: translateY(-2px);
    }
    
    .nav-btn.active {
        background: linear-gradient(to right, var(--primary), var(--accent));
        color: rgb(255, 255, 255);
        border-color: transparent;
        box-shadow: 0 4px 10px rgba(74, 111, 165, 0.3);
    }
    
    /* CONTAINER */
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 20px;
    }
    
    /* КАРТКИ */
    .cards-container {
        display: grid;
        gap: 20px;
    }

    .card {
        background: var(--card-bg);
        padding: 25px;
        border-radius: var(--radius);
        box-shadow: var(--shadow);
        border-left: 5px solid var(--accent);
        display: none;
        animation: fadeIn 0.5s ease;
        transition: background 0.3s;
    }

    .card.active {
        display: block;
    }

    @keyframes fadeIn {
        from { opacity: 0; transform: translateY(10px); }
        to { opacity: 1; transform: translateY(0); }
    }

    .card h2 {
        color: var(--primary);
        margin-bottom: 15px;
        font-size: 1.5rem;
    }

    .info-box {
        background: var(--light);
        padding: 15px;
        border-radius: 8px;
        margin-top: 15px;
        transition: background 0.3s;
    }

    /* ПОСИЛАННЯ */
    .drive-link {
        display: inline-block;
        background: linear-gradient(to right, var(--primary), var(--primary-dark));
        color: rgb(255, 255, 255);
        padding: 12px 20px;
        border-radius: 50px;
        text-decoration: none;
        font-weight: 600;
        margin-top: 10px;
        transition: all 0.3s;
        border: 2px solid transparent;
    }

    .drive-link:hover {
        transform: translateY(-2px);
        box-shadow: 0 5px 15px rgba(74, 111, 165, 0.3);
    }

    .groups-grid {
        display: grid;
        grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
        gap: 10px;
        margin-top: 15px;
    }

    .group-link {
        background: var(--card-bg);
        border: 2px solid var(--light-gray);
        padding: 12px;
        border-radius: 8px;
        text-decoration: none;
        color: var(--primary);
        font-weight: 600;
        text-align: center;
        transition: all 0.3s;
    }

    .group-link:hover {
        background: var(--light-gray);
        transform: translateY(-2px);
    }
    
    /* МОДАЛЬНЕ ВІКНО */
    .modal {
        display: none;
        position: fixed;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.7);
        z-index: 1000;
        justify-content: center;
        align-items: center;
        backdrop-filter: blur(5px);
    }

    .modal-content {
        background: var(--card-bg);
        padding: 30px;
        border-radius: var(--radius);
        width: 90%;
        max-width: 400px;
        position: relative;
        box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
        animation: modalAppear 0.3s ease;
        transition: background 0.3s;
    }

    @keyframes modalAppear {
        from {
            opacity: 0;
            transform: translateY(-20px) scale(0.95);
        }
        to {
            opacity: 1;
            transform: translateY(0) scale(1);
        }
    }

    .modal-close {
        position: absolute;
        top: 15px;
        right: 15px;
        background: none;
        border: none;
        font-size: 24px;
        cursor: pointer;
        color: var(--text-color);
        transition: color 0.3s;
    }

    .modal-close:hover {
        color: var(--primary);
    }

    .modal h3 {
        color: var(--primary);
        margin-bottom: 20px;
        text-align: center;
    }

    .modal-tabs {
        display: flex;
        gap: 10px;
        margin-bottom: 20px;
        border-bottom: 2px solid var(--light-gray);
        padding-bottom: 10px;
    }

    .modal-tab {
        background: none;
        border: none;
        padding: 10px 20px;
        font-weight: 600;
        color: var(--text-color);
        cursor: pointer;
        border-radius: 5px;
        transition: all 0.3s;
        flex: 1;
        text-align: center;
    }

    .modal-tab.active {
        background: var(--primary);
        color: white;
    }

    .modal-input {
        width: 100%;
        padding: 12px;
        margin: 10px 0;
        border: 2px solid var(--light-gray);
        border-radius: 8px;
        font-size: 1rem;
        background: var(--light);
        color: var(--text-color);
        transition: all 0.3s;
    }

    .modal-input:focus {
        outline: none;
        border-color: var(--accent);
    }

    .modal-btn {
        width: 100%;
        padding: 12px;
        background: linear-gradient(to right, var(--primary), var(--primary-dark));
        color: white;
        border: none;
        border-radius: 8px;
        font-size: 1rem;
        font-weight: 600;
        cursor: pointer;
        margin-top: 10px;
        transition: all 0.3s;
    }

    .modal-btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 5px 15px rgba(74, 111, 165, 0.3);
    }

    .demo-info {
        margin-top: 15px;
        padding: 15px;
        background: var(--light);
        border-radius: 8px;
        font-size: 0.9rem;
        color: var(--text-color);
        opacity: 0.8;
        transition: background 0.3s;
    }

    /* Вікно профілю */
    .profile-dropdown {
        display: none;
        position: absolute;
        top: 100%;
        right: 20px;
        background: var(--card-bg);
        border-radius: var(--radius);
        box-shadow: var(--shadow);
        min-width: 250px;
        z-index: 100;
        margin-top: 10px;
        animation: dropdownAppear 0.3s ease;
        border: 1px solid var(--light-gray);
    }

    @keyframes dropdownAppear {
        from {
            opacity: 0;
            transform: translateY(-10px);
        }
        to {
            opacity: 1;
            transform: translateY(0);
        }
    }

    .profile-header {
        padding: 20px;
        display: flex;
        align-items: center;
        gap: 15px;
        border-bottom: 1px solid var(--light-gray);
    }

    .profile-avatar-large {
        width: 60px;
        height: 60px;
        border-radius: 50%;
        object-fit: cover;
        border: 3px solid var(--primary);
    }

    .profile-info {
        flex: 1;
    }

    .profile-name {
        font-weight: 600;
        font-size: 1.1rem;
        color: var(--text-color);
    }

    .profile-email {
        font-size: 0.9rem;
        opacity: 0.8;
        color: var(--text-color);
    }

    .profile-menu {
        padding: 10px 0;
    }

    .profile-menu-item {
        display: flex;
        align-items: center;
        gap: 10px;
        padding: 12px 20px;
        color: var(--text-color);
        text-decoration: none;
        cursor: pointer;
        transition: all 0.3s;
        border: none;
        background: none;
        width: 100%;
        text-align: left;
        font-size: 1rem;
    }

    .profile-menu-item:hover {
        background: var(--light-gray);
    }

    .theme-switch {
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 12px 20px;
        color: var(--text-color);
    }

    .theme-toggle {
        position: relative;
        width: 50px;
        height: 26px;
        background: var(--light-gray);
        border-radius: 13px;
        cursor: pointer;
    }

    .theme-toggle::after {
        content: '';
        position: absolute;
        top: 3px;
        left: 3px;
        width: 20px;
        height: 20px;
        background: var(--primary);
        border-radius: 50%;
        transition: transform 0.3s;
    }

    .dark-theme .theme-toggle::after {
        transform: translateX(24px);
    }

    .avatar-upload {
        position: relative;
        display: inline-block;
        cursor: pointer;
    }

    .avatar-upload input[type="file"] {
        display: none;
    }

    .avatar-overlay {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: rgba(0, 0, 0, 0.5);
        border-radius: 50%;
        display: flex;
        align-items: center;
        justify-content: center;
        opacity: 0;
        transition: opacity 0.3s;
        color: white;
        font-size: 12px;
        text-align: center;
        padding: 5px;
    }

    .avatar-upload:hover .avatar-overlay {
        opacity: 1;
    }

    /* Індикатор завантаження */
    .loading {
        display: inline-block;
        width: 20px;
        height: 20px;
        border: 3px solid rgba(255,255,255,.3);
        border-radius: 50%;
        border-top-color: #fff;
        animation: spin 1s ease-in-out infinite;
    }

    @keyframes spin {
        to { transform: rotate(360deg); }
    }

    /* FOOTER */
    footer {
        text-align: center;
        padding: 30px 20px;
        background: var(--dark);
        color: white;
        margin-top: 40px;
        transition: background 0.3s;
    }

    .footer-sub {
        opacity: 0.8;
        font-size: 0.9rem;
        margin-top: 5px;
    }

    /* RESPONSIVE */
    @media (max-width: 768px) {
        nav {
            flex-direction: column;
            align-items: center;
        }
        
        .nav-btn {
            width: 100%;
            max-width: 300px;
            justify-content: center;
        }
        
        .groups-grid {
            grid-template-columns: 1fr 1fr;
        }
        
        .container {
            padding: 15px;
        }
        
        .card {
            padding: 20px;
        }
        
        .header-buttons {
            flex-direction: column;
            align-items: center;
        }
        
        .user-profile-header {
            width: 100%;
            justify-content: center;
        }
        
        .profile-dropdown {
            right: 10px;
            left: 10px;
            min-width: auto;
        }
    }

    @media (max-width: 480px) {
        .groups-grid {
            grid-template-columns: 1fr;
        }
        
        header h1 {
            font-size: 1.8rem;
        }
        
        .header-btn {
            padding: 10px 20px;
            font-size: 0.9rem;
        }
    }
    </style>
</head>
<body>

<header>
    <h1>Овруцький ЗДО №8 «Ластівка» Овруцької міської ради</h1>
    <p>Офіційний сайт дитячого садка</p>
    <div class="header-buttons">
        <button class="header-btn" id="loginBtn" onclick="openAuthModal()">
            <span>🔐</span> Увійти / Зареєструватися
        </button>
        <div class="user-profile-header" id="userProfileBtn" style="display: none;" onclick="toggleProfileDropdown()">
            <img src="" alt="Аватар" class="user-avatar" id="headerAvatar">
            <span class="user-name" id="headerUserName"></span>
        </div>
    </div>
</header>

<!-- Випадаюче меню профілю -->
<div class="profile-dropdown" id="profileDropdown">
    <div class="profile-header">
        <div class="avatar-upload">
            <img src="" alt="Аватар" class="profile-avatar-large" id="profileAvatar">
            <div class="avatar-overlay">
                Змінити<br>аватар
                <input type="file" id="avatarInput" accept="image/*" onchange="uploadAvatar(event)">
            </div>
        </div>
        <div class="profile-info">
            <div class="profile-name" id="profileUserName"></div>
            <div class="profile-email" id="profileUserEmail"></div>
        </div>
    </div>
    <div class="profile-menu">
        <button class="profile-menu-item" onclick="openEditProfileModal()">
            <span>✏️</span> Змінити ім'я
        </button>
        <button class="profile-menu-item" onclick="openAvatarModal()">
            <span>🖼️</span> Змінити аватар
        </button>
        <div class="theme-switch">
            <span>🌓</span> Темна тема
            <div class="theme-toggle" onclick="toggleTheme()"></div>
        </div>
        <button class="profile-menu-item" onclick="logout()">
            <span>🚪</span> Вийти
        </button>
    </div>
</div>

<nav>
    <button class="nav-btn active" onclick="showTab('home')">🏠 Головна</button>
    <button class="nav-btn" onclick="showTab('news')">📰 Новини</button>
    <button class="nav-btn" onclick="showTab('album')">📸 Фото</button>
    <button class="nav-btn" onclick="showTab('groups')">👨‍👩‍👧‍👦 Групи</button>
    <button class="nav-btn" onclick="showTab('schedule')">📅 Розклад</button>
    <button class="nav-btn" onclick="showTab('collective')">👩‍🏫 Педколектив</button>
    <button class="nav-btn" onclick="showTab('inclusive')">❤️ Інклюзія</button>
    <button class="nav-btn" onclick="showTab('statut')">📋 Статут</button>
    <button class="nav-btn" onclick="showTab('orders')">📄 Накази</button>
</nav>

<div class="container">
    <div class="cards-container">
        <!-- ГОЛОВНА -->
        <div id="home" class="card active">
            <h2>🏠 Ласкаво просимо!</h2>
            <p>Офіційний сайт Овруцький ЗДО №8 «Ластівка» Овруцької міської ради— місце, де кожна дитина отримує турботу, любов та якісну дошкільну освіту.</p>
            <p><strong>Наша місія:</strong> створення безпечного та комфортного середовища для гармонійного розвитку дітей віком від 1 до 6 років.</p>
            <div class="info-box">
                <p><strong>📍 Адреса:</strong> вул. Прикордонна</p>
            </div>
        </div>

        <!-- НОВИНИ -->
        <div id="news" class="card">
            <h2>📰 Новини та оголошення</h2>
            <p>Актуальні новини та важлива інформація для батьків:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1zooffQ541chkyuKTUul2nkPjJDwirvxQ" target="_blank">
                📁 Новини нашого садочка
            </a>
        </div>

        <!-- ФОТОАЛЬБОМ -->
        <div id="album" class="card">
            <h2>📸 Фотоальбом нашого садочка</h2>
            <p>Фотографії з життя нашого садочка:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1IknDuijQtf-RrgZ8PtK89K1W2_tWz6xU" target="_blank">
                📁 Фотоальбом
            </a>
        </div>

        <!-- ГРУПИ -->
        <div id="groups" class="card">
            <h2>👨‍👩‍👧‍👦 Групи садочка</h2>
            <p>Оберіть групу для перегляду матеріалів:</p>
            <div class="groups-grid">
                <a class="group-link" href="https://drive.google.com/drive/folders/1JGMSOMT_J2t3BaH-gb9zfTsBa0Mwcit_" target="_blank">🍯 Бджілки</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1x4hdq03XGAvSasfasuUZDnglTzIGeAtl" target="_blank">🌈 Веселка</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1NniCYxUD-PQG7C_QRuWc7xw02BMgdagk" target="_blank">⭐ Зірочки</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1ILclmWrIcnjUO5A0inVl1lFKYr-M0KZ2" target="_blank">💧 Краплинки</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1_88DhBgMjTTY9Bnxh-HFlhyIHROHkx5B" target="_blank">🔍 Пізнайко</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1IaHJfVHh_g9W55Yc1ZIeGVPBQqsZxdAG" target="_blank">☀️ Сонечко</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/1cjb4QtNFRAcVbNB62YaHsp0n8L4r8wzg" target="_blank">🌻 Соняшник</a>
                <a class="group-link" href="https://drive.google.com/drive/folders/16wVHEkqukh9DEyDiaW_QqjnBCH_aWxDn" target="_blank">❓ Чомусики</a>
            </div>
        </div>

        <!-- РОЗКЛАД -->
        <div id="schedule" class="card">
            <h2>📅 Розклад занять</h2>
            <p>Щоденний розклад та режим дня нашого садочка:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1WiA4RmGSrRH29CbrXg14df5JtuYd6TeJ" target="_blank">
                📁 Розклад
            </a>
        </div>

        <!-- ПЕДКОЛЕКТИВ -->
        <div id="collective" class="card">
            <h2>👩‍🏫 Педагогічний колектив</h2>
            <p>Інформація про наших педагогів:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1Fwu64LsLkIeybCPFTni-_5DgFPvtBMp7" target="_blank">
                📁 Документи педколективу
            </a>
        </div>

        <!-- ІНКЛЮЗІЯ -->
        <div id="inclusive" class="card">
            <h2>❤️ Інклюзивна освіта</h2>
            <p>Документи з інклюзивної освіта нашого садочка:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/10Q-sd76LpOaqeMxjuyNNYUhFwHMz3lRK" target="_blank">
                📁 Документи з інклюзії
            </a>
        </div>

        <!-- СТАТУТ -->
        <div id="statut" class="card">
            <h2>📋 Статут</h2>
            <p>Офіційний статут садочка:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1fJZhnr-yTZ5Uecl4jdnkuSEDhleSx0dz" target="_blank">
                📁 Статут
            </a>
        </div>

        <!-- НАКАЗИ -->
        <div id="orders" class="card">
            <h2>📄 Накази</h2>
            <p>Накази:</p>
            <a class="drive-link" href="https://drive.google.com/drive/folders/1ANR6bzU3viTLAgj2NSY-n6JfDlzs_9mS" target="_blank">
                📁 Накази нашого садочка
            </a>
        </div>
    </div>
</div>

<!-- МОДАЛЬНЕ ВІКНО АВТОРИЗАЦІЇ -->
<div id="authModal" class="modal">
    <div class="modal-content">
        <button class="modal-close" onclick="closeAuthModal()">×</button>
        <h3>🔐 Увійти / Зареєструватися</h3>
        <div class="modal-tabs">
            <button class="modal-tab active" onclick="switchAuthTab('login')">Вхід</button>
            <button class="modal-tab" onclick="switchAuthTab('register')">Реєстрація</button>
        </div>
        <div id="loginForm">
            <input type="email" class="modal-input" id="loginEmail" placeholder="Email">
            <input type="password" class="modal-input" id="loginPassword" placeholder="Пароль">
            <button class="modal-btn" id="loginButton" onclick="handleLogin()">
                <span id="loginText">Увійти</span>
                <span id="loginLoading" class="loading" style="display: none;"></span>
            </button>
        </div>
        <div id="registerForm" style="display: none;">
            <input type="text" class="modal-input" id="registerName" placeholder="Ваше ім'я">
            <input type="email" class="modal-input" id="registerEmail" placeholder="Email">
            <input type="password" class="modal-input" id="registerPassword" placeholder="Пароль">
            <input type="password" class="modal-input" id="registerConfirmPassword" placeholder="Підтвердіть пароль">
            <button class="modal-btn" id="registerButton" onclick="handleRegister()">
                <span id="registerText">Зареєструватися</span>
                <span id="registerLoading" class="loading" style="display: none;"></span>
            </button>
        </div>
        <div class="demo-info">
            <p><strong></strong></p>
            <p></p>
            <p></p>
        </div>
    </div>
</div>

<!-- МОДАЛЬНЕ ВІКНО РЕДАГУВАННЯ ПРОФІЛЮ -->
<div id="editProfileModal" class="modal">
    <div class="modal-content">
        <button class="modal-close" onclick="closeEditProfileModal()">×</button>
        <h3>✏️ Змінити ім'я</h3>
        <input type="text" class="modal-input" id="editProfileName" placeholder="Нове ім'я">
        <button class="modal-btn" id="saveProfileButton" onclick="saveProfileName()">
            <span id="saveProfileText">Зберегти зміни</span>
            <span id="saveProfileLoading" class="loading" style="display: none;"></span>
        </button>
    </div>
</div>

<!-- МОДАЛЬНЕ ВІКНО ЗМІНИ АВАТАРА -->
<div id="avatarModal" class="modal">
    <div class="modal-content">
        <button class="modal-close" onclick="closeAvatarModal()">×</button>
        <h3>🖼️ Змінити аватар</h3>
        <div style="text-align: center; margin: 20px 0;">
            <div class="avatar-upload" style="display: inline-block;">
                <img src="" alt="Аватар" class="profile-avatar-large" id="modalAvatarPreview" style="width: 120px; height: 120px;">
                <div class="avatar-overlay" style="width: 120px; height: 120px;">
                    Вибрати файл
                </div>
                <input type="file" id="modalAvatarInput" accept="image/*" onchange="previewAvatar(event)">
            </div>
        </div>
        <button class="modal-btn" id="saveAvatarButton" onclick="saveAvatar()">
            <span id="saveAvatarText">Зберегти аватар</span>
            <span id="saveAvatarLoading" class="loading" style="display: none;"></span>
        </button>
    </div>
</div>

<footer>
    <p>© 2026 Овруцький ЗДО №8 Ластівка Овруцької міської ради.</p>
    <p class="footer-sub">Офіційний сайт садочку</p>
</footer>

<script>
// ========== FIREBASE CONFIGURATION ==========
const firebaseConfig = {
    apiKey: "AIzaSyD0tJbZoYdKOCHQNXYwd3_ATevH0tAjC-8",
    authDomain: "zdo-lastivka.firebaseapp.com",
    projectId: "zdo-lastivka",
    storageBucket: "zdo-lastivka.firebasestorage.app",
    messagingSenderId: "920607978182",
    appId: "1:920607978182:web:1e035a72ed1c146f7a1dc7"
};

// Initialize Firebase
firebase.initializeApp(firebaseConfig);
const auth = firebase.auth();
const db = firebase.firestore();
const storage = firebase.storage();

// ========== ГЛОБАЛЬНІ ЗМІННІ ==========
let currentUser = null;
let isDarkTheme = false;
let avatarFile = null;

// ========== ФУНКЦІЇ ДЛЯ COOKIES (тільки для теми) ==========
function setCookie(name, value, days) {
    let expires = "";
    if (days) {
        const date = new Date();
        date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
        expires = "; expires=" + date.toUTCString();
    }
    document.cookie = name + "=" + (value || "") + expires + "; path=/";
}

function getCookie(name) {
    const nameEQ = name + "=";
    const ca = document.cookie.split(';');
    for(let i = 0; i < ca.length; i++) {
        let c = ca[i];
        while (c.charAt(0) === ' ') c = c.substring(1, c.length);
        if (c.indexOf(nameEQ) === 0) return c.substring(nameEQ.length, c.length);
    }
    return null;
}

function eraseCookie(name) {   
    document.cookie = name + '=; Max-Age=-99999999; path=/';
}

// ========== ФУНКЦІЇ ДЛЯ ТЕМИ ==========
function saveThemePreference(isDark) {
    setCookie('lastivka_theme', isDark ? 'dark' : 'light', 365);
}

function getThemePreference() {
    const theme = getCookie('lastivka_theme');
    return theme === 'dark';
}

function applyTheme(isDark) {
    if (isDark) {
        document.body.classList.add('dark-theme');
    } else {
        document.body.classList.remove('dark-theme');
    }
    window.isDarkTheme = isDark;
    saveThemePreference(isDark);
}

function toggleTheme() {
    const newTheme = !window.isDarkTheme;
    applyTheme(newTheme);
}

// ========== ОСНОВНІ ФУНКЦІЇ ==========
function showTab(tabId) {
    document.querySelectorAll('.card').forEach(card => {
        card.classList.remove('active');
    });
    
    document.querySelectorAll('.nav-btn').forEach(btn => {
        btn.classList.remove('active');
    });
    
    const selectedCard = document.getElementById(tabId);
    if (selectedCard) {
        selectedCard.classList.add('active');
    }
    
    const activeButton = document.querySelector(`[onclick="showTab('${tabId}')"]`);
    if (activeButton) {
        activeButton.classList.add('active');
    }
    
    window.scrollTo({ top: 0, behavior: 'smooth' });
}

// ========== ФУНКЦІЇ ДЛЯ МОДАЛЬНИХ ВІКОН ==========
function openAuthModal() {
    document.getElementById('authModal').style.display = 'flex';
    document.getElementById('loginEmail').focus();
    switchAuthTab('login');
}

function closeAuthModal() {
    document.getElementById('authModal').style.display = 'none';
    document.getElementById('loginEmail').value = '';
    document.getElementById('loginPassword').value = '';
    document.getElementById('registerName').value = '';
    document.getElementById('registerEmail').value = '';
    document.getElementById('registerPassword').value = '';
    document.getElementById('registerConfirmPassword').value = '';
}

function switchAuthTab(tab) {
    const loginForm = document.getElementById('loginForm');
    const registerForm = document.getElementById('registerForm');
    const loginTab = document.querySelector('[onclick="switchAuthTab(\'login\')"]');
    const registerTab = document.querySelector('[onclick="switchAuthTab(\'register\')"]');
    
    if (tab === 'login') {
        loginForm.style.display = 'block';
        registerForm.style.display = 'none';
        loginTab.classList.add('active');
        registerTab.classList.remove('active');
    } else {
        loginForm.style.display = 'none';
        registerForm.style.display = 'block';
        loginTab.classList.remove('active');
        registerTab.classList.add('active');
    }
}

function openEditProfileModal() {
    if (!window.currentUser) return;
    
    document.getElementById('editProfileModal').style.display = 'flex';
    document.getElementById('editProfileName').value = window.currentUser.displayName || '';
    document.getElementById('editProfileName').focus();
    closeProfileDropdown();
}

function closeEditProfileModal() {
    document.getElementById('editProfileModal').style.display = 'none';
}

function openAvatarModal() {
    if (!window.currentUser) return;
    
    const avatarImg = document.getElementById('modalAvatarPreview');
    avatarImg.src = window.currentUser.photoURL || getDefaultAvatar();
    
    document.getElementById('avatarModal').style.display = 'flex';
    closeProfileDropdown();
}

function closeAvatarModal() {
    document.getElementById('avatarModal').style.display = 'none';
    document.getElementById('modalAvatarInput').value = '';
    window.avatarFile = null;
}

// ========== FIREBASE АВТОРИЗАЦІЯ ==========
async function handleLogin() {
    const email = document.getElementById('loginEmail').value.trim();
    const password = document.getElementById('loginPassword').value.trim();
    
    if (!email || !password) {
        alert('❌ Будь ласка, заповніть всі поля');
        return;
    }
    
    // Показуємо індикатор завантаження
    const loginBtn = document.getElementById('loginButton');
    const loginText = document.getElementById('loginText');
    const loginLoading = document.getElementById('loginLoading');
    
    loginText.style.display = 'none';
    loginLoading.style.display = 'inline-block';
    loginBtn.disabled = true;
    
    try {
        const userCredential = await auth.signInWithEmailAndPassword(email, password);
        const user = userCredential.user;
        
        // Отримуємо додаткові дані користувача з Firestore
        const userDoc = await db.collection('users').doc(user.uid).get();
        
        if (userDoc.exists) {
            const userData = userDoc.data();
            window.currentUser = {
                uid: user.uid,
                email: user.email,
                displayName: user.displayName || userData.displayName || 'Користувач',
                photoURL: user.photoURL || userData.photoURL || null,
                role: userData.role || 'user',
                createdAt: userData.createdAt || user.metadata.creationTime
            };
        } else {
            window.currentUser = {
                uid: user.uid,
                email: user.email,
                displayName: user.displayName || 'Користувач',
                photoURL: user.photoURL || null,
                role: 'user',
                createdAt: user.metadata.creationTime
            };
        }
        
        updateUIAfterLogin();
        closeAuthModal();
        
        alert(`✅ Вітаємо, ${window.currentUser.displayName}! Успішний вхід в систему.`);
        
    } catch (error) {
        console.error('Помилка входу:', error);
        
        let errorMessage = '❌ Помилка входу. ';
        switch (error.code) {
            case 'auth/user-not-found':
                errorMessage += 'Користувача не знайдено.';
                break;
            case 'auth/wrong-password':
                errorMessage += 'Невірний пароль.';
                break;
            case 'auth/invalid-email':
                errorMessage += 'Невірний формат email.';
                break;
            case 'auth/user-disabled':
                errorMessage += 'Користувача вимкнено.';
                break;
            default:
                errorMessage += 'Спробуйте ще раз.';
        }
        
        alert(errorMessage);
    } finally {
        // Ховаємо індикатор завантаження
        loginText.style.display = 'inline';
        loginLoading.style.display = 'none';
        loginBtn.disabled = false;
    }
}

async function handleRegister() {
    const name = document.getElementById('registerName').value.trim();
    const email = document.getElementById('registerEmail').value.trim();
    const password = document.getElementById('registerPassword').value.trim();
    const confirmPassword = document.getElementById('registerConfirmPassword').value.trim();
    
    if (!name || !email || !password || !confirmPassword) {
        alert('❌ Будь ласка, заповніть всі поля');
        return;
    }
    
    if (password !== confirmPassword) {
        alert('❌ Паролі не співпадають');
        return;
    }
    
    if (password.length < 6) {
        alert('❌ Пароль має містити щонайменше 6 символів');
        return;
    }
    
    // Перевірка email
    const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/;
    if (!emailRegex.test(email)) {
        alert('❌ Будь ласка, введіть коректний email');
        return;
    }
    
    // Показуємо індикатор завантаження
    const registerBtn = document.getElementById('registerButton');
    const registerText = document.getElementById('registerText');
    const registerLoading = document.getElementById('registerLoading');
    
    registerText.style.display = 'none';
    registerLoading.style.display = 'inline-block';
    registerBtn.disabled = true;
    
    try {
        // Створюємо користувача в Firebase Authentication
        const userCredential = await auth.createUserWithEmailAndPassword(email, password);
        const user = userCredential.user;
        
        // Оновлюємо відображуване ім'я
        await user.updateProfile({
            displayName: name
        });
        
        // Зберігаємо додаткові дані в Firestore
        await db.collection('users').doc(user.uid).set({
            uid: user.uid,
            email: email,
            displayName: name,
            photoURL: null,
            role: 'user',
            createdAt: firebase.firestore.FieldValue.serverTimestamp(),
            updatedAt: firebase.firestore.FieldValue.serverTimestamp()
        });
        
        window.currentUser = {
            uid: user.uid,
            email: user.email,
            displayName: name,
            photoURL: null,
            role: 'user',
            createdAt: new Date().toISOString()
        };
        
        updateUIAfterLogin();
        closeAuthModal();
        
        alert(`✅ Вітаємо, ${name}! Реєстрація пройшла успішно.`);
        
    } catch (error) {
        console.error('Помилка реєстрації:', error);
        
        let errorMessage = '❌ Помилка реєстрації. ';
        switch (error.code) {
            case 'auth/email-already-in-use':
                errorMessage += 'Цей email вже використовується.';
                break;
            case 'auth/invalid-email':
                errorMessage += 'Невірний формат email.';
                break;
            case 'auth/operation-not-allowed':
                errorMessage += 'Реєстрація вимкнена.';
                break;
            case 'auth/weak-password':
                errorMessage += 'Пароль занадто слабкий.';
                break;
            default:
                errorMessage += 'Спробуйте ще раз.';
        }
        
        alert(errorMessage);
    } finally {
        // Ховаємо індикатор завантаження
        registerText.style.display = 'inline';
        registerLoading.style.display = 'none';
        registerBtn.disabled = false;
    }
}

// ========== ФУНКЦІЇ ПРОФІЛЮ ==========
function updateUIAfterLogin() {
    if (!window.currentUser) return;
    
    document.getElementById('loginBtn').style.display = 'none';
    document.getElementById('userProfileBtn').style.display = 'flex';
    
    updateProfileUI();
}

function updateProfileUI() {
    if (!window.currentUser) return;
    
    const user = window.currentUser;
    const defaultAvatar = getDefaultAvatar();
    
    // Оновлюємо хедер
    document.getElementById('headerAvatar').src = user.photoURL || defaultAvatar;
    document.getElementById('headerUserName').textContent = user.displayName;
    
    // Оновлюємо випадаюче меню
    document.getElementById('profileAvatar').src = user.photoURL || defaultAvatar;
    document.getElementById('profileUserName').textContent = user.displayName;
    document.getElementById('profileUserEmail').textContent = user.email;
}

function getDefaultAvatar() {
    const colors = ['#4a6fa5', '#6dbfb8', '#ff9a76', '#ffd166', '#06d6a0'];
    const color = colors[Math.floor(Math.random() * colors.length)];
    
    const canvas = document.createElement('canvas');
    canvas.width = 100;
    canvas.height = 100;
    const ctx = canvas.getContext('2d');
    
    // Фон
    ctx.fillStyle = color;
    ctx.fillRect(0, 0, 100, 100);
    
    // Текст з ініціалами
    if (window.currentUser && window.currentUser.displayName) {
        const initials = window.currentUser.displayName.split(' ').map(n => n[0]).join('').toUpperCase().substring(0, 2);
        ctx.fillStyle = 'white';
        ctx.font = 'bold 40px Arial';
        ctx.textAlign = 'center';
        ctx.textBaseline = 'middle';
        ctx.fillText(initials, 50, 50);
    }
    
    return canvas.toDataURL();
}

function toggleProfileDropdown() {
    const dropdown = document.getElementById('profileDropdown');
    if (dropdown.style.display === 'block') {
        dropdown.style.display = 'none';
    } else {
        dropdown.style.display = 'block';
        updateProfileUI();
    }
}

function closeProfileDropdown() {
    document.getElementById('profileDropdown').style.display = 'none';
}

async function saveProfileName() {
    const newName = document.getElementById('editProfileName').value.trim();
    
    if (!newName) {
        alert('❌ Будь ласка, введіть ім\'я');
        return;
    }
    
    // Показуємо індикатор завантаження
    const saveBtn = document.getElementById('saveProfileButton');
    const saveText = document.getElementById('saveProfileText');
    const saveLoading = document.getElementById('saveProfileLoading');
    
    saveText.style.display = 'none';
    saveLoading.style.display = 'inline-block';
    saveBtn.disabled = true;
    
    try {
        // Оновлюємо в Firebase Authentication
        const user = auth.currentUser;
        if (user) {
            await user.updateProfile({
                displayName: newName
            });
        }
        
        // Оновлюємо в Firestore
        await db.collection('users').doc(window.currentUser.uid).update({
            displayName: newName,
            updatedAt: firebase.firestore.FieldValue.serverTimestamp()
        });
        
        // Оновлюємо локальні дані
        window.currentUser.displayName = newName;
        
        // Оновлюємо UI
        updateProfileUI();
        closeEditProfileModal();
        
        alert('✅ Ім\'я успішно змінено!');
        
    } catch (error) {
        console.error('Помилка зміни імені:', error);
        alert('❌ Помилка при зміні імені. Спробуйте ще раз.');
    } finally {
        // Ховаємо індикатор завантаження
        saveText.style.display = 'inline';
        saveLoading.style.display = 'none';
        saveBtn.disabled = false;
    }
}

function previewAvatar(event) {
    const file = event.target.files[0];
    if (!file) return;
    
    if (!file.type.match('image.*')) {
        alert('❌ Будь ласка, виберіть зображення');
        return;
    }
    
    if (file.size > 5 * 1024 * 1024) { // 5MB
        alert('❌ Розмір файлу не повинен перевищувати 5MB');
        return;
    }
    
    window.avatarFile = file;
    
    const reader = new FileReader();
    reader.onload = function(e) {
        document.getElementById('modalAvatarPreview').src = e.target.result;
    };
    reader.readAsDataURL(file);
}

async function saveAvatar() {
    if (!window.avatarFile) {
        alert('❌ Будь ласка, виберіть зображення');
        return;
    }
    
    // Показуємо індикатор завантаження
    const saveBtn = document.getElementById('saveAvatarButton');
    const saveText = document.getElementById('saveAvatarText');
    const saveLoading = document.getElementById('saveAvatarLoading');
    
    saveText.style.display = 'none';
    saveLoading.style.display = 'inline-block';
    saveBtn.disabled = true;
    
    try {
        const user = auth.currentUser;
        if (!user) {
            throw new Error('Користувач не авторизований');
        }
        
        // Завантажуємо аватар в Firebase Storage
        const storageRef = storage.ref();
        const avatarRef = storageRef.child(`avatars/${user.uid}/${Date.now()}_${window.avatarFile.name}`);
        const snapshot = await avatarRef.put(window.avatarFile);
        
        // Отримуємо URL завантаженого файлу
        const downloadURL = await snapshot.ref.getDownloadURL();
        
        // Оновлюємо в Firebase Authentication
        await user.updateProfile({
            photoURL: downloadURL
        });
        
        // Оновлюємо в Firestore
        await db.collection('users').doc(user.uid).update({
            photoURL: downloadURL,
            updatedAt: firebase.firestore.FieldValue.serverTimestamp()
        });
        
        // Оновлюємо локальні дані
        window.currentUser.photoURL = downloadURL;
        
        // Оновлюємо UI
        updateProfileUI();
        closeAvatarModal();
        
        alert('✅ Аватар успішно змінено!');
        
    } catch (error) {
        console.error('Помилка завантаження аватара:', error);
        alert('❌ Помилка при завантаженні аватара. Спробуйте ще раз.');
    } finally {
        // Ховаємо індикатор завантаження
        saveText.style.display = 'inline';
        saveLoading.style.display = 'none';
        saveBtn.disabled = false;
        window.avatarFile = null;
    }
}

function uploadAvatar(event) {
    const file = event.target.files[0];
    if (!file) return;
    
    if (!file.type.match('image.*')) {
        alert('❌ Будь ласка, виберіть зображення');
        return;
    }
    
    if (file.size > 5 * 1024 * 1024) { // 5MB
        alert('❌ Розмір файлу не повинен перевищувати 5MB');
        return;
    }
    
    // Безпосереднє завантаження
    saveAvatarFromFile(file);
}

async function saveAvatarFromFile(file) {
    try {
        const user = auth.currentUser;
        if (!user) {
            throw new Error('Користувач не авторизований');
        }
        
        // Завантажуємо аватар в Firebase Storage
        const storageRef = storage.ref();
        const avatarRef = storageRef.child(`avatars/${user.uid}/${Date.now()}_${file.name}`);
        const snapshot = await avatarRef.put(file);
        
        // Отримуємо URL завантаженого файлу
        const downloadURL = await snapshot.ref.getDownloadURL();
        
        // Оновлюємо в Firebase Authentication
        await user.updateProfile({
            photoURL: downloadURL
        });
        
        // Оновлюємо в Firestore
        await db.collection('users').doc(user.uid).update({
            photoURL: downloadURL,
            updatedAt: firebase.firestore.FieldValue.serverTimestamp()
        });
        
        // Оновлюємо локальні дані
        window.currentUser.photoURL = downloadURL;
        
        // Оновлюємо UI
        updateProfileUI();
        
        alert('✅ Аватар успішно змінено!');
        
    } catch (error) {
        console.error('Помилка завантаження аватара:', error);
        alert('❌ Помилка при завантаженні аватара. Спробуйте ще раз.');
    }
}

async function logout() {
    try {
        await auth.signOut();
        window.currentUser = null;
        
        document.getElementById('loginBtn').style.display = 'inline-flex';
        document.getElementById('userProfileBtn').style.display = 'none';
        document.getElementById('profileDropdown').style.display = 'none';
        
        alert('✅ Ви успішно вийшли з системи');
        
    } catch (error) {
        console.error('Помилка виходу:', error);
        alert('❌ Помилка при виході з системи');
    }
}

// ========== ІНІЦІАЛІЗАЦІЯ ==========
document.addEventListener('DOMContentLoaded', async function() {
    // Застосовуємо збережену тему
    const savedTheme = getThemePreference();
    applyTheme(savedTheme);
    
    // Показуємо першу вкладку
    showTab('home');
    
    // Перевіряємо чи користувач вже авторизований
    auth.onAuthStateChanged(async (user) => {
        if (user) {
            // Отримуємо додаткові дані користувача з Firestore
            const userDoc = await db.collection('users').doc(user.uid).get();
            
            if (userDoc.exists) {
                const userData = userDoc.data();
                window.currentUser = {
                    uid: user.uid,
                    email: user.email,
                    displayName: user.displayName || userData.displayName || 'Користувач',
                    photoURL: user.photoURL || userData.photoURL || null,
                    role: userData.role || 'user',
                    createdAt: userData.createdAt || user.metadata.creationTime
                };
            } else {
                window.currentUser = {
                    uid: user.uid,
                    email: user.email,
                    displayName: user.displayName || 'Користувач',
                    photoURL: user.photoURL || null,
                    role: 'user',
                    createdAt: user.metadata.creationTime
                };
            }
            
            updateUIAfterLogin();
        }
    });
    
    // Закриваємо модальні вікна по кліку поза ними
    document.querySelectorAll('.modal').forEach(modal => {
        modal.addEventListener('click', function(event) {
            if (event.target === this) {
                this.style.display = 'none';
            }
        });
    });
    
    // Закриваємо випадаюче меню по кліку поза ним
    document.addEventListener('click', function(event) {
        const dropdown = document.getElementById('profileDropdown');
        const profileBtn = document.getElementById('userProfileBtn');
        
        if (dropdown && dropdown.style.display === 'block' && 
            !dropdown.contains(event.target) && 
            (!profileBtn || !profileBtn.contains(event.target))) {
            dropdown.style.display = 'none';
        }
    });
    
    // Вхід по Enter
    document.getElementById('loginPassword').addEventListener('keypress', function(event) {
        if (event.key === 'Enter') {
            handleLogin();
        }
    });
    
    document.getElementById('registerConfirmPassword').addEventListener('keypress', function(event) {
        if (event.key === 'Enter') {
            handleRegister();
        }
    });
    
    // Закрити по Escape
    document.addEventListener('keydown', function(event) {
        if (event.key === 'Escape') {
            closeAuthModal();
            closeEditProfileModal();
            closeAvatarModal();
            closeProfileDropdown();
        }
    });
    
    console.log('🚀 Сайт ЗДО «Садочок Ластівка» завантажено!');
    console.log('🔥 Firebase підключено!');
});
</script>
</body>
</html>
