<html>
<head>
    <title>Login Page</title>
    <style>
        body, html {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            font-family: 'Arial', sans-serif;
            overflow: hidden;
            display: flex;
            align-items: center;
            justify-content: center;
            background-color: black;
        }
        .wrapper {
            width: 100vw;
            height: calc(100vw * 9 / 16); /* 16:9 aspect ratio */
            max-height: 100vh;
            position: relative;
            overflow: hidden;
        }
        .background-image {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            z-index: 1;
        }
        .overlay-video {
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            object-fit: cover;
            opacity: 0.5;
            z-index: 2;
        }
        .container {
            position: relative;
            z-index: 3;
            color: white;
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            height: 100%;
            text-align: center;
        }
        h1 {
            font-size: 2em;
            margin-bottom: 20px;
        }
        .input-container {
            margin: 10px 0;
        }
        .input-container label {
            display: block;
            font-size: 1.1em;
            margin-bottom: 5px;
        }
        .input-container input {
            width: 300px;
            padding: 10px;
            border: 2px solid white;
            border-radius: 25px;
            background: transparent;
            color: white;
            font-size: 1em;
            text-align: center;
        }
        .input-container input::placeholder {
            color: white;
        }
        .button-container {
            margin-top: 20px;
        }
        .button-container button {
            width: 150px;
            padding: 10px;
            border: none;
            border-radius: 25px;
            background: orange;
            color: white;
            font-size: 1.2em;
            cursor: pointer;
        }
        .footer-text {
            position: absolute;
            bottom: 40px; /* Naikkan sedikit agar tidak terlalu dekat dengan tepi bawah */
            right: 20px;
            font-size: 0.8em;
            color: white;
            background-color: rgba(0, 0, 0, 0.5); /* Menambahkan latar belakang transparan */
            padding: 5px 10px;
            border-radius: 10px;
            z-index: 4; /* Pastikan berada di atas video dan gambar */
        }
    </style>
</head>
<body>
    <div class="wrapper">
        <!-- Ganti URL background image dengan link Google Drive -->
        <img src="https://drive.google.com/uc?export=download&id=1-2ThDJEcJzpsFFbmfkDp3IHu_qgd8-hs" alt="Background Image" class="background-image">
        
        <!-- Ganti URL video overlay dengan link Google Drive -->
        <video class="overlay-video" autoplay loop muted>
            <source src="https://drive.google.com/uc?export=download&id=1-liXIRusKnFRJKGhXZbZHZGeU" type="video/mp4">
            Your browser does not support the video tag.
        </video>
        
        <div class="container">
            <h1>SIAP BUAT LIHAT SESUATU YANG SPESIAL?</h1>
            <div class="input-container">
                <label for="username">Username</label>
                <input type="text" id="username" placeholder="Enter your username">
            </div>
            <div class="input-container">
                <label for="password">Password</label>
                <input type="password" id="password" placeholder="Enter your password">
            </div>
            <div class="button-container">
                <button>Start</button>
            </div>
        </div>
        
        <div class="footer-text">
            Buat pasword aku kasi cluenya, masi inget ngga tanggal kita mulai deket?
        </div>
    </div>
</body>
</html>
