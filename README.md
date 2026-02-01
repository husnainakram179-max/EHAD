[index.html](https://github.com/user-attachments/files/24996692/index.html)
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Ehad… I’m Sorry</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <style>
    /* Background setup */
    body {
      margin: 0;
      height: 100vh;
      background: 
        linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.85)),
        url('bg.jpg') no-repeat center center fixed;
      background-size: cover;
      display: flex;
      justify-content: center;
      align-items: center;
      font-family: 'Segoe UI', sans-serif;
      color: white;
      text-align: center;
      overflow: hidden;
    }

    /* Heartbeat glow effect */
    .card {
      background: rgba(0,0,0,0.4);
      padding: 40px;
      border-radius: 25px;
      max-width: 90%;
      box-shadow: 0 0 40px rgba(255,0,100,0.5);
      animation: fadeIn 2s ease;
    }

    h1 {
      font-size: 2.4em;
      margin-bottom: 20px;
      letter-spacing: 1px;
      opacity: 0;
      animation: appear 2s forwards 0.5s;
    }

    p {
      font-size: 1.2em;
      line-height: 1.8;
      opacity: 0;
      margin-bottom: 15px;
    }

    /* Animation for text lines */
    .line1 { animation: appear 2s forwards 2s; }
    .line2 { animation: appear 2s forwards 4s; }
    .line3 { animation: appear 2s forwards 6s; }

    .signature {
      margin-top: 25px;
      font-style: italic;
      opacity: 0;
      animation: appear 2s forwards 8s;
    }

    .heart {
      font-size: 2em;
      margin-top: 15px;
      animation: pulse 2s infinite;
    }

    .tap {
      margin-top: 25px;
      font-size: 0.9em;
      opacity: 0.5;
      animation: appear 2s forwards 10s;
    }

    @keyframes fadeIn {
      from { opacity: 0; transform: translateY(20px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.15); }
      100% { transform: scale(1); }
    }

    @keyframes appear {
      from { opacity: 0; transform: translateY(10px); }
      to { opacity: 1; transform: translateY(0); }
    }

  </style>
</head>
<body>

  <div class="card">
    <h1>Ehad…</h1>

    <p class="line1">I am so sorry…</p>
    <p class="line2">Please forgive me. My heart aches every second I hurt you.</p>
    <p class="line3">You have no idea how deeply I love you — it’s all for you, always.</p>

    <div class="signature">— Always yours, Zain</div>
    <div class="heart">❤️</div>
    <div class="tap">(Tap anywhere to hear my heart)</div>
  </div>

  <!-- Background music with fade in -->
  <audio id="bgMusic" loop>
    <source src="sorry-darling.mp3" type="audio/mpeg">
  </audio>

  <script>
    document.body.addEventListener('click', function () {
      const music = document.getElementById('bgMusic');
      music.volume = 0;
      music.play();
      let vol = 0;
      let fadeIn = setInterval(() => {
        if(vol < 1){
          vol += 0.02;
          music.volume = vol;
        } else {
          clearInterval(fadeIn);
        }
      }, 100);
    }, { once: true });
  </script>

</body>
</html>
[sorry-darling.mp3.mp3](https://github.com/user-attachments/files/24996693/sorry-darling.mp3.mp3)
![24ef8f73-5b09-4c85-9450-6ec310020591](https://github.com/user-attachments/assets/9f940461-82d1-4127-9701-49eb9f2a5724)
