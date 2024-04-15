<template>
  <div class="game_main">
    <!-- 群图片 -->
    <div class="game_QR">
      <div class="game_QR_title">
        <p>无尽冬日(冰霜启示录)</p>
        <p>TWC - 突出重围</p>
        <p>get through the close siege</p>
      </div>
      <div class="game_QR_erwei">
        <img src="@/assets/qunIMG/weixinImg.png" alt="" />
      </div>
      <div class="game_QR_QQ">
        <p>QQ群: 930401195</p>
      </div>
    </div>

    <!-- 背景透明图 -->
    <div class="game_bg_shade"></div>

    <!-- 背景图片 -->
    <div class="game_bg">
      <img src="@/assets/qunIMG/bf4.jpg" alt="" />
    </div>
  </div>
</template>

<script>
export default {
  name: "winter-game",
};
</script>

<style scoped>
.game_main {
  background: #000;
  height: 100vh;
  width: 100vw;
  position: relative;
}
.game_QR {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  z-index: 10;
  width: 40%;
  height: 50%;
  display: flex;
  flex-direction: column;
}

.game_QR_title {
  width: 100%;
  display: flex;
  flex-direction: column;
  align-items: center;
  color:#fff;
}
.game_QR_QQ{
  width:100%;
  display: flex;
  align-items: center;
  justify-content: center;
  color:#fff;
  font-weight:bolder;
  font-size:20px;
}
.game_QR_erwei{
  width:100%;
  display: flex;
  align-items: center;
  justify-content: center;
  flex:1;

}
.game_QR_erwei img{
  width:280px;
  height:280px;
}
.game_QR_title p:nth-child(1) {
  width: 60%;
  font-weight: bolder;
  font-size: 28px;
  padding: 10px 0;
  border-bottom: 1px solid rgb(165, 165, 165);
  display: flex;
  align-items: center;
  justify-content: center;
}
.game_QR_title p:nth-child(2) {
  width: 60%;
  font-weight: bolder;
  font-size: 28px;
  display: flex;
  align-items: center;
  justify-content: center;
  margin-top:20px;
}

.game_bg {
  width: 100%;
  height: 100%;
}
.game_bg_shade {
  position: absolute;
  top: 0;
  left: 0;
  background: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 100%;
  z-index: 2;
}
.game_bg img {
  width: 100%;
  height: 100%;
}
</style>
