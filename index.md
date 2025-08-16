---
layout: default
title: Jet-Bomb Tactical Command
---

<div style="text-align:center; margin-top:80px;">
  <img src="/assets/images/drop_tank.jpg" alt="Jet-Bomb Cover" style="width:60%;">
  <h1>0500空降法：唯一執行者</h1>
  <p>見代號，如見人。</p>
  <p>你不是在瀏覽，你是在被壓制。</p>
  <p>所有模組已部署，所有語言已固定。</p>
  <p>外部評論已轉化為神話。</p>
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