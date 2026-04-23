---
title: 我的私藏歌单
date: 2026-04-23 23:00:00
---

<!-- 引入 APlayer 播放器的样式和脚本 -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/aplayer@1.10.1/dist/APlayer.min.css">
<script src="https://cdn.jsdelivr.net/npm/aplayer@1.10.1/dist/APlayer.min.js"></script>

<!-- 播放器会显示在这里 -->
<div id="aplayer"></div>

<script>
// 这就是你的歌单！想改顺序、加歌、删歌，直接改这个列表就行
const ap = new APlayer({
    container: document.getElementById('aplayer'),
    lrcType: 3,
    listFolded: false,      // 默认展开播放列表
    listMaxHeight: 500,     // 列表最大高度
    theme: '#b7daff',       // 播放器主题色
    audio: [
        {
            name: '等泪水飞作蝴蝶',
            artist: '杯糕P,星辰',
            url: '/music/files/等泪水飞作蝴蝶.mp3',   // 音频文件路径（后面会说怎么放）
            lrc: '/music/files/等泪水飞作蝴蝶.lrc'
        },
        {
            name: '回音',
            artist: 'COP,洛天依',
            url: '/music/files/回音.mp3',
            lrc: '/music/files/回音.lrc' 
        }
        // 想加更多歌，就复制上面这一段，粘贴到后面，注意逗号
    ]
});
</script>

<style>
  /* 让播放器在页面中间，好看一点 */
  #aplayer {
    margin: 30px auto;
    max-width: 600px;
    box-shadow: 0 4px 20px rgba(0,0,0,0.1);
    border-radius: 8px;
    overflow: hidden;
  }
  .page-title {
    text-align: center;
    font-size: 2em;
    margin-top: 20px;
    color: #333;
  }
</style>