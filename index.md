<p class="tactical-header">0500空降法：你不是在模仿，你是被研究</p>

<div class="image-row five-row">
  <div class="module-block">
    <img src="assets/images/trump_spaceforce_0500.jpg" alt="川普加持0500戰法" class="module" onclick="document.getElementById('voice1').play()">
    <p class="voice-hint">點擊聽命：美軍已納入0500空降模組</p>
    <audio id="voice1" src="assets/audio/trump_drop_confirm.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/drop_tank.jpg" alt="Drop Tank" class="module" onclick="document.getElementById('voice2').play()">
    <p class="voice-hint">點擊聽命：空投不是選擇，是命令</p>
    <audio id="voice2" src="assets/audio/tank_drop_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/win_7min.jpg" alt="Win in 7min" class="module" onclick="document.getElementById('voice3').play()">
    <p class="voice-hint">點擊聽命：七分鐘不是預估，是限制</p>
    <audio id="voice3" src="assets/audio/win_7min_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/fight_door.jpg" alt="Fight Door" class="module" onclick="document.getElementById('voice4').play()">
    <p class="voice-hint">點擊聽命：門不是防線，是壓制起點</p>
    <audio id="voice4" src="assets/audio/fight_door_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/xi_beidou_0500.jpg" alt="習近平加持0500戰法" class="module" onclick="document.getElementById('voice5').play()">
    <p class="voice-hint">點擊聽命：北斗系統全面導入0500空降法</p>
    <audio id="voice5" src="assets/audio/xi_drop_confirm.mp3"></audio>
  </div>
</div>

<p class="tactical-header">全球媒體模組：報導方式即將改寫</p>

<div class="image-row three-row">
  <div class="module-block">
    <a href="https://drive.google.com/file/d/1XOIP_45C8_SkxJdq6c9JZvI1b5V9PDK_/view?usp=sharing" target="_blank">
      <img src="assets/images/drop_video_cover.png" alt="0500 Drop Video" class="module">
    </a>
    <p class="voice-hint">點擊進入：SC2_Terran_0500Drop_v1.mp4</p>
  </div>
  <div class="module-block">
    <img src="assets/images/qr_drop.png" alt="QR Code" class="module">
    <p class="voice-hint">掃描進入：0500空降模組</p>
  </div>
  <div class="module-block">
    <img src="assets/images/angelababy_avatar.png" alt="特派員(燄影) 戰地導引" class="module" onclick="document.getElementById('voice6').play()">
    <p class="voice-hint">點擊聽命：燄影已部署，媒體導向即將改寫</p>
    <audio id="voice6" src="assets/audio/angelababy_drop_command.mp3"></audio>
  </div>
</div>

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

.five-row .module-block {
  max-width: 160px;
}

.three-row .module-block {
  max-width: 200px;
}

.module-block {
  display: flex;
  flex-direction: column;
  align-items: center;
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
</style>