<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stock Education AI</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 50px;
            background-color: #f0f8ff;
        }
        h1 {
            color: #2e8b57;
        }
        p {
            color: #333;
            font-size: 18px;
        }
        input, button {
            padding: 10px;
            font-size: 16px;
            margin: 10px;
        }
        .answer {
            margin-top: 20px;
            font-weight: bold;
        }
    </style>
</head>
<body>
    <h1>Stock & Mutual Fund Education AI</h1>
    <p>Ask your question below:</p>
    <input type="text" id="question" placeholder="Type your question here">
    <button onclick="getAnswer()">Ask AI</button>
    <div class="answer" id="answer"></div>

    <script>
        function getAnswer() {
            const question = document.getElementById('question').value.toLowerCase();
            let answer = "Sorry, I don't know the answer yet.";

            if(question.includes("stock risk")) {
                answer = "Stock risk refers to the possibility of losing money in stock investments.";
            } else if(question.includes("mutual fund")) {
                answer = "Mutual funds pool money from investors to buy diversified assets.";
            } else if(question.includes("low risk")) {
                answer = "Low-risk investments have smaller returns but more stability.";
            }

            document.getElementById('answer').innerText = answer;
        }
    </script>
</body>
</html>
