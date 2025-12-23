<!-- ПОЛНЫЙ КОД САЙТА ДЛЯ ЗАГРУЗКИ НА GITHUB PAGES -->
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Saya Coin - Новогодний дилер 2026</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="icon" type="image/x-icon" href="https://img.icons8.com/color/96/000000/bitcoin--v1.png">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }
        
        body {
            background-color: #0a1f2e;
            color: #fff;
            background-image: 
                radial-gradient(circle at 10% 20%, rgba(28, 58, 83, 0.7) 0%, transparent 20%),
                radial-gradient(circle at 90% 80%, rgba(28, 58, 83, 0.7) 0%, transparent 20%),
                url('https://images.unsplash.com/photo-1513151233558-d860c5398176?q=80&w=2070&auto=format&fit=crop');
            background-size: cover;
            background-blend-mode: overlay;
            min-height: 100vh;
            position: relative;
            overflow-x: hidden;
        }
        
        /* Снег */
        .snowflakes {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }
        
        .snowflake {
            position: absolute;
            background-color: white;
            border-radius: 50%;
            opacity: 0.8;
            animation: fall linear infinite;
        }
        
        @keyframes fall {
            to {
                transform: translateY(100vh);
            }
        }
        
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            position: relative;
            z-index: 2;
            background: rgba(10, 31, 46, 0.85);
            min-height: 100vh;
        }
        
        /* Шапка */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px 0;
            border-bottom: 2px solid rgba(255, 255, 255, 0.1);
            margin-bottom: 40px;
            flex-wrap: wrap;
        }
        
        .logo {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo-icon {
            width: 60px;
            height: 60px;
            background: linear-gradient(45deg, #ff9800, #ffeb3b);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            font-weight: bold;
            color: #0a1f2e;
            animation: pulse 2s infinite;
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.05); }
            100% { transform: scale(1); }
        }
        
        .logo-text {
            font-size: 28px;
            font-weight: 800;
            background: linear-gradient(to right, #ff9800, #ffeb3b);
            -webkit-background-clip: text;
            background-clip: text;
            color: transparent;
            text-shadow: 0 2px 5px rgba(0, 0, 0, 0.3);
        }
        
        .logo-subtitle {
            font-size: 14px;
            color: #a3d5ff;
            margin-top: 5px;
        }
        
        .domain-info {
            text-align: right;
            background: rgba(255, 255, 255, 0.1);
            padding: 10px 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.2);
        }
        
        .domain-info .free-badge {
            background: #4CAF50;
            color: white;
            padding: 3px 10px;
            border-radius: 20px;
            font-size: 12px;
            font-weight: bold;
            margin-left: 10px;
        }
        
        /* Обратный отсчет */
        .countdown {
            text-align: center;
            margin-bottom: 50px;
            background: rgba(0, 0, 0, 0.3);
            padding: 30px;
            border-radius: 20px;
            border: 1px solid rgba(255, 215, 0, 0.3);
        }
        
        .countdown h2 {
            font-size: 32px;
            margin-bottom: 20px;
            color: #ffeb3b;
            text-shadow: 0 0 10px rgba(255, 235, 59, 0.5);
        }
        
        .countdown-box {
            display: flex;
            justify-content: center;
            gap: 20px;
            margin-top: 20px;
            flex-wrap: wrap;
        }
        
        .countdown-item {
            background: rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 20px;
            min-width: 100px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
            transition: transform 0.3s;
        }
        
        .countdown-item:hover {
            transform: translateY(-5px);
            border-color: #ff9800;
        }
        
        .countdown-number {
            font-size: 36px;
            font-weight: bold;
            color: #4fc3f7;
            text-shadow: 0 0 10px rgba(79, 195, 247, 0.5);
        }
        
        .countdown-label {
            font-size: 14px;
            color: #a3d5ff;
            margin-top: 5px;
        }
        
        /* Пакеты монет */
        .packages {
            margin-bottom: 60px;
        }
        
        .packages h2 {
            font-size: 32px;
            text-align: center;
            margin-bottom: 30px;
            color: #ffeb3b;
            text-shadow: 0 0 10px rgba(255, 235, 59, 0.5);
            padding: 15px;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 15px;
        }
        
        .package-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 25px;
            margin-top: 30px;
        }
        
        .package-card {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 25px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            transition: all 0.3s;
            position: relative;
            overflow: hidden;
        }
        
        .package-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4);
            border-color: rgba(255, 235, 59, 0.5);
        }
        
        .package-card.popular::before {
            content: 'ПОПУЛЯРНЫЙ';
            position: absolute;
            top: 15px;
            right: -30px;
            background: linear-gradient(45deg, #ff9800, #ff5722);
            color: white;
            padding: 5px 30px;
            font-size: 12px;
            font-weight: bold;
            transform: rotate(45deg);
        }
        
        .package-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .package-price {
            font-size: 24px;
            font-weight: bold;
            color: #4fc3f7;
        }
        
        .package-coins {
            font-size: 20px;
            font-weight: bold;
            color: #ffeb3b;
        }
        
        .package-bonus {
            font-size: 14px;
            color: #81c784;
            margin-top: 5px;
        }
        
        .package-description {
            margin-top: 15px;
            font-size: 14px;
            color: #a3d5ff;
            line-height: 1.5;
            min-height: 60px;
        }
        
        .payment-instruction {
            background: rgba(255, 193, 7, 0.1);
            border: 1px solid rgba(255, 193, 7, 0.3);
            border-radius: 10px;
            padding: 15px;
            margin: 20px 0;
            font-size: 13px;
        }
        
        .payment-instruction h4 {
            color: #ffc107;
            margin-bottom: 10px;
            font-size: 14px;
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .payment-instruction h4 i {
            font-size: 16px;
        }
        
        .payment-instruction ol {
            margin-left: 20px;
            color: #e0e0e0;
        }
        
        .payment-instruction li {
            margin-bottom: 8px;
            line-height: 1.4;
        }
        
        .payment-instruction a {
            color: #4fc3f7;
            text-decoration: none;
            font-weight: bold;
        }
        
        .payment-instruction a:hover {
            text-decoration: underline;
        }
        
        .payment-note {
            background: rgba(244, 67, 54, 0.1);
            border: 1px solid rgba(244, 67, 54, 0.3);
            border-radius: 5px;
            padding: 10px;
            margin-top: 10px;
            font-size: 12px;
            color: #ffab91;
        }
        
        .buy-button {
            display: block;
            width: 100%;
            background: linear-gradient(to right, #ff9800, #ff5722);
            color: white;
            border: none;
            padding: 15px;
            border-radius: 10px;
            font-size: 16px;
            font-weight: bold;
            margin-top: 10px;
            cursor: pointer;
            transition: all 0.3s;
            text-align: center;
            text-decoration: none;
        }
        
        .buy-button:hover {
            background: linear-gradient(to right, #ff5722, #ff9800);
            box-shadow: 0 5px 15px rgba(255, 87, 34, 0.4);
            transform: translateY(-2px);
        }
        
        /* Блок с Telegram */
        .telegram-info {
            background: rgba(0, 136, 204, 0.1);
            border: 1px solid rgba(0, 136, 204, 0.3);
            border-radius: 10px;
            padding: 20px;
            margin: 30px 0;
            text-align: center;
        }
        
        .telegram-info h3 {
            color: #29b6f6;
            margin-bottom: 15px;
            font-size: 22px;
        }
        
        .telegram-info p {
            margin-bottom: 15px;
            line-height: 1.6;
            color: #e0e0e0;
        }
        
        .telegram-button {
            display: inline-flex;
            align-items: center;
            gap: 10px;
            background: #0088cc;
            color: white;
            padding: 12px 25px;
            border-radius: 50px;
            text-decoration: none;
            font-weight: bold;
            font-size: 16px;
            transition: all 0.3s;
        }
        
        .telegram-button:hover {
            background: #0077b5;
            transform: translateY(-3px);
            box-shadow: 0 5px 15px rgba(0, 136, 204, 0.4);
        }
        
        /* График работы */
        .schedule {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 15px;
            padding: 25px;
            margin-top: 40px;
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .schedule h3 {
            font-size: 24px;
            margin-bottom: 15px;
            color: #4fc3f7;
        }
        
        .schedule p {
            font-size: 16px;
            line-height: 1.6;
            color: #a3d5ff;
        }
        
        .schedule .highlight {
            color: #ffeb3b;
            font-weight: bold;
        }
        
        footer {
            text-align: center;
            padding: 30px 0;
            margin-top: 50px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            color: #a3d5ff;
            font-size: 14px;
        }
        
        .free-hosting {
            background: rgba(76, 175, 80, 0.1);
            border: 1px solid rgba(76, 175, 80, 0.3);
            border-radius: 10px;
            padding: 15px;
            margin-top: 20px;
            text-align: center;
        }
        
        .free-hosting h4 {
            color: #4CAF50;
            margin-bottom: 10px;
        }
        
        /* Адаптивность */
        @media (max-width: 768px) {
            header {
                flex-direction: column;
                gap: 15px;
                text-align: center;
            }
            
            .domain-info {
                text-align: center;
            }
            
            .countdown-box {
                gap: 10px;
            }
            
            .countdown-item {
                min-width: 70px;
                padding: 15px 10px;
            }
            
            .countdown-number {
                font-size: 28px;
            }
            
            .package-grid {
                grid-template-columns: 1fr;
            }
        }
        
        /* Анимация новогодних огней */
        @keyframes twinkle {
            0%, 100% { opacity: 0.7; }
            50% { opacity: 1; }
        }
        
        .lights {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 20px;
            z-index: 1;
        }
        
        .light {
            position: absolute;
            width: 10px;
            height: 10px;
            border-radius: 50%;
            animation: twinkle 1.5s infinite;
        }
        
        .light:nth-child(1) { left: 5%; background-color: #ff5252; animation-delay: 0s; }
        .light:nth-child(2) { left: 15%; background-color: #ffeb3b; animation-delay: 0.2s; }
        .light:nth-child(3) { left: 25%; background-color: #4fc3f7; animation-delay: 0.4s; }
        .light:nth-child(4) { left: 35%; background-color: #69f0ae; animation-delay: 0.6s; }
        .light:nth-child(5) { left: 45%; background-color: #ff9800; animation-delay: 0.8s; }
        .light:nth-child(6) { left: 55%; background-color: #e040fb; animation-delay: 1s; }
        .light:nth-child(7) { left: 65%; background-color: #ff5252; animation-delay: 1.2s; }
        .light:nth-child(8) { left: 75%; background-color: #ffeb3b; animation-delay: 1.4s; }
        .light:nth-child(9) { left: 85%; background-color: #4fc3f7; animation-delay: 1.6s; }
        .light:nth-child(10) { left: 95%; background-color: #69f0ae; animation-delay: 1.8s; }
        
        /* Модальное окно */
        .modal-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.9);
            z-index: 1000;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }
        
        .modal-content {
            background: #1a2b3c;
            border-radius: 15px;
            padding: 30px;
            max-width: 500px;
            width: 100%;
            max-height: 90vh;
            overflow-y: auto;
            border: 2px solid #ff9800;
        }
        
        .modal-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
        }
        
        .modal-title {
            color: #ffeb3b;
            font-size: 24px;
        }
        
        .close-modal {
            background: none;
            border: none;
            color: #fff;
            font-size: 24px;
            cursor: pointer;
        }
        
        .payment-option {
            background: rgba(255, 255, 255, 0.05);
            border-radius: 10px;
            padding: 20px;
            margin-bottom: 15px;
            cursor: pointer;
            transition: all 0.3s;
            border: 1px solid transparent;
        }
        
        .payment-option:hover {
            border-color: #4fc3f7;
            transform: translateY(-3px);
        }
        
        .payment-option.selected {
            border-color: #4CAF50;
            background: rgba(76, 175, 80, 0.1);
        }
        
        .payment-details {
            display: none;
            margin-top: 20px;
            padding: 20px;
            background: rgba(0, 0, 0, 0.3);
            border-radius: 10px;
        }
        
        .card-number {
            font-family: monospace;
            font-size: 20px;
            letter-spacing: 2px;
            background: rgba(0, 0, 0, 0.5);
            padding: 15px;
            border-radius: 8px;
            text-align: center;
            margin: 10px 0;
            border: 1px dashed #4fc3f7;
        }
        
        .copy-btn {
            background: #2196F3;
            color: white;
            border: none;
            padding: 10px 20px;
            border-radius: 5px;
            cursor: pointer;
            margin-top: 10px;
            width: 100%;
        }
        
        .copy-btn:hover {
            background: #1976D2;
        }
    </style>
</head>
<body>
    <!-- Огни -->
    <div class="lights">
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
        <div class="light"></div>
    </div>
    
    <!-- Снег -->
    <div class="snowflakes" id="snowflakes"></div>
    
    <div class="container">
        <header>
            <div class="logo">
                <div class="logo-icon">SC</div>
                <div>
                    <div class="logo-text">Saya Coin</div>
                    <div class="logo-subtitle">Новогодний дилер 2026 | Ручная оплата</div>
                </div>
            </div>
            <div class="domain-info">
                <div>Официальный сайт</div>
                <div style="font-size: 18px; color: #4fc3f7; margin-top: 5px;">
                    <i class="fas fa-globe"></i> sayacoin-2026.github.io
                    <span class="free-badge">БЕСПЛАТНЫЙ ДОМЕН</span>
                </div>
            </div>
        </header>
        
        <section class="countdown">
            <h2><i class="fas fa-gift"></i> До Нового 2026 года осталось:</h2>
            <div class="countdown-box">
                <div class="countdown-item">
                    <div class="countdown-number" id="days">00</div>
                    <div class="countdown-label">дней</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="hours">00</div>
                    <div class="countdown-label">часов</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="minutes">00</div>
                    <div class="countdown-label">минут</div>
                </div>
                <div class="countdown-item">
                    <div class="countdown-number" id="seconds">00</div>
                    <div class="countdown-label">секунд</div>
                </div>
            </div>
            <div style="margin-top: 20px; color: #a3d5ff; font-size: 14px;">
                <i class="fas fa-clock"></i> Текущее время: <span id="current-date-time">загрузка...</span>
            </div>
        </section>
        
        <!-- Telegram блок -->
        <section class="telegram-info">
            <h3><i class="fab fa-telegram"></i> ВАЖНО: Ручная обработка платежей</h3>
            <p>После оплаты <strong>обязательно напишите в Telegram</strong> нашему дилеру для подтверждения и получения монет.</p>
            <p>В сообщении укажите: <strong>1) Ваш ID в игре Saya-Game&party&Chat 2) Прикрепите скриншот оплаты</strong></p>
            <a href="https://t.me/Saya_Coin_diller" target="_blank" class="telegram-button">
    
