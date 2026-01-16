<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>us?</title>
<link href="https://fonts.googleapis.com/css2?family=Allura&display=swap" rel="stylesheet">
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

html, body {
  width: 100%;
  height: 100%;
  overflow: hidden;
}

body {
  display: flex;
  align-items: center;
  justify-content: center;
  position: relative;
  background: linear-gradient(135deg, #ffc5dc, #c5dcff, #ffe8b5, #ffc5dc);
  background-size: 400% 400%;
  animation: flowingColors 25s ease infinite;
}

@keyframes flowingColors {
  0% { background-position: 0% 50%; }
  25% { background-position: 50% 100%; }
  50% { background-position: 100% 50%; }
  75% { background-position: 50% 0%; }
  100% { background-position: 0% 50%; }
}

.magic-layer {
  position: fixed;
  inset: 0;
  pointer-events: none;
  overflow: hidden;
}

.sparkle {
  position: absolute;
  color: rgba(255, 255, 255, 0.6);
  font-size: 14px;
  animation: sparkleFloat 15s ease-in-out infinite;
}

.sparkle:nth-child(1) { top: 10%; left: 15%; animation-delay: 0s; font-size: 16px; }
.sparkle:nth-child(2) { top: 20%; left: 80%; animation-delay: 2s; font-size: 12px; }
.sparkle:nth-child(3) { top: 30%; left: 45%; animation-delay: 4s; font-size: 18px; }
.sparkle:nth-child(4) { top: 50%; left: 10%; animation-delay: 1s; font-size: 14px; }
.sparkle:nth-child(5) { top: 60%; left: 85%; animation-delay: 3s; font-size: 16px; }
.sparkle:nth-child(6) { top: 70%; left: 25%; animation-delay: 5s; font-size: 12px; }
.sparkle:nth-child(7) { top: 80%; left: 65%; animation-delay: 2.5s; font-size: 15px; }
.sparkle:nth-child(8) { top: 15%; left: 55%; animation-delay: 4.5s; font-size: 13px; }
.sparkle:nth-child(9) { top: 40%; left: 70%; animation-delay: 1.5s; font-size: 17px; }
.sparkle:nth-child(10) { top: 85%; left: 40%; animation-delay: 3.5s; font-size: 14px; }
.sparkle:nth-child(11) { top: 25%; left: 20%; animation-delay: 6s; font-size: 16px; }
.sparkle:nth-child(12) { top: 55%; left: 50%; animation-delay: 0.5s; font-size: 13px; }
.sparkle:nth-child(13) { top: 75%; left: 75%; animation-delay: 5.5s; font-size: 15px; }
.sparkle:nth-child(14) { top: 35%; left: 90%; animation-delay: 2.8s; font-size: 12px; }
.sparkle:nth-child(15) { top: 90%; left: 15%; animation-delay: 4.2s; font-size: 14px; }
.sparkle:nth-child(16) { top: 5%; left: 35%; animation-delay: 1.2s; font-size: 15px; }
.sparkle:nth-child(17) { top: 45%; left: 30%; animation-delay: 3.8s; font-size: 13px; }
.sparkle:nth-child(18) { top: 65%; left: 60%; animation-delay: 0.8s; font-size: 16px; }
.sparkle:nth-child(19) { top: 12%; left: 72%; animation-delay: 5.2s; font-size: 14px; }
.sparkle:nth-child(20) { top: 48%; left: 88%; animation-delay: 2.2s; font-size: 12px; }
.sparkle:nth-child(21) { top: 78%; left: 8%; animation-delay: 4.8s; font-size: 17px; }
.sparkle:nth-child(22) { top: 32%; left: 12%; animation-delay: 1.8s; font-size: 13px; }
.sparkle:nth-child(23) { top: 88%; left: 52%; animation-delay: 6.2s; font-size: 15px; }
.sparkle:nth-child(24) { top: 22%; left: 62%; animation-delay: 3.2s; font-size: 14px; }
.sparkle:nth-child(25) { top: 58%; left: 78%; animation-delay: 0.2s; font-size: 16px; }
.sparkle:nth-child(26) { top: 8%; left: 48%; animation-delay: 5.8s; font-size: 12px; }
.sparkle:nth-child(27) { top: 68%; left: 38%; animation-delay: 2.6s; font-size: 18px; }
.sparkle:nth-child(28) { top: 42%; left: 5%; animation-delay: 4.4s; font-size: 13px; }
.sparkle:nth-child(29) { top: 92%; left: 68%; animation-delay: 1.4s; font-size: 15px; }
.sparkle:nth-child(30) { top: 18%; left: 92%; animation-delay: 3.4s; font-size: 14px; }

@keyframes sparkleFloat {
  0%, 100% { 
    opacity: 0.2; 
    transform: translateY(0px) scale(1);
  }
  25% { 
    opacity: 0.6; 
    transform: translateY(-15px) scale(1.2);
  }
  50% { 
    opacity: 0.4; 
    transform: translateY(-8px) scale(0.9);
  }
  75% { 
    opacity: 0.7; 
    transform: translateY(-20px) scale(1.1);
  }
}

.glow-orbs {
  position: fixed;
  inset: 0;
  pointer-events: none;
}

.orb {
  position: absolute;
  border-radius: 50%;
  filter: blur(40px);
  animation: orbFloat 20s ease-in-out infinite;
}

.orb:nth-child(1) {
  width: 300px;
  height: 300px;
  top: -50px;
  left: -50px;
  background: radial-gradient(circle, rgba(249, 214, 229, 0.4), transparent);
  animation-delay: 0s;
}

.orb:nth-child(2) {
  width: 250px;
  height: 250px;
  bottom: -50px;
  right: -50px;
  background: radial-gradient(circle, rgba(214, 230, 246, 0.4), transparent);
  animation-delay: 5s;
}

.orb:nth-child(3) {
  width: 280px;
  height: 280px;
  top: 50%;
  left: 50%;
  background: radial-gradient(circle, rgba(251, 241, 212, 0.3), transparent);
  animation-delay: 10s;
}

@keyframes orbFloat {
  0%, 100% { transform: translate(0, 0) scale(1); }
  33% { transform: translate(30px, -40px) scale(1.1); }
  66% { transform: translate(-40px, 30px) scale(0.9); }
}

.content {
  position: relative;
  z-index: 10;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 56px;
}

.title {
  font-family: 'Allura', cursive;
  font-size: 96px;
  color: #ffffff;
  text-shadow: 
    0 0 20px rgba(255, 240, 250, 0.9),
    0 0 40px rgba(255, 220, 240, 0.6),
    0 0 60px rgba(255, 200, 230, 0.4);
  letter-spacing: 8px;
  animation: textFloat 6s ease-in-out infinite;
}

@keyframes textFloat {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-12px); }
}

video {
  width: 480px;
  max-width: 88vw;
  border-radius: 20px;
  box-shadow: 
    0 15px 60px rgba(255, 255, 255, 0.3),
    0 0 40px rgba(255, 220, 240, 0.2);
  cursor: pointer;
  transition: transform 0.3s ease;
}

video:hover {
  transform: scale(1.03);
}

@media (max-width: 600px) {
  .title {
    font-size: 64px;
    letter-spacing: 4px;
  }
}
</style>
</head>
<body>

<div class="glow-orbs">
  <div class="orb"></div>
  <div class="orb"></div>
  <div class="orb"></div>
</div>

<div class="magic-layer">
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
  <div class="sparkle">✦</div>
  <div class="sparkle">✧</div>
  <div class="sparkle">✨</div>
</div>

<div class="content">
  <div class="title">us?</div>
  <video controls>
    <source src="video.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>
</div>

</body>
</html>
