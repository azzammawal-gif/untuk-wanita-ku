# untuk-wanita-ku
sehat sehat wanita ku
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Penjaga Hati — Untuk Elvira Rizki Ayunda P</title>
  <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,500;0,700;1,500&family=Plus+Jakarta+Sans:wght@400;500;600&display=swap" rel="stylesheet">
  <style>
    :root {
      --bg-1: #fff6f8;
      --bg-2: #ffe8ee;
      --card: rgba(255, 255, 255, 0.86);
      --primary: #c94a6a;
      --primary-dark: #a63452;
      --gold: #c89b54;
      --text: #3a232b;
      --muted: #7a5863;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      min-height: 100vh;
      font-family: 'Plus Jakarta Sans', sans-serif;
      color: var(--text);
      background: radial-gradient(circle at top left, var(--bg-1), var(--bg-2));
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 24px 16px;
      overflow-x: hidden;
      position: relative;
    }

    .floating-heart {
      position: fixed;
      bottom: -30px;
      color: rgba(201, 74, 106, 0.35);
      pointer-events: none;
      animation: floatUp linear forwards;
      z-index: 0;
    }

    @keyframes floatUp {
      0% { transform: translateY(0) scale(0.8); opacity: 0; }
      15% { opacity: 0.8; }
      100% { transform: translateY(-110vh) scale(1.25); opacity: 0; }
    }

    .card {
      position: relative;
      z-index: 1;
      width: 100%;
      max-width: 520px;
      background: var(--card);
      backdrop-filter: blur(12px);
      border: 1px solid rgba(201, 74, 106, 0.18);
      border-radius: 28px;
      padding: 36px 28px;
      box-shadow: 0 20px 50px rgba(166, 52, 82, 0.12);
      text-align: center;
    }

    .badge {
      display: inline-block;
      font-size: 12px;
      letter-spacing: 1.5px;
      text-transform: uppercase;
      color: var(--gold);
      font-weight: 600;
      margin-bottom: 10px;
    }

    h1 {
      font-family: 'Cormorant Garamond', serif;
      font-size: 36px;
      line-height: 1.15;
      color: var(--primary-dark);
      margin-bottom: 6px;
    }

    .recipient {
      font-family: 'Cormorant Garamond', serif;
      font-style: italic;
      font-size: 24px;
      color: var(--primary);
      margin-bottom: 24px;
    }

    /* Vinyl Player */
    .vinyl-wrap {
      display: flex;
      flex-direction: column;
      align-items: center;
      margin-bottom: 24px;
    }

    .vinyl {
      width: 112px;
      height: 112px;
      border-radius: 50%;
      background: radial-gradient(circle, #2b1d22 0%, #160e11 70%);
      border: 4px solid #f7d6df;
      box-shadow: 0 10px 25px rgba(58, 35, 43, 0.22);
      display: flex;
      align-items: center;
      justify-content: center;
      cursor: pointer;
      position: relative;
      transition: transform 0.3s ease;
    }

    .vinyl.playing {
      animation: spin 6s linear infinite;
    }

    .vinyl::before {
      content: "";
      position: absolute;
      inset: 14px;
      border-radius: 50%;
      border: 1px dashed rgba(255, 255, 255, 0.15);
    }

    .vinyl-center {
      width: 38px;
      height: 38px;
      border-radius: 50%;
      background: linear-gradient(135deg, var(--primary), var(--gold));
      display: flex;
      align-items: center;
      justify-content: center;
      color: #fff;
      font-size: 14px;
      box-shadow: inset 0 0 0 3px rgba(255,255,255,0.25);
    }

    @keyframes spin {
      100% { transform: rotate(360deg); }
    }

    .music-hint {
      margin-top: 10px;
      font-size: 12.5px;
      color: var(--muted);
    }

    /* Message Box */
    .letter-box {
      background: rgba(255, 246, 248, 0.9);
      border: 1px solid rgba(201, 74, 106, 0.14);
      border-radius: 18px;
      padding: 20px;
      text-align: left;
      margin-bottom: 20px;
      min-height: 148px;
    }

    .salutation {
      font-weight: 600;
      color: var(--primary-dark);
      margin-bottom: 8px;
      font-size: 15px;
    }

    #typed-text {
      font-size: 14.5px;
      line-height: 1.7;
      color: var(--text);
      white-space: pre-line;
    }

    .whisper {
      font-family: 'Cormorant Garamond', serif;
      font-style: italic;
      font-size: 19px;
      color: var(--primary-dark);
      margin-bottom: 22px;
      min-height: 28px;
    }

    .actions {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
      justify-content: center;
    }

    button {
      border: none;
      border-radius: 999px;
      padding: 12px 20px;
      font-family: inherit;
      font-size: 13.5px;
      font-weight: 600;
      cursor: pointer;
      transition: all 0.2s ease;
    }

    .btn-primary {
      background: linear-gradient(135deg, var(--primary), var(--primary-dark));
      color: #fff;
      box-shadow: 0 8px 20px rgba(201, 74, 106, 0.28);
    }

    .btn-primary:hover { transform: translateY(-2px); }

    .btn-secondary {
      background: #fff;
      color: var(--primary-dark);
      border: 1px solid rgba(201, 74, 106, 0.3);
    }

    .btn-secondary:hover { background: #fff0f4; }
  </style>
</head>
<body>

  <main class="card">
    <div class="badge">Special Dedication</div>
    <h1>Penjaga Hati</h1>
    <div class="recipient">Elvira Rizki Ayunda P</div>

    <div class="vinyl-wrap">
      <div class="vinyl" id="vinyl" title="Klik untuk putar/jeda melodi">
        <div class="vinyl-center" id="play-icon">▶</div>
      </div>
      <div class="music-hint" id="music-status">Ketuk piringan hitam untuk melodi lembut</div>
    </div>

    <div class="letter-box">
      <div class="salutation">Untuk Elvira Rizki Ayunda P,</div>
      <div id="typed-text"></div>
    </div>

    <div class="whisper" id="whisper-text">"Kan ku arungi tujuh laut samudra, demi menjaga hatimu."</div>

    <div class="actions">
      <button class="btn-primary" onclick="rainHearts()">Kirim Hujan Cinta ♥</button>
      <button class="btn-secondary" onclick="nextWhisper()">Bisikan Manis Lainnya</button>
    </div>
  </main>

  <script>
    const message =
      "Di antara riuhnya dunia, kehadiranmu selalu jadi tempat pulang paling tenang. " +
      "Terima kasih sudah menjadi alasan di balik setiap senyum dan semangat hari ini.\n\n" +
      "Tetaplah jadi Elvira yang hangat—karena sejauh apa pun langkah berjalan, hati ini akan selalu tahu ke mana harus pulang dan siapa yang ingin terus dijaga.";

    const whispers = [
      '"Kan ku arungi tujuh laut samudra, demi menjaga hatimu."',
      '"Bersamamu, hal-hal sederhana selalu terasa istimewa, Elvira."',
      '"Jika lelah menyapa harimu, ingat selalu ada hati yang mendoakanmu."',
      '"Namamu adalah bagian favorit di setiap doa dan cerita baikku."'
    ];

    // Typewriter effect
    let idx = 0;
    const typedEl = document.getElementById("typed-text");
    function typeWriter() {
      if (idx < message.length) {
        typedEl.textContent += message.charAt(idx);
        idx++;
        setTimeout(typeWriter, 28);
      }
    }
    typeWriter();

    // Whisper switcher
    let whisperIdx = 0;
    function nextWhisper() {
      whisperIdx = (whisperIdx + 1) % whispers.length;
      document.getElementById("whisper-text").textContent = whispers[whisperIdx];
      spawnHeart();
    }

    // Floating hearts
    function spawnHeart() {
      const heart = document.createElement("div");
      heart.className = "floating-heart";
      heart.textContent = ["♥", "♡", "✿"][Math.floor(Math.random() * 3)];
      heart.style.left = Math.random() * 100 + "vw";
      heart.style.fontSize = (14 + Math.random() * 18) + "px";
      heart.style.animationDuration = (4 + Math.random() * 4) + "s";
      document.body.appendChild(heart);
      setTimeout(() => heart.remove(), 8000);
    }

    setInterval(spawnHeart, 900);

    function rainHearts() {
      for (let i = 0; i < 24; i++) {
        setTimeout(spawnHeart, i * 80);
      }
    }

    // Soft Web Audio Melody
    let audioCtx = null;
    let isPlaying = false;
    let melodyTimer = null;
    const notes = [261.63, 329.63, 392.00, 493.88, 523.25, 493.88, 392.00, 329.63];
    let step = 0;

    function playNote(freq) {
      if (!audioCtx) audioCtx = new (window.AudioContext || window.webkitAudioContext)();
      const osc = audioCtx.createOscillator();
      const gain = audioCtx.createGain();
      osc.type = "sine";
      osc.frequency.setValueAtTime(freq, audioCtx.currentTime);
      gain.gain.setValueAtTime(0.001, audioCtx.currentTime);
      gain.gain.exponentialRampToValueAtTime(0.06, audioCtx.currentTime + 0.1);
      gain.gain.exponentialRampToValueAtTime(0.0001, audioCtx.currentTime + 1.2);
      osc.connect(gain);
      gain.connect(audioCtx.destination);
      osc.start();
      osc.stop(audioCtx.currentTime + 1.25);
    }

    const vinyl = document.getElementById("vinyl");
    const playIcon = document.getElementById("play-icon");
    const musicStatus = document.getElementById("music-status");

    vinyl.addEventListener("click", () => {
      isPlaying = !isPlaying;
      if (isPlaying) {
        vinyl.classList.add("playing");
        playIcon.textContent = "❚❚";
        musicStatus.textContent = "Melodi Penjaga Hati sedang mengalun...";
        playNote(notes[step % notes.length]);
        step++;
        melodyTimer = setInterval(() => {
          playNote(notes[step % notes.length]);
          step++;
        }, 750);
      } else {
        vinyl.classList.remove("playing");
        playIcon.textContent = "▶";
        musicStatus.textContent = "Melodi dijeda";
        clearInterval(melodyTimer);
      }
    });
  </script>
</body>
</html>
