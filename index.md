---
layout: default
title: Jet-Bomb Tactical Command
---

<h1>🧨 0500空降法：執行者不是創造者，是壓制者</h1>

<hr>

<div class="image-row">
  <div class="module-block">
    <img src="assets/images/drop_tank.jpg" alt="Drop Tank" class="module" onclick="playAudio('tank_drop_story')">
    <audio id="tank_drop_story" src="assets/audio/tank_drop_story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/win_7min.jpg" alt="Win in 7min" class="module" onclick="playAudio('win_7min.story')">
    <audio id="win_7min.story" src="assets/audio/win_7min.story.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/fight_door.jpg" alt="Fight Door" class="module" onclick="playAudio('fight_door.story')">
    <audio id="fight_door.story" src="assets/audio/fight_door.story.mp3"></audio>
  </div>
</div>

<style>
.image-row {
  display: flex;
  justify-content: center;
  gap: 20px;
  margin: 30px 0;
}
.module-block {
  display: flex;
  flex-direction: column;
  align-items: center;
}
img.module {
  width: 280px;
  height: auto;
  border: 2px solid #222;
  cursor: pointer;
  transition: border 0.2s ease;
}
img.module:hover {
  border-color: #ff0000;
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

<hr>

<p>兩枚掛載，一個時間點。錯過即失敗。<br>
七分鐘不是預估，是限制。第八分鐘即為錯誤。<br>
失敗不是結束，是門前壓制的開始。</p>

<hr>

<h1>🧨 Order or die?</h1>

<p>你不是在選擇，你是在被選擇。<br>
語音模組已部署，QR已部署，CSS已部署。<br>
你還在猶豫，別人已經死了。</p>

<hr>