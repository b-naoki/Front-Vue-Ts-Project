<template>
  <header class="header">
    <h1>{{ title }}</h1>
    <nav>
      <ul>
        <li><a href="#">ホーム</a></li>
        <li><a href="#">資格一覧</a></li>
        <li><a href="#">受講者の声</a></li>
        <li><a href="#">お問い合わせ</a></li>
      </ul>
    </nav>
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";

export default defineComponent({
  name: "AppHeader",
  props: {
    title: {
      type: String,
      default: "資格取得サイト",
    },
  },
});
</script>

<style scoped lang="scss">
.header {
  background-color: #2c3e50; /* ダークグリーン */
  color: white;
  padding: 20px;
  text-align: center;

  h1 {
    margin: 0;
    font-size: 2.5em;
    font-weight: bold;
  }

  nav {
    margin-top: 15px;

    ul {
      list-style-type: none;
      padding: 0;

      li {
        display: inline-block;
        margin: 0 15px;

        a {
          color: #42b983; /* 明るいグリーン */
          text-decoration: none;
          font-weight: bold;

          &:hover {
            text-decoration: underline; /* ホバー時に下線を追加 */
          }
        }
      }
    }
  }
}
</style>
