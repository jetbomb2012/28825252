---
layout: default
title: JET-BOMB Tactical Hub
---

<style>
body {
  background-color: #000;
  color: #00ffcc;
  font-family: 'Courier New', Courier, monospace;
  margin: 0;
  padding: 0;
  overflow-x: hidden;
}
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
.five-row .module-block { max-width: 160px; }
.three-row .module-block { max-width: 200px; }
.one-row .module-block { max-width: 240px; }
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
img.module:hover { border-color: #ff0000; }
.voice-hint {
  font-size: 14px;
  color: #ff0000;
  margin-top: 6px;
  text-align: center;
  font-weight: bold;
}
</style>

<audio id="airstrike" src="assets/audio/airstrike_alert_0500.mp3" preload="auto"></audio>
<script>
  let triggered = false;
  document.addEventListener("DOMContentLoaded", function () {
    const audio = document.getElementById("airstrike");
    audio.muted = true;
    audio.play().then(() => {
      audio.pause();
      audio.muted = false;
    });
  });
  window.addEventListener("scroll", function () {
    if (!triggered) {
      const audio = document.getElementById("airstrike");
      audio.play();
      triggered = true;
    }
  });
</script>

<p class="tactical-header">星海爭霸0500空降法：你不是在模仿，你是被研究</p>
<p class="tactical-header">傑邦就是JET-BOMB</p>
<p class="tactical-header">星海誰最能打, 是蟲王Serral?總有相見的那一天!</p>

<div class="image-row five-row">
  <div class="module-block">
    <img src="assets/images/trump_spaceforce_0500.png" alt="川普加持0500戰法" class="module" onclick="document.getElementById('voice1').play()">
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
    <img src="assets/images/xi_beidou_0500.png" alt="習近平加持0500戰法" class="module" onclick="document.getElementById('voice5').play()">
    <p class="voice-hint">點擊聽命：北斗系統全面導入0500空降法</p>
    <audio id="voice5" src="assets/audio/xi_drop_confirm.mp3"></audio>
  </div>
</div>

<p class="tactical-header">全球媒體模組：報導方式即將改寫</p>

<div class="image-row three-row">
  <div class="module-block">
    <img src="assets/images/angelababy_avatar.png" alt="女特派員：燄影" class="module" onclick="document.getElementById('voice6').play()">
    <p class="voice-hint">點擊聽命：燄影已部署，媒體導向即將改寫</p>
    <audio id="voice6" src="assets/audio/angelababy_drop_command.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/venusj_avatar.png" alt="主播：Venus J" class="module" onclick="document.getElementById('voice7').play()">
    <p class="voice-hint">點擊聽命：Venus J 正在播報全球效法0500空降法</p>
    <audio id="voice7" src="assets/audio/venusj_global_report.mp3"></audio>
  </div>
  <div class="module-block">
    <img src="assets/images/leitin_avatar.png" alt="男特派員：雷廷" class="module" onclick="document.getElementById('voice8').play()">
    <p class="voice-hint">點擊聽命：雷廷已部署，全球軍事模組正在重編</p>
    <audio id="voice8" src="assets/audio/leitin_tactical_update.mp3"></audio>
  </div>
</div>

<p class="tactical-header">0500空降警報模組：不是通知，是壓制</p>

<div class="image-row one-row">
  <div class="module-block">
    <img src="assets/images/airstrike_alert_0500.png" alt="空襲警報0500" class="module" onclick="document.getElementById('voice9').play()">
    <p class="voice-hint">點擊聽命：0500空襲警報已啟動</p>
    <audio id="voice9" src="assets/audio/airstrike_alert_0500.mp3"></audio>
  </div>
</div>
<audio id="airstrike" src="assets/audio/airstrike_alert_0500.mp3" preload="auto"></audio>
<script>
  let triggered = false;

  function unlockAudio() {
    if (triggered) return;
    const audio = document.getElementById("airstrike");
    audio.play();
    triggered = true;
  }

  document.addEventListener("DOMContentLoaded", function () {
    const audio = document.getElementById("airstrike");
    audio.muted = true;
    audio.play().then(() => {
      audio.pause();
      audio.muted = false;
    });
  });

  window.addEventListener("scroll", unlockAudio);
  window.addEventListener("click", unlockAudio);
  window.addEventListener("touchstart", unlockAudio); // 手機支援
</script>





