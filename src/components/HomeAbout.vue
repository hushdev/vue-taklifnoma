<template>
  <div class="container about">
    <div class="row">
      <div class="col-lg-7">
        <H2 text="О нас" />
        <P :text="pText" />
      </div>
      <img :src="imgUrl" alt="Фотография администратора" class="col-lg-5" />
    </div>
  </div>
</template>

<script>
import H2 from "@/components/H2";
import P from "@/components/Paragraph";
import Photo from "@/assets/img/home-about-item.png";
export default {
  components: { H2, P },
  data() {
    return {
      pText: `Студия FTaklifnoma занимается изготовлением свадебной полиграфии. 
            Профессионализм дизайнеров поможет сделать вашу свадьбу незабываемой. Важной частью каждой свадьбы являются пригласительные – именно 
            они сообщают гостям дату, время, место проведения торжества, стиль, предпочтительный стиль в одежде и множество других пожеланий.
            Мы стремимся быть одними из лучших на рынке свадебной полиграфии и прикладываем для этого большие усилия`,
      imgUrl: Photo,
    };
  },
};
</script>

<style lang="scss" scoped>
.about {
  padding: 30px 0 0 0;
  h2 {
    margin-bottom: 25px;
  }
}
</style>