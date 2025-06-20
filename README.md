<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>300 Спартанок — Бизнес-сообщество сильных женщин</title>
    <style>
        body {
            margin: 0;
            font-family: 'Segoe UI', sans-serif;
            background: linear-gradient(to right, #1a1a1a, #333);
            color: #f5f5f5;
            overflow-x: hidden;
        }
        header {
            background: url('https://images.unsplash.com/photo-1584824486539-53bb4646bdbc') no-repeat center/cover;
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            position: relative;
        }
        header::after {
            content: "";
            position: absolute;
            top: 0; left: 0; right: 0; bottom: 0;
            background: rgba(0,0,0,0.5);
        }
        header h1 {
            position: relative;
            font-size: 4em;
            margin: 0;
            color: #ffe4e9;
            text-shadow: 2px 2px 5px #000;
            z-index: 1;
        }
        header p {
            position: relative;
            font-size: 1.5em;
            color: #ffd1e1;
            z-index: 1;
            margin-top: 20px;
        }
        .section {
            max-width: 1000px;
            margin: 80px auto;
            padding: 0 20px;
            opacity: 0;
            transform: translateY(50px);
            transition: all 0.8s ease;
        }
        .section.active {
            opacity: 1;
            transform: translateY(0);
        }
        .btn {
            display: inline-block;
            background-color: #b30059;
            color: white;
            padding: 15px 30px;
            border-radius: 5px;
            text-decoration: none;
            margin-top: 30px;
            transition: 0.3s;
        }
        .btn:hover {
            background-color: #ff3377;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: #111;
            font-size: 0.9em;
        }
        .features {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-around;
        }
        .feature {
            width: 280px;
            background-color: #2e2e2e;
            padding: 20px;
            margin: 15px;
            border-radius: 10px;
            text-align: center;
            transition: 0.5s;
        }
        .feature:hover {
            transform: translateY(-10px);
            box-shadow: 0 5px 15px rgba(255, 51, 119, 0.4);
        }
        .feature h3 {
            margin-bottom: 15px;
            color: #ff77aa;
        }
        .story {
            background-color: #2b2b2b;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 0 20px rgba(0,0,0,0.3);
        }
    </style>
</head>
<body>

<header>
    <h1>300 Спартанок</h1>
    <p>Женская энергия, которая движет бизнесом</p>
</header>

<div class="section" id="about">
    <h2>О нас</h2>
    <p>
        «300 Спартанок» — это не просто бизнес-сообщество.  
        Это пространство силы, поддержки и роста для женщин, которые решают идти до конца, ставить амбициозные цели и воплощать их. Здесь рождаются настоящие бизнес-воительницы.
    </p>
</div>

<div class="section" id="services">
    <h2>Что мы даём</h2>
    <div class="features">
        <div class="feature">
            <h3>Бизнес-консалтинг</h3>
            <p>От стратегии до запуска: мы выстраиваем систему под твой характер и амбиции.</p>
        </div>
        <div class="feature">
            <h3>Обучение</h3>
            <p>Живые мастер-группы, интенсивы и тренинги, после которых ты не останешься прежней.</p>
        </div>
        <div class="feature">
            <h3>Сообщество</h3>
            <p>Поддержка, честные разговоры, обмен опытом, контакты и нетворкинг.</p>
        </div>
    </div>
</div>

<div class="section" id="story">
    <h2>Одна из наших историй</h2>
    <div class="story">
        <p><em>
            «Когда я пришла в "300 Спартанок", мой бизнес уже три года топтался на одном месте. Я сомневалась в себе, не умела продавать, боялась рисковать.  
            Уже через 4 месяца наставничества я увеличила доход в 3 раза, набрала команду и впервые почувствовала настоящую уверенность.  
            Здесь не просто учат — здесь рядом с тобой стоят такие же сильные, которые знают, что такое настоящий рост».
        </em></p>
        <p style="text-align: right;">— Марина К., владелица агентства дизайна</p>
    </div>
</div>

<div class="section" id="join">
    <h2>Готова стать одной из нас?</h2>
    <p>Оставь заявку — и мы обсудим твой путь в сообществе «300 Спартанок».</p>
    <a href="mailto:join@300spartanki.ru" class="btn">Хочу в команду</a>
</div>

<footer>
    © 2025 300 Спартанок | Все права защищены
</footer>

<script>
    // Анимация при прокрутке
    const sections = document.querySelectorAll('.section');
    window.addEventListener('scroll', () => {
        sections.forEach(section => {
            const rect = section.getBoundingClientRect();
            if (rect.top < window.innerHeight - 100) {
                section.classList.add('active');
            }
        });
    });
</script>

</body>
</html>
