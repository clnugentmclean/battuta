---
title: "StoryMap"
layout: single
permalink: /maps/storymap/
---
<div id="storymap-wrap">
  <iframe id="storymap-frame" src="https://uploads.knightlab.com/storymapjs/d1ee5d64be1b87b46201fa01d2973aa8/practice/index.html" frameborder="0" width="100%"></iframe>
</div>

<script>
  function sizeStoryMap() {
    var frame = document.getElementById('storymap-frame');
    if (!frame) return;
    var top = frame.getBoundingClientRect().top + window.scrollY;
    var height = window.innerHeight - top;
    frame.style.height = Math.max(height, 500) + 'px'; // 500px floor so it never gets too cramped
  }
  window.addEventListener('load', sizeStoryMap);
  window.addEventListener('resize', sizeStoryMap);
</script>