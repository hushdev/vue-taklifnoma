<template>
  <div class="col-lg-3">
    <div class="card">
      <img :src="imgUrl" alt="" />
      <div class="content">
        <h3>{{ title }}</h3>
        <p>От {{ cost }} сум</p>
      </div>
    </div>
  </div>
</template>

<script>
import P from "@/components/Paragraph";

export default {
  el: ".card",
  props: {
    title: String,
    cost: Number,
    imgUrl: String,
  },
};
</script>

<style lang="scss" scoped>
.col-lg-3 {
  .card {
    background: var(--white);
    padding: 21px 21px 31px 21px;
    border-radius: 10px;
    border: 1px solid #ececec;
    max-width: 224px;
    width: 100%;
    transition: .3s;
    height: 320px;

    display: flex;
    flex-direction: column;
    justify-content: space-between;

    &:hover {
      transform: scale(.95);
    }

    * {
      overflow: hidden;
    }
    img {
      width: 100%;
      max-height: 187px;
      height: auto;
    }
    .content {
      margin-top: 30px;
      h3 {
        color: var(--blue);
        font-size: 23px;
        font-family: "Proxima-Bold";
        font-weight: 700;
      }
      p {
      }
    }
  }
}
</style>