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

<!-- 空襲警報模組：滾動觸發 -->
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
  window.addEventListener("touchstart", unlockAudio);
</script>

<!-- Venus J 導引語音模組：滾動觸發 -->
<audio id="venusJ_intro" src="assets/audio/venusj_intro_0500.mp3" preload="auto"></audio>
<script>
  let venusTriggered = false;
  document.addEventListener("DOMContentLoaded", function () {
    const audio = document.getElementById("venusJ_intro");
    audio.muted = true;
    audio.play().then(() => {
      audio.pause();
      audio.muted = false;
    });
  });
  window.addEventListener("scroll", function () {
    if (!venusTriggered) {
      const audio = document.getElementById("venusJ_intro");
      audio.play();
      venusTriggered = true;
    }
  });
</script>

<!-- 字幕渲染區：Venus J 導引字幕 -->
<div id="venusJ_subtitle_box" style="font-size: 1.2em; font-weight: bold; color: #00ffcc; text-align: center; margin: 20px 0;"></div>

<!-- 戰術標語 -->
<p class="tactical-header">星海爭霸0500空降法：你不是在模仿，你是被研究</p>
<p class="tactical-header">傑邦就是JET-BOMB</p>
<p class="tactical-header">星海誰最能打, 是蟲王Serral?總有相見的那一天!</p>

<!-- 五模組區塊 -->
<div class="image-row five-row">
  <!-- 模組內容略，已保留不動 -->
</div>

<!-- 媒體模組區塊 -->
<p class="tactical-header">全球媒體模組：報導方式即將改寫</p>
<div class="image-row three-row">
  <!-- 模組內容略，已保留不動 -->
</div>

<!-- 空襲模組區塊 -->
<p class="tactical-header">0500空降警報模組：不是通知，是壓制</p>
<div class="image-row one-row">
  <!-- 模組內容略，已保留不動 -->
</div>

<!-- 字幕模組引用 -->
<script src="assets/modules/venusj_intro_subtitles.js"></script>
<script src="assets/modules/subtitle_renderer.js"></script>