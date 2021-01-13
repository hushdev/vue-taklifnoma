<template>
  <header>
    <div class="container">
      <div class="row">
        <a href="/" class="logo">Ftaklifnoma.uz </a>
        <ul class="menu">
          <li v-for="(path, index) in paths" :key="index">
            <a :href="path.href">{{ path.name }}</a>
          </li>
        </ul>
        <div class="change-lang">
          <span>RUS</span>
          <span>UZB</span>
        </div>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  el: "header",
  name: "header",
  data() {
    return {
      paths: [
        {
          href: "/",
          name: "главная",
        },
        {
          href: "/",
          name: "о нас",
        },
        {
          href: "/",
          name: "пригласительные",
        },
        {
          href: "/",
          name: "галерея работ",
        },
        {
          href: "/",
          name: "контакты",
        },
      ],
    };
  },
  methods: {
  }
};
</script>

<style lang="scss" scoped>
header {
  background: transparent;
  padding: 16px 0;
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 50;
  .container {
    .row {
      display: flex;
      align-items: center;
      a.logo {
        text-decoration: none;
        color: var(--white);
        font-family: "Proxima-Bold";
        font-size: 26px;
        margin-right: 37px;
      }
      .menu {
        display: flex;
        list-style-type: none;
        margin-top: 0;
        margin-bottom: 0;
        li {
          margin: 0 10px;
          &:first-child {
            margin: 0 10px 0 0;
          }
          &:last-child {
            margin: 0 0 0 10px;
          }
          a {
            color: var(--white);
            text-decoration: none;
            font-family: "Proxima-Bold";
            text-transform: uppercase;
            font-size: 14px;
          }
        }
      }
      .change-lang {
        margin-left: auto;
        span {
          color: var(--white);
          font-family: "Proxima-SemiBold";
          font-size: 14px;
          &:hover {
            cursor: pointer;
          }
          &:last-child {
            margin-left: 10px;
          }
        }
      }
    }
  }
}
</style>