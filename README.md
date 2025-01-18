<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>❤️</title>
    <style>
        body {
            margin: 0;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background: linear-gradient(45deg, #ff9a9e, #fad0c4);
            font-family: Arial, sans-serif;
            text-align: center;
            padding: 20px;
        }

        .container {
            background: rgba(255, 255, 255, 0.95);
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.1);
            max-width: 350px;
            width: 90%;
        }

        h1 {
            color: #333;
            margin-bottom: 20px;
            font-size: 24px;
        }

        .photo-container {
            margin: 20px 0;
            position: relative;
            width: 100%;
            max-width: 300px;
            margin: 0 auto;
        }

        .photo {
            width: 100%;
            height: auto;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
        }

        .button {
            display: block;
            width: 100%;
            padding: 15px;
            margin: 10px 0;
            border: none;
            border-radius: 50px;
            background: #ff6b6b;
            color: white;
            font-size: 18px;
            cursor: pointer;
            transition: transform 0.3s, background 0.3s;
        }

        .button:hover {
            transform: scale(1.05);
            background: #ff5252;
        }

        .heart {
            font-size: 50px;
            margin-bottom: 20px;
            animation: pulse 1.5s infinite;
        }

        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.1); }
            100% { transform: scale(1); }
        }

        .message {
            font-size: 16px;
            color: #666;
            margin: 20px 0;
            line-height: 1.5;
        }

        .photo-frame {
            position: relative;
            padding: 10px;
            background: white;
            border-radius: 15px;
            box-shadow: 0 4px 8px rgba(0,0,0,0.1);
            margin: 20px 0;
        }

        .photo-frame::before {
            content: '';
            position: absolute;
            top: -5px;
            left: 50%;
            transform: translateX(-50%);
            width: 50px;
            height: 10px;
            background: #ff9a9e;
            border-radius: 5px;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="heart">❤️</div>
        <h1>OWO 喂喂喂？菜头在吗</h1>
        <h2>hello？</h2>
        <div class="photo-frame">
            <!-- 将下面的图片URL替换为你的图片地址 -->
            <img class="photo" src="[[https://phototj.photo.store.qq.com/psc?/V11hQB6t2VKUPe/bqQfVz5yrrGYSXMvKr.cqWrObVf4gh0Xhv*SJv1Xc4pJ7bsn4NMtR85PILRKJbH8XG1yd7Z4JRYrf.z*yYLm8srT8oSPykHrLa5*gerdIU4!/b&bo=QAZgCUAGYAkWECA!&rf=viewer_311](https://i.postimg.cc/gjL5dbh7/image.png)](https://i.postimg.cc/gjL5dbh7/image.png)" alt="我们的照片">
        </div>

        <p class="message">long time no see...</p>
        <button class="button" onclick="callLove('yes')">在~</button>
        <button class="button" onclick="callLove('definitely')">我错了！！我在！！！</button>
    </div>

    <script>
        function callLove(choice) {
            let message = '';
            if (choice === 'yes') {
                message = '哈，给我打电话！';
            } else {
                message = '现在就给我打电话！';
            }
            
            alert(message);
            window.location.href = 'tel:'; // 直接跳转到拨号界面
        }
    </script>
</body>
</html>
