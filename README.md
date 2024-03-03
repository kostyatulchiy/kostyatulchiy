<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Buttons</title>
    <style>
        body {
            margin: 0;
            padding: 0;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-image: url('https://i.postimg.cc/0Ngh9HWq/1.jpg');
            background-size: cover;
            background-repeat: no-repeat;
        }
        .button-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            gap: 20px;
        }
        button {
            padding: 15px 30px;
            font-size: 20px;
            border: none;
            background-color: #000000;
            color: #ffffff;
            cursor: pointer;
            border-radius: 50px;
            width: 300px; /* Adjust the width as needed */
            position: relative;
            overflow: hidden;
            box-shadow: 5 10px 15px rgba(0, 0, 0, 0.5);
        }
        button img {
            position: absolute;
            left: 10px;
            top: 50%;
            transform: translateY(-50%);
            height: 30px;
            width: auto;
        }
        button span {
            margin-left: 40px;
            position: relative;
            z-index: 1;
        }
        button:hover {
            background-color: #ffffffb6;
        }
    </style>
</head>
<body>
    <div class="button-container">
        <button onclick="openTelegram()">
            <img src="https://i.postimg.cc/4xHLW1WY/Telegram-logo.png" alt="Telegram Logo">
            <span>UC SHOP</span>
        </button>
        <button onclick="openDonate()">
            <img src="https://i.postimg.cc/5y9KpdrJ/mono-logo-200-1x.png" alt="Mono Logo">
            <span> DONATE</span>
        </button>
    </div>

    <script>
        function openTelegram() {
            window.open('https://t.me/immaculate_uc', '_blank');
        }

        function openDonate() {
            window.open('https://send.monobank.ua/jar/4DZyU1A1Eq', '_blank');
        }
    </script>
</body>
</html>
