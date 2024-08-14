<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Playlist Imagine Dragons</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            text-align: center;
            padding: 50px;
        }
        h1 {
            color: #333;
        }
        .player {
            margin: 20px 0;
        }
        button {
            margin: 5px;
            padding: 10px 20px;
            font-size: 16px;
            cursor: pointer;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
        }
        button:hover {
            background-color: #45a049;
        }
    </style>
</head>
<body>
    <h1>Playlist Imagine Dragons</h1>

    <div class="player">
        <audio id="audioPlayer" controls>
            <source id="audioSource" src="musica1.mp3" type="audio/mpeg">
            Seu navegador não suporta o elemento de áudio.
        </audio>
    </div>

    <div class="playlist">
        <button onclick="playSong('musica1.mp3')">Radioactive</button>
        <button onclick="playSong('musica2.mp3')">Believer</button>
        <button onclick="playSong('musica3.mp3')">Demons</button>
        <button onclick="playSong('musica4.mp3')">Thunder</button>
        <button onclick="playSong('musica5.mp3')">Whatever It Takes</button>
    </div>

    <script>
        function playSong(musicFile) {
            var audioPlayer = document.getElementById('audioPlayer');
            var audioSource = document.getElementById('audioSource');
            audioSource.src = musicFile;
            audioPlayer.load();
            audioPlayer.play();
        }
    </script>
</body>
</html>
