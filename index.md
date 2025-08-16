<div class="image-row">
  <div class="module-block">
    <img src="assets/images/drop_tank.jpg" alt="Drop Tank" class="module" onclick="playAudio('tank_drop_story')">
    <audio id="tank_drop_story" src="assets/audio/tank_drop_story.mp3"></audio>
    <p class="voice-hint">點擊聽命：空投不是選擇，是命令。</p>
  </div>
  <div class="module-block">
    <img src="assets/images/win_7min.jpg" alt="Win in 7min" class="module" onclick="playAudio('win_7min_story')">
    <audio id="win_7min_story" src="assets/audio/win_7min.story.mp3"></audio>
    <p class="voice-hint">點擊聽命：七分鐘不是預估，是限制。</p>
  </div>
  <div class="module-block">
    <img src="assets/images/fight_door.jpg" alt="Fight Door" class="module" onclick="playAudio('fight_door_story')">
    <audio id="fight_door_story" src="assets/audio/fight_door.story.mp3"></audio>
    <p class="voice-hint">點擊聽命：門不是防線，是壓制起點。</p>
  </div>
</div>

<style>
.image-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 30px 0;
  flex-wrap: wrap;
}
.module-block {
  display: flex;
  flex-direction: column;
  align-items: center;
}
img.module {
  width: 280px;
  max-width: 45vw;
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
  margin-top: 8px;
  text-align: center;
  font-weight: bold;
}
</style>

<script>
function playAudio(id) {
  const audio = document.getElementById(id);
  if (audio) {
    audio.currentTime = 0;
    audio.play();
  }
}
</script>