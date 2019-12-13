<template>
  <div class="home">
    <div class="webBg"></div>
    <div class="navBar">
      <div class="item1 item" @click="linkTo('http://192.168.100.7/AppUpdate')">
        <img class="img1" src="./img/01.png" alt="">
        <img class="hoverimg1" src="./img/01-hover.png" alt="">
        <div class="name">总院HIS</div>
      </div>
      <div class="item2 item" @click="linkTo('http://192.168.103.22/AppUpdate')">
        <img class="img2" src="./img/02.png" alt="">
        <img class="hoverimg2" src="./img/02-hover.png" alt="">
        <div class="name">旧院HIS</div>
      </div>
      <div class="item3 item" @click="linkTo('http://192.168.102.9/AppUpdate')">
        <img class="img3" src="./img/03.png" alt="">
        <img class="hoverimg3" src="./img/03-hover.png" alt="">
        <div class="name">护理院养老</div>
      </div>
      <div class="item4 item" @click="linkTo('http://192.168.200.253/AppUpdate')">
        <img class="img4" src="./img/04.png" alt="">
        <img class="hoverimg4" src="./img/04-hover.png" alt="">
        <div class="name">护理院医保</div>
      </div>
      <div class="item5 item" @click="linkTo('http://192.168.200.253/AppUpdate')">
        <img class="img5" src="./img/05.png" alt="">
        <img class="hoverimg5" src="./img/05-hover.png" alt="">
        <div class="name">三水健翔</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'home',
  data () {
    return {
    }
  },
  methods: {
    linkTo (url) {
      return url
    }
  }
}
</script>

<style scoped>
.webBg {
  background: url('./img/BG1.jpg') no-repeat;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: -10;
  zoom: 1;
  background-size: cover;
  -webkit-background-size: cover;
  -o-background-size: cover;
  background-position: center 0;
}
.navBar {
  padding-top: 30vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
.item {
  margin: 1vh 2vw;
  width: 12vw;
  height: 30vh;
  cursor: pointer;
  display: flex;
  flex-direction: column;
}
img {
  width: 12vw;
}
.name {
  margin-top: 1vh;
  text-align: center;
  font-size: 1.8vw;
  font-weight: bold;
  color: #1eb0a8;
}
.hoverimg1,.hoverimg2,.hoverimg3,.hoverimg4,.hoverimg5 {
  display: none;
}
.item1:hover .img1 {
  display: none;
}
.item1:hover .hoverimg1 {
  display: block;
}
.item2:hover .img2 {
  display: none;
}
.item2:hover .hoverimg2 {
  display: block;
}
.item3:hover .img3 {
  display: none;
}
.item3:hover .hoverimg3 {
  display: block;
}
.item4:hover .img4 {
  display: none;
}
.item4:hover .hoverimg4 {
  display: block;
}
.item5:hover .img5 {
  display: none;
}
.item5:hover .hoverimg5 {
  display: block;
}
</style>
