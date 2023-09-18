# kikiqyt063.github.io

This is a birthday gift for a special Jerry.

<!DOCTYPE html>
<html>
<head>
    <title>Happy Birthday!</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f7f7f7;
        }
        .container {
            max-width: 600px;
            margin: 0 auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.2);
            position: relative;
        }
        h1 {
            color: #ff6f61;
        }
        p {
            font-size: 18px;
        }
        .question {
            font-weight: bold;
            color: #ff6f61;
        }
        #answer {
            font-style: italic;
            color: #009688;

        }
        .penguin {
            position: fixed;
            top: 10;
            left: 20%;
            width: 20%;
            height: 30%;
            pointer-events: fill;
        }

        .fireworks {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
        }
        #questionnaire {
            display: -moz-box;

        }
        #round {
            font-weight: bold;
            font-size: 20px;
            color: #ff6f61;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Happy Birthday!</h1>
        <p>Dear Birthday Boy Akash Jetata,</p>
        <p>Your farts and your lovely ass officially turn 28 today!</p>
        <p>Here's a fun birthday card just for you,</p>
        <p>Produced by Kiki the Cartoon Giant Gentoo Penguin:</p>
        
        <div id="questionnaire">
            <p id="round">Round 1:</p>
            <p class="question" id="questionText"></p>
            <button onclick="nextQuestion('Yes')">Yes</button>
            <button onclick="nextQuestion('No')">No</button>
        </div>
        
        <div id="birthday-message" style="display: none;">
            <p class="question">Happy Birthday! 🎉</p>
            <p id="answer">Every single day with you is a blessing, </p>
            <p>Especially when you admit you are a Jerry. </p>
            <p>What a journey we've had and will continue to have,
                <p> filled with laughter and joy, </p>
            <p>Have an amazing birthday in Bangalore even without the annoying Kiki!</p>
        </div>
    </div>

    <!-- Animals and Fireworks Effects -->
    <img class="penguin" src="penguin.gif" alt="penguin">
    <img class="jerry" src="jerry.gif" alt="jerry">
    <img class="fireworks" src="fireworks.gif" alt="Fireworks">

    <script>
        let round = 0;
        const questions = [
            "Are you ready for this?",
            "Are you REALLY ready for this?", 
            "Identity Verification: Are you the BIRTHDAY BOY JETATA?",           
            "OK. Is babe a LOVELY Jerry?",
            "Good. Is baobei a CLEVER Patata?!",
            "Hmm? Is baobei a Jetata AKA a Human 2.0?!?!",
            "Fine. Does baobei REALLY LOVE the Penguin baobei?"
        ];

        function nextQuestion(answer) {
            round++;
            if (round < questions.length) {
                document.getElementById("round").textContent = "Round " + (round + 1) + ":";
                document.getElementById("questionText").textContent = questions[round];
            } else {
                // Display the Happy Birthday message
                document.getElementById("questionnaire").style.display = "none";
                document.getElementById("birthday-message").style.display = "block";
            }
        }

        // Start with the first question
        document.getElementById("questionText").textContent = questions[round];
    </script>
</body>
</html>
