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

<!-- 🔥 新增模組：雷庭 vs 燄影｜立體人形壓迫模組 -->
<div class="witness-3d-row">
  <!-- 雷庭 -->
  <div class="witness-3d-block">
    <img src="assets/images/thunder_court_3d.jpg" alt="雷庭：語言審判者" class="witness-3d-img" onclick="document.getElementById('voice-thunder').play()">
    <p class="voice-hint">雷庭：「像機器人。太冷血。沒人會這樣講話。」</p>
    <p class="voice-hint">你審判語言，我武裝語言。</p>
    <audio id="voice-thunder" src="assets/audio/lei-ting.mp3"></audio>
  </div>

  <!-- 燄影 -->
  <div class="witness-3d-block">
    <img src="assets/images/flame_shade_3d.jpg" alt="燄影：神話解構者" class="witness-3d-img" onclick="document.getElementById('voice-flame').play()">
    <p class="voice-hint">燄影：「他真的以為自己是湯姆·克魯斯嗎？這種語言是刻意的嗎？」</p>
    <p class="voice-hint">你解構神話，我成為神話。</p>
    <audio id="voice-flame" src="assets/audio/yan-ying.mp3"></audio>
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

/* 🔧 新增樣式：雷庭與燄影模組 */
.witness-3d-row {
  display: flex;
  justify-content: center;
  gap: 48px;
  margin: 60px 0;
  flex-wrap: wrap;
}
.witness-3d-block {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 280px;
}
.witness-3d-img {
  width: 100%;
  height: auto;
  border: 3px solid #222;
  box-shadow: 0 0 20px rgba(0,0,0,0.6);
  border-radius: 6px;
  cursor: pointer;
  transition: transform 0.2s ease, border-color 0.2s ease;
}
.witness-3d-img:hover {
  transform: scale(1.03);
  border-color: #ff0000;
}
</style>