<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Danish Baby Name Swiper</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
        }
        .card {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            padding: 20px;
            width: 300px;
            text-align: center;
        }
        .name {
            font-size: 24px;
            margin-bottom: 20px;
        }
        .buttons {
            display: flex;
            justify-content: space-around;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        #dislike { background-color: #ff4d4d; }
        #like { background-color: #4CAF50; }
        #favorite { background-color: #ff9800; }
        #shareCode, #loadCode {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
        }
        #loadButton {
            width: 100%;
            padding: 10px;
            background-color: #008CBA;
            color: white;
        }
        #choices {
            margin-top: 20px;
            text-align: left;
        }
    </style>
</head>
<body>
    <div class="card">
        <div class="name" id="currentName"></div>
        <div class="buttons">
            <button id="dislike">👎</button>
            <button id="favorite">❤️</button>
            <button id="like">👍</button>
        </div>
    </div>
    <input type="text" id="shareCode" readonly placeholder="Your share code will appear here">
    <input type="text" id="loadCode" placeholder="Enter share code">
    <button id="loadButton">Load Shared Names</button>
    <div id="choices"></div>

    <script>
        const danishBabyNames = [
            'Freja', 'Oscar', 'Alma', 'William', 'Clara', 'Noah', 'Ella', 'Alfred',
            'Sofia', 'Carl', 'Ida', 'Emil', 'Anna', 'Oliver', 'Isabella', 'August',
            'Laura', 'Valdemar', 'Karla', 'Aksel', 'Nora', 'Magnus', 'Liva', 'Elias'
        ];

        let currentNames = [];
        let currentIndex = 0;
        let choices = {};

        function shuffleArray(array) {
            for (let i = array.length - 1; i > 0; i--) {
                const j = Math.floor(Math.random() * (i + 1));
                [array[i], array[j]] = [array[j], array[i]];
            }
        }

        function initializeNames() {
            currentNames = [...danishBabyNames];
            shuffleArray(currentNames);
            currentIndex = 0;
            choices = {};
            updateShareCode();
            showCurrentName();
            updateChoices();
        }

        function showCurrentName() {
            document.getElementById('currentName').textContent = currentNames[currentIndex];
        }

        function updateShareCode() {
            const shareCode = btoa(JSON.stringify(currentNames));
            document.getElementById('shareCode').value = shareCode;
        }

        function handleChoice(choice) {
            choices[currentNames[currentIndex]] = choice;
            currentIndex = (currentIndex + 1) % currentNames.length;
            showCurrentName();
            updateChoices();
        }

        function updateChoices() {
            const choicesDiv = document.getElementById('choices');
            choicesDiv.innerHTML = '<h3>Your Choices:</h3>';
            for (const [name, choice] of Object.entries(choices)) {
                const emoji = choice === 'like' ? '👍' : choice === 'dislike' ? '👎' : '❤️';
                choicesDiv.innerHTML += `<div>${name}: ${emoji}</div>`;
            }
        }

        document.getElementById('dislike').addEventListener('click', () => handleChoice('dislike'));
        document.getElementById('like').addEventListener('click', () => handleChoice('like'));
        document.getElementById('favorite').addEventListener('click', () => handleChoice('favorite'));

        document.getElementById('loadButton').addEventListener('click', () => {
            const loadCode = document.getElementById('loadCode').value;
            try {
                const loadedNames = JSON.parse(atob(loadCode));
                if (Array.isArray(loadedNames) && loadedNames.every(name => typeof name === 'string')) {
                    currentNames = loadedNames;
                    currentIndex = 0;
                    choices = {};
                    showCurrentName();
                    updateChoices();
                    alert('Shared names loaded successfully!');
                } else {
                    throw new Error('Invalid shared code');
                }
            } catch (error) {
                alert('Invalid shared code. Please try again.');
            }
        });

        initializeNames();
    </script>
</body>
</html>
