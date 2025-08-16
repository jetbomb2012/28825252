<p class="tactical-header">星海爭霸0500戰術，聽命或被殺？</p>

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