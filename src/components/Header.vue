<template>
  <div>
  <nav class="navbar navbar-expand-lg bg-body-tertiary">
  <div class="container">
    <a class="navbar-brand logo" href="/">
      <img src="../assets/images/icons/logo.png" alt="logo"/>
    </a>
    <div class="collapse collapse-fontsize navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0">
        <li class="nav-item menu-link" v-for="(menu, index) in headerMenuList" :key="index">
          <router-link class="nav-link  active" aria-current="page" :to="menu.path">
          {{ menu.name }}
          </router-link>
        </li>
      </ul>
      <div class="icons">
        <a href="https://www.facebook.com/" target="_blank"><img src="../assets/images/icons/f.png" alt=""/></a>
        <a href="https://www.pinterest.ru/" target="_blank"><img src="../assets/images/icons/p.png" alt=""/></a>
        <a href="https://www.instagram.com/" target="_blank"><img src="../assets/images/icons/insta.png" alt=""/></a>
        <a href="https://myaccount.google.com/" target="_blank"><img src="../assets/images/icons/g+.png" alt=""/></a>
      </div>
    </div>
  </div>
</nav>
</div>
</template>

<script>
import { menuList} from '../constants/MenuLinks'

export default {
  name: 'HeaderWorld',
  props: {
    msg: String,
  },
  data() {
    return {
      headerMenuList: menuList,
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/layouts/index.scss";
.navbar {
  height: 90px;
}  
.navbar-nav {
  height: 94px;
}
.logo {
    padding-right: 180px;
  }
  .collapse-fontsize {
    font-size: 18px;
  }
  .menu-link {
    padding: 25px 30px;

    &:hover {
      background: gray;
    }
  }
  .icons {
    a {
      width: 30px;
      height: 30px;
      text-align: center;
      border: 1px solid $gray;
      border-radius: 50%;
      margin-right: 10px;
      display: inline-block;
    }
  }
</style>
