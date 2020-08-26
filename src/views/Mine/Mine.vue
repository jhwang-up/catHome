<template>
  <div class="mine">
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <div class="user-info-box">
      <div class="header">
        <div class="top-icon">
          <div class="left">
            <img src="https://sabotdata.oss-cn-beijing.aliyuncs.com/cathome/help.png" alt />
          </div>
          <div class="right">
            <img src="https://sabotdata.oss-cn-beijing.aliyuncs.com/cathome/setting.png" alt />
            <img src="https://sabotdata.oss-cn-beijing.aliyuncs.com/cathome/message.png" alt />
          </div>
        </div>
        <div class="user-info">
          <div class="info-left">
            <img src="../../assets/mine/user-pic.svg" alt />
          </div>
          <div class="info-right">
            <div class="nick">鸭嘴兽泰瑞</div>
            <div class="sign">主人太懒了，什么也没有留下</div>
          </div>
        </div>
      </div>
    </div>
    <div class="my-order">
      <div>我的订单</div>
      <div>查看全部</div>
    </div>
  </div>
</template>
<style lang="less" scoped>
// 这里用100vh是否ok？？ padding如何设置多少？此处需要引用px转vw  其中px是蓝湖那边读取的值，宽度是设置尺寸；
// 思考下背景图切成多大和代码咋写//。。。。
.mine {
  display: flex;
  flex-direction: column;
  .user-info-box {
    height: 38vh;
    background-image: url("../../assets/mine/bg.png");
    background-size: cover;
    background-repeat: no-repeat;
    color: white;
    padding: 20px 15px;
    .header {
      .top-icon {
        display: flex;
        flex: row;
        justify-content: space-between;
        align-content: center;
        img {
          width: 24px;
          height: 24px;
        }
        .right {
          // display: flex;
          // flex: row;
          // justify-content: space-between;
          img {
            margin-left: 15px;
          }
        }
      }
      .user-info {
        display: flex;
        // justify-content: center;
        align-items: center;
        padding-top: 20px;
        .info-left {
          img {
            width: 70px;
          }
        }
        .info-right {
          margin-left: 10px;
          text-align: left;
        }
      }
    }
  }

  .my-order {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px;
  }
}
</style>
<script>
// @ is an alias to /src
// import HelloWorld from "@/components/HelloWorld.vue";

export default {
  name: "Mine",
  components: {
    // HelloWorld
  },
  data() {
    return {
      // imgUrl:''
    };
  }
};
</script>
