<template>
  <div class="wrap">
    <div id="preview">
      <a
        href="https://si.geilicdn.com/wdseller1681912870-31210000018d8ee4db110a210370_2048_2048.jpg?w=800&h=800&cp=1"
        data-lg-size="800-800"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/wdseller1681912870-31210000018d8ee4db110a210370_2048_2048.jpg?w=800&h=800&cp=1"
        />
      </a>
      <a
        href="https://si.geilicdn.com/sceondhand1818984644-55340000018fbdfbd0cd0a2315ef_1282_1664.jpg?w=800&h=800&cp=1"
        data-lg-size="800-800"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/sceondhand1818984644-55340000018fbdfbd0cd0a2315ef_1282_1664.jpg?w=800&h=800&cp=1"
        />
      </a>
      <a
        href="https://si.geilicdn.com/sceondhand1207738034-52a60000018fbe056e540a2102c5_827_827.jpg?w=800&h=800&cp=1"
        data-lg-size="800-800"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/sceondhand1207738034-52a60000018fbe056e540a2102c5_827_827.jpg?w=800&h=800&cp=1"
        />
      </a>
      <a
        href="https://si.geilicdn.com/sceondhand1784134191-6dba000001906bc265450a21146b_1536_2048.jpg?w=800&h=800&cp=1"
        data-lg-size="800-800"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/sceondhand1784134191-6dba000001906bc265450a21146b_1536_2048.jpg?w=800&h=800&cp=1"
        />
      </a>
      <a
        href="https://si.geilicdn.com/weidian1681003977-3a330000018f19734bcc0a20e35c_1728_2304.jpg?w=800&h=800&cp=1"
        data-lg-size="800-800"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/weidian1681003977-3a330000018f19734bcc0a20e35c_1728_2304.jpg?w=800&h=800&cp=1"
        />
      </a>
      <!-- <a
        data-lg-size="827-827"
        data-video='{"source": [{"src":"https://v.geilicdn.com/video/svpk1164786033-76ad00000173c8609b7c0a217216_720_720.mp4.f20.mp4", "type":"video/mp4"}], "tracks": [{"src": "{/videos/title.txt", "kind":"captions", "srclang": "en", "label": "English", "default": "true"}], "attributes": {"preload": false, "playsinline": true, "controls": true}}'
        data-poster="https://si.geilicdn.com/sceondhand1207738034-52a60000018fbe056e540a2102c5_827_827.jpg"
      >
        <img
          class="box"
          src="https://si.geilicdn.com/sceondhand1207738034-52a60000018fbe056e540a2102c5_827_827.jpg"
        />
      </a> -->
    </div>
  </div>
</template>
<script lang="ts" setup>
import Lightgallery from "lightgallery";
import { onMounted } from "vue";
import lgZoom from "lightgallery/lib/plugins/zoom/lg-zoom";
const start = () => {
  //
  const el = document.getElementById("preview");
  if (!el) return;
  const instance = new Lightgallery(el, {
    plugins: [lgZoom],
    swipeThreshold: 0,
    speed: 0,
    thumbnail: false,
    zoom: true,
    slideDelay: 0,
    zoomFromOrigin: true,
    autoplayFirstVideo: true,
    autoplayVideoOnSlide: true,
    controls: false,
    preload: 4,
  });
};
onMounted(() => {
  start();
});
</script>
<style lang="less" scoped>
.box {
  width: 150px;
}
</style>
