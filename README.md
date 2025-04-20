
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Muskan, Will You Be Mine?</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to right, #ff4e50, #f9d423);
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      height: 100vh;
      color: white;
      text-align: center;
      overflow: hidden;
      animation: fadeIn 2s ease-in;
      position: relative;
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    h1 {
      font-size: 2.8rem;
      margin-bottom: 20px;
      z-index: 2;
    }

    p {
      font-size: 1.3rem;
      margin-bottom: 30px;
      z-index: 2;
    }

    .buttons {
      display: flex;
      gap: 20px;
      z-index: 2;
    }

    button {
      padding: 15px 30px;
      font-size: 1rem;
      border: none;
      border-radius: 30px;
      cursor: pointer;
      transition: transform 0.2s;
    }

    .yes {
      background-color: #e6005c;
      color: white;
    }

    .yes:hover {
      transform: scale(1.1);
    }

    .no {
      background-color: white;
      color: #e6005c;
    }

    .no:hover {
      transform: scale(1.1);.
    }

    .heart {
      font-size: 3rem;
      animation: pulse 1.5s infinite;
      z-index: 2;
    }

    @keyframes pulse {
      0% { transform: scale(1); }
      50% { transform: scale(1.2); }
      100% { transform: scale(1); }
    }

    .floating-heart {
      position: absolute;
      color: rgba(255, 0, 100, 0.6);
      font-size: 2rem;
      animation: floatUp 6s infinite;
      z-index: 1;
    }

    @keyframes floatUp {
      0% { bottom: -50px; opacity: 0; }
      50% { opacity: 1; }
      100% { bottom: 100%; opacity: 0; }
    }

    .image-container {
      margin-bottom: 20px;
      z-index: 2;
    }

    .image-container img {
      max-width: 200px;
      border-radius: 20px;
      box-shadow: 0 0 15px rgba(0, 0, 0, 0.3);
    }
<body>
  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-love.mp3" type="audio/mpeg">
    Your browser does not support the audio element.
  </audio>

  <!-- Cartoon Clouds -->
  <div class="cloud cloud1"></div>
  <div class="cloud cloud2"></div>
  <div class="cloud cloud3"></div>

  <!-- Image -->
  <div class="image-container">
    <img src="A_digital_photograph_captures_a_young_man_in_his_e.png" alt="Boy holding black rose">
  </div>

  <div class="heart">❤</div>
  <h1>Muskan, Will You Be Mine?</h1>
  <p>Muskan, I really like you. Will you be my forever?</p>
  <div class="buttons">
    <button class="yes" onclick="alert('YAY! Muskan said YES!')">Yes</button>
    <button class="no" onclick="alert('No? I’ll keep trying, Muskan!')">No</button>
  </div>

  <script>
    function createHeart() {
      const heart = document.createElement('div');
      heart.classList.add('floating-heart');
      heart.style.left = Math.random() * 100 + 'vw';
      heart.style.animationDuration = (3 + Math.random() * 3) + 's';
      heart.innerText = '❤';
      document.body.appendChild(heart);

      setTimeout(() => {
        heart.remove();
      }, 6000);
    }

    setInterval(createHeart, 500);
  </script>
</body>
</html>
