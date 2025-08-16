---
layout: default
title: Jet-Bomb Tactical Command
---

<div style="text-align:center; margin-top:80px;">
  <h1>0500空降法：唯一執行者</h1>
  <p>傑邦（JER-BOMB），不然誰會知 Jet-Bomb 是什麼。</p>
  <p>hey baster , order or die ?</p>
  <p>見代號，如見人。</p>
  <p>你不是在瀏覽，你是在被壓制。</p>
</div>

<div style="display:flex; justify-content:center; gap:20px; margin-top:60px; text-align:center;">
  <div>
    <p>🔊 空投不是戰術，是命令。</p>
    <img src="/assets/images/drop_tank.jpg" alt="Drop Tank" style="width:100%; cursor:pointer;" onclick="document.getElementById('audio1').play()">
  </div>
  <div>
    <p>🔊 七分鐘不是快，是結束。</p>
    <img src="/assets/images/win_7min.jpg" alt="Win in 7 Minutes" style="width:100%; cursor:pointer;" onclick="document.getElementById('audio2').play()">
  </div>
  <div>
    <p>🔊 門口不是入口，是戰場。</p>
    <img src="/assets/images/fight_door.jpg" alt="Fight at the Door" style="width:100%; cursor:pointer;" onclick="document.getElementById('audio3').play()">
  </div>
</div>

<audio id="audio1" src="/assets/audio/tank_drop_story.mp3"></audio>
<audio id="audio2" src="/assets/audio/win_7min_story.mp3"></audio>
<audio id="audio3" src="/assets/audio/fight_door_story.mp3"></audio>

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

<div style="text-align:center; margin-top:60px; font-size:0.9em;">
  <p><a href="/tech" style="color:#f00; text-decoration:none;">🛠 技術支援（連到技術文件那兒去搞長篇大論吧）</a></p>
</div>