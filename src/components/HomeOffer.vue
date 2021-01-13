<template>
  <div class="home-offer">
    <div class="container">
      <div class="row">
        <div class="col-lg-7">
          <h1>Пригласительные на свадьбу</h1>
          <P
            text="А также все виды полиграфических услуг в самом центре Ташкента"
          />
          <Btn text="Связаться" />
        </div>
      </div>
      <div class="row">
        <div class="col-lg-6">
          <div class="item">
            Стоимость от
            <p><span>2000</span> Сум</p>
          </div>
          <div class="item">
            Тираж от
            <p><span>1</span> Штуки</p>
          </div>
          <div class="item">
            Работаем уже
            <p><span>6</span> Лет</p>
          </div>
        </div>
        <div class="col-lg-1">
          <a href="">
            <img :src="telegram" />
          </a>
          <a href="">
            <img :src="instagram" />
          </a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import P from "@/components/Paragraph";
import Btn from "./Btn.vue";
import Instagram from "@/assets/img/instagram.svg";
import Telegram from "@/assets/img/telegram.svg";

export default {
  components: { P, Btn },
  data() {
    return {
      instagram: Instagram,
      telegram: Telegram,
    };
  },
};
</script>

<style lang="scss" scoped>
.home-offer {
  background: url("../assets/img/home-offer-bg.jpg") no-repeat center;
  background-size: cover;
  background-attachment: fixed;
  padding: 226px 0 35px 0;
  .container {
    .row {
      .col-lg-7 {
        h1 {
          font-size: 70px;
          font-family: "Proxima-Bold";
          margin-bottom: 40px;
          color: var(--white);
        }
        p {
          color: #d7d7d7;
          margin-bottom: 40px;
          font-size: 32px;
          font-family: "Proxima-SemiBold";
        }
      }
    }
    .row:last-child {
      margin-top: 251px;
      display: flex;
      justify-content: space-between;
      align-items: center !important;
      .col-lg-6 {
        display: flex;
        justify-content: space-between;
        .item {
          font-family: "Proxima-Bold";
          font-size: 18px;
          color: var(--white);
          max-height: 100px;
          overflow: hidden;
            
          p {
            span {
              color: var(--blue);
              font-family: "Proxima-Black";
              font-weight: 900;
              font-size: 63px;
              text-shadow: 0 2px 0 var(--white);
            }
          }
        }
      }
      .col-lg-1 {
        margin-top: auto;
        a:last-child {
          margin-left: 10px;
        }
      }
    }
  }
}
</style>