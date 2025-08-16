---
layout: default
title: Jet-Bomb Tactical Command
---

<div style="text-align:center; margin-top:80px;">
  <h1>0500空降法：唯一執行者</h1>
  <p>hey baster , order or die ?</p>
  <p>見代號，如見人。</p>
  <p>你不是在瀏覽，你是在被壓制。</p>
</div>

<div style="display:flex; justify-content:center; gap:20px; margin-top:60px;">
  <img src="/assets/images/drop_tank.jpg" alt="Drop Tank" style="width:30%;">
  <img src="/assets/images/win_7min.jpg" alt="Win in 7 Minutes" style="width:30%;">
  <img src="/assets/images/fight_door.jpg" alt="Fight at the Door" style="width:30%;">
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

<div style="text-align:center; margin-top:80px; font-size:1em; font-weight:bold;">
  <p>hey guy , order or die</p>
</div>