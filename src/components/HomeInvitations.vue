<template>
  <div class="home-invitations">
    <div class="container">
      <H2 text="Пригласительные" />
      <div class="row">
        <Card
          v-for="(card, index) in cards"
          :key="index"
          :title="card.title"
          :cost="card.cost"
          :imgUrl="card.imgUrl"
        />
      </div>
    </div>
  </div>
</template>

<script>
import Card from "@/components/InvitationCard";
import H2 from "./H2";

import CardItem1 from "@/assets/img/cardItem1.png";
import CardItem2 from "@/assets/img/cardItem2.png";
import CardItem3 from "@/assets/img/cardItem3.png";
import CardItem4 from "@/assets/img/cardItem4.png";

export default {
  components: { Card, H2 },
  data() {
    return {
      cards: [
        {
          title: "Standart",
          cost: 2000,
          imgUrl: CardItem1,
        },
        {
          title: "Kristall",
          cost: 8000,
          imgUrl: CardItem2,
        },
        {
          title: "Armoni",
          cost: 10000,
          imgUrl: CardItem3,
        },
        {
          title: "Erdem",
          cost: 12000,
          imgUrl: CardItem4,
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
.home-invitations {
  background: url("../assets/img/home-offer-bg.jpg") no-repeat center;
  background-size: cover;
  background-attachment: fixed;
  padding: 60px 0;
  .container {
    h2 {
      color: var(--white);
      margin-bottom: 45px;
      text-shadow: 0 2px 0 var(--blue);
    }
  }
}
</style>