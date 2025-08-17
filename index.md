<!-- 🔥 固定浮貼：雷庭（左）與燄影（右） -->
<style>
.fixed-witness {
  position: fixed;
  top: 80px;
  width: 180px;
  z-index: 999;
  text-align: center;
}
.fixed-left { left: 0; }
.fixed-right { right: 0; }

.voice-button {
  margin-top: 8px;
  font-size: 18px;
  background: none;
  border: none;
  cursor: pointer;
}

.speech-bubble {
  margin-top: 6px;
  font-size: 14px;
  color: #ff0000;
  font-weight: bold;
  background: #fff0f0;
  padding: 6px;
  border-radius: 6px;
  box-shadow: 0 0 6px rgba(0,0,0,0.2);
}
</style>

<!-- 左側：雷庭 -->
<div class="fixed-witness fixed-left">
  <lottie-player src="assets/animations/leiting_motion.json"
                 background="transparent"
                 speed="1"
                 style="width: 180px; height: 400px;"
                 loop autoplay>
  </lottie-player>
  <audio id="voice-leiting" src="assets/audio/lei-ting.mp3"></audio>
  <button onclick="document.getElementById('voice-leiting').play()" class="voice-button">🔊</button>
  <div class="speech-bubble">「0500, 不是時間, 是信仰」<br>「命令不需解釋, 執行才是語言」</div>
</div>

<!-- 右側：燄影 -->
<div class="fixed-witness fixed-right">
  <lottie-player src="assets/animations/yanying_motion.json"
                 background="transparent"
                 speed="1"
                 style="width: 180px; height: 400px;"
                 loop autoplay>
  </lottie-player>
  <audio id="voice-yanying" src="assets/audio/yan-ying.mp3"></audio>
  <button onclick="document.getElementById('voice-yanying').play()" class="voice-button">🔊</button>
  <div class="speech-bubble">「見代號, 如見人」<br>「你不是在看立牌, 你在被審問」</div>
</div>

<!-- 🔻戰術語言模組 -->
<p class="tactical-header">星海爭霸0500戰術，聽命或被殺？</p>
<p class="tactical-header">傑邦就是JET-BOMB</p>
<p class="tactical-header">星海爭霸誰最能打,是Serral？</p>

<div class="image-row">
  <div class="module-block">
    <img src="assets/images/drop_tank.jpg" alt="Drop Tank" class="module" onclick="document.getElementById('voice1').play()">
    <p class="voice-hint">點擊聽命：空投不是選擇，是命令。</p>
    <audio id="voice1" src="assets/audio/tank_drop_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/win_7min.jpg" alt="Win in 7min" class="module" onclick="document.getElementById('voice2').play()">
    <p class="voice-hint">點擊聽命：七分鐘不是預估，是限制。</p>
    <audio id="voice2" src="assets/audio/win_7min_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/fight_door.jpg" alt="Fight Door" class="module" onclick="document.getElementById('voice3').play()">
    <p class="voice-hint">點擊聽命：門不是防線，是壓制起點。</p>
    <audio id="voice3" src="assets/audio/fight_door_story.mp3"></audio>
  </div>
</div>

<!-- 🔧 原CSS樣式保留 -->
<style>
.tactical-header {
  font-size: 18px;
  color: #ff0000;
  text-align: center;
  font-weight: bold;
  margin-bottom: 20px;
}
.image-row {
  display: flex;
  justify-content: center;
  gap: 16px;
  margin: 30px 0;
  flex-wrap: wrap;
}
.module-block {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 180px;
}
img.module {
  width: 100%;
  height: auto;
  border: 2px solid #222;
  cursor: pointer;
  transition: border 0.2s ease;
}
img.module:hover {
  border-color: #ff0000;
}
.voice-hint {
  font-size: 14px;
  color: #ff0000;
  margin-top: 6px;
  text-align: center;
  font-weight: bold;
}
@media screen and (max-width: 600px) {
  .module-block {
    max-width: 100%;
  }
  img.module {
    max-width: 80vw;
  }
}
</style>

<!-- 🔧 引入 Lottie 播放器 -->
<script src="https://unpkg.com/@lottiefiles/lottie-player@latest/dist/lottie-player.js"></script>