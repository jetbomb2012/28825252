---
layout: default
title: Jet-Bomb Tactical Command Center
---

**見代號如見人。**  
**0500空降法，執行者唯一。**  
**Order or die.**

## 🎧 Tactical Audio Modules

點擊任一圖像，立即播放語音壓力。

<style>
.image-module {
  display: flex;
  gap: 20px;
  justify-content: center;
  margin-top: 20px;
}
.image-module img {
  width: 300px;
  cursor: pointer;
  border: 2px solid transparent;
  transition: border 0.2s ease;
}
.image-module img:hover {
  border: 2px solid #ff0000;
}
</style>

<div class="image-module">
  <img src="/assets/images/drop_tank.jpg" onclick="playAudio('/assets/audio/drop_tank_voice.mp3')" alt="Drop Tank">
  <img src="/assets/images/win_7min.jpg" onclick="playAudio('/assets/audio/win_7min_voice.mp3')" alt="Win in 7 Minutes">
  <img src="/assets/images/fight_door.jpg" onclick="playAudio('/assets/audio/fight_door_voice.mp3')" alt="Fight at the Door">
</div>

<script>
function playAudio(src) {
  const audio = new Audio(src);
  audio.play();
}
</script>

你已進入戰術中心，離開即失效。