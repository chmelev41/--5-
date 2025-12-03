<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Простая машинка</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            background: #139fd6bb;
            overflow: hidden;
        }
        
        .car {
            position: absolute;
            width: 200px;
            height: 80px;
            left: -200px;
            top: 50%;
            animation: move 3s ease-out forwards;
        }
        
        .body {
            position: absolute;
            width: 100%;
            height: 60px;
            background: rgb(255, 18, 18);
            top: 20px;
            border-radius: 10px 10px 0 0;
        }
        
        .cab {
            position: absolute;
            width: 80px;
            height: 35px;
            background: rgb(252, 0, 0);
            top: 0;
            left: 120px;
            border-radius: 5px;
        }
        
        .window {
            position: absolute;
            width: 60px;
            height: 30px;
            background: lightblue;
            top: 5px;
            left: 10px;
            border-radius: 3px;
        }
        
        .wheel {
            position: absolute;
            width: 35px;
            height: 35px;
            background: black;
            border-radius: 50%;
            bottom: 0;
        }
        
        .wheel1 {
            left: 20px;
        }
        
        .wheel2 {
            right: 20px;
        }
        
        @keyframes move {
            0% { left: -200px; }
            100% { left: calc(100% - 250px); }
        }
    </style>
</head>
<body>
    <div class="car">
        <div class="body"></div>
        <div class="cab">
            <div class="window"></div>
        </div>
        <div class="wheel wheel1"></div>
        <div class="wheel wheel2"></div>
    </div>
</body>
</html>
