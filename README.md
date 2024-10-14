
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <title>Тест "Какой круг ада тебе подходит?"</title>
    <style>

        body {
            font-family: 'Arial', sans-serif;
            background-color: #f0f4f8; /* Нежный серый фон */
            color: #333;
            line-height: 1.6;
            padding: 20px;
        }
        
        .point {
            color: #333; /* Изменен на более темный для контраста */
        }
        
        .questions {
            margin: 2em 0;
            padding: 20px;
            background: #212121; /* Темный фон */
            border-radius: 10px; /* Более закругленные углы */
            box-shadow: 0 4px 20px rgba(0, 0, 0, 0.15); /* Более заметная тень */
        }
        
        .question span {
            display: block;
            margin-bottom: 1em;
            font-size: 1.3em; /* Увеличен размер шрифта */
            font-weight: bold;
            color: #fefefe; /* Цвет текста остался белым */
        }
        
        .answers {
            display: flex;
            justify-content: space-around; /* Изменено для равномерного распределения */
            margin-top: 1em; /* Добавлен отступ сверху */
        }
        
        .answer {
            flex: 1;
            padding: 15px;
            margin: 0 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
            background: #ffffff; /* Белый фон для ответов */
            transition: background 0.3s, transform 0.3s;
            cursor: pointer;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1); /* Легкая тень */
        }
        
        button {
            background-color: #009688; /* Цвет тропического чайного */
            color: white;
            border: none;
            padding: 15px 32px;
            text-align: center;
            text-decoration: none;
            display: inline-block;
            font-size: 16px;
            margin: 4px 2px;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s, transform 0.2s; /* Добавлено изменение размера */
        }
        
        button:hover {
            background-color: #00796b; /* Цвет при наведении */
            transform: scale(1.05); /* Увеличение кнопки */
        }
        
        .answer:hover {
            background: #e1f5fe; /* Нежный голубой фон при наведении */
            transform: translateY(-3px); /* Немного больше поднятие */
        }
        
        .selected {
            background-color: #ffb74d; /* Ярко-оранжевый цвет для выбранного */
            border: 1px solid #fff; /* Белая рамка для выделения */
        }
        
        .result {
            margin: 2em 0;
            color: #d32f2f;
            font-size: 1.5em;
            font-weight: bold;
        }
        
        </style>
        
</head>
<body>
    <h1 class="point">Тест "Какой круг ада тебе подходит?"</h1>
    
    <!-- Пункты опроса -->
    <div class="questions">
        <div class="question">
            <span >Как вы обычно реагируете на неудачи?</span>
            <div class="answers">
                <div class="answer" data-score="10">Я стараюсь учиться на ошибках и двигаться дальше.</div>
                <div class="answer" data-score="5">Я злюсь и виню других людей.</div>
                <div class="answer" data-score="1">Я расстраиваюсь и теряю интерес к делу.</div>
            </div>
        </div>

        <div class="question">
            <span>Как вы относитесь к деньгам?</span>
            <div class="answers">
                <div class="answer" data-score="10">Я стремлюсь зарабатывать достаточно, чтобы жить комфортно.</div>
                <div class="answer" data-score="5">Я люблю тратить деньги на дорогие вещи.</div>
                <div class="answer" data-score="1">Я экономлю и инвестирую в будущее.</div>
            </div>
        </div>

        <div class="question">
            <span>Как вы оцениваете свои достижения?</span>
            <div class="answers">
                <div class="answer" data-score="10">Я горжусь своими успехами и стараюсь их приумножить.</div>
                <div class="answer" data-score="5">Я сравниваю себя с другими и чувствую зависть.</div>
                <div class="answer" data-score="1">Я принимаю свои успехи как должное и не слишком радуюсь им.</div>
            </div>
        </div>

        <div class="question">
            <span>Как вы проводите свободное время?</span>
            <div class="answers">
                <div class="answer" data-score="10">Я занимаюсь спортом или хобби, которые мне нравятся.</div>
                <div class="answer" data-score="5">Я много ем и смотрю телевизор.</div>
                <div class="answer" data-score="1">Я сплю или просто бездельничаю.</div>
            </div>
        </div>

        <div class="question">
            <span>Как вы относитесь к отношениям с другими людьми?</span>
            <div class="answers">
                <div class="answer" data-score="10">Я ценю дружбу и поддерживаю хорошие отношения.</div>
                <div class="answer" data-score="5">Я часто конфликтую и обижаю других людей.</div>
                <div class="answer" data-score="1">Я избегаю близких отношений и предпочитаю одиночество.</div>
            </div>
        </div>
        <div class="question">
            <span>Вы когда ни будь крали что-либо?</span>
            <div class="answers">
                <div class="answer" data-score="10">да, меньше 1000 рублей</div>
                <div class="answer" data-score="5">да, больше 1000 рублей</div>
                <div class="answer" data-score="1">никогда.</div>
            </div>
        </div>
        <div class="question">
            <span>Вы когда ни будь обманывали людей?</span>
            <div class="answers">
                <div class="answer" data-score="10">конечно, всегда</div>
                <div class="answer" data-score="5">было пару раз</div>
                <div class="answer" data-score="1">нет, никогда</div>
            </div>
        </div>
        <div class="question">
            <span>У вас целая шоколадка, а у вашего друга нет, что
                вы выберете?</span>
            <div class="answers">
                <div class="answer" data-score="10">съесть все</div>
                <div class="answer" data-score="5">поделить поровну</div>
                <div class="answer" data-score="1">поделиться кусочком</div>
            </div>
        </div>
        <div class="question">
            <span>Вы видите, как бабушка несёт тяжелые пакеты с
                продуктами, что вы сделаете?</span>
            <div class="answers">
                <div class="answer" data-score="10">помочь донести пакеты до ее дома</div>
                <div class="answer" data-score="5">пройти мимо</div>
                <div class="answer" data-score="1">подставить ейподножку</div>
            </div>
        </div>
    </div>

    <!-- Форма для отправки ответов -->
    <form id="quizForm">
        <button type="button" onclick="checkQuiz()">Отправить ответы</button>
    </form>
    

    <!-- Результаты теста -->
    <div id="results"></div>

    <script>
// Функция для проверки ответов
function checkQuiz() {
    let totalScore = 0;
    const questions = document.querySelectorAll('.question');

    for (const question of questions) {
        const selectedAnswer = question.querySelector('.answer.selected');

        // Проверка выбранного ответа
        if (!selectedAnswer) {
            alert("Пожалуйста, выберите хотя бы один ответ.");
            return;
        }

        totalScore += parseInt(selectedAnswer.getAttribute('data-score'), 10);
    }

    showResults(totalScore);
}

// Показать результаты
function showResults(score) {
    const resultsDiv = document.getElementById('results');
    resultsDiv.textContent = `Ваш результат: ${score} баллов`;

    const resultMessage = getResultMessage(score);
    resultsDiv.innerHTML += `<br><strong>${resultMessage}</strong>`;
}

// Функция для получения сообщения о результате
function getResultMessage(score) {
    if (score <= 20) return "Круг 1 – Лимб";
    if (score <= 40) return "Круг 2 – Похоть";
    if (score <= 60) return "Круг 3 – Чревоугодие";
    if (score <= 80) return "Круг 4 – Скупость, алчность, жадность";
    if (score <= 100) return "Круг 5 – гнев";
    if (score <= 120) return "Круг 6 – Стены города Дита";
    if (score <= 140) return "Круг 7 – Город Дит";
    if (score <= 160) return "Круг 8 – Обманувшие недоверившихся";
    if (score <= 180) return "Круг 9 – Обманувшие доверившихся";
}

// Обработчик кликов для выбора ответа
document.addEventListener('click', function(event) {
    if (event.target.matches('.answer')) {
        const selectedAnswer = event.target;
        const question = selectedAnswer.closest('.question');

        // Удаляем класс 'selected' у всех ответов в текущем вопросе
        question.querySelectorAll('.answer').forEach(answer => {
            answer.classList.remove('selected');
        });

        // Добавляем класс 'selected' к выбранному ответу
        selectedAnswer.classList.add('selected');
    }
});
    </script>
    
</body>
</html>
