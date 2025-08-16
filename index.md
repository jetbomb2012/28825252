---
layout: default
title: Jet-Bomb Tactical Command
---

<style>
  body {
    background-color: #000;
    color: #eee;
    font-family: 'Courier New', monospace;
    margin: 0;
    padding: 0;
  }
  .centered {
    text-align: center;
    margin-top: 80px;
  }
  .badge-top-right {
    position: absolute;
    top: 12px;
    right: 12px;
  }
  .audio-warning {
    text-align: center;
    font-weight: bold;
    margin-top: 4px;
    color: #f00;
    font-size: 1.1em;
  }
</style>

<div class="badge-top-right">
  <img src="/assets/images/jetbomb_badge.png" alt="Jet-Bomb Badge" style="width:80px;">
</div>

<audio id="jetbomb-audio" src="/assets/audio/order_or_die_init.mp3"></audio>
<script>
  window.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('jetbomb-audio');
    const playPromise = audio.play();
    if (playPromise !== undefined) {
      playPromise.catch(() => {
        document.body.addEventListener('click', () => audio.play(), { once: true });
      });
    }
  });
</script>

<p class="audio-warning">
  🔊 你已被鎖定。命令已下達。執行或滅亡。
</p>

<div class="centered">
  <h1>0500空降法：唯一執行者</h1>
  <p>見代號，如見人。</p>
  <p>你不是在瀏覽，你是在被壓制。</p>
  <p>所有模組已部署，所有語言已固定。</p>
  <p>外部評論已轉化為神話。</p>
</div>