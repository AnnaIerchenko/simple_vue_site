<!-- eslint-disable vue/multi-word-component-names -->
<!-- eslint-disable-next-line vue/multi-word-component-names -->
<template>
  <footer class="footer footer_bg">
    <div class="container">
      <div class="row">
       <FooterIcons />
       <FooterNav :footerMenu="footerMenu"/>
       <FooterClient :footerMenuClient="footerMenuClient"/>
       <FooterContacts />
      </div>
      Footer
    </div>
  </footer>
</template>

<script> 
import { menuList, menuClient} from '../../constants/MenuLinks'
import FooterIcons from './FooterIcons.vue'
import FooterNav from './FooterNav.vue'
import FooterClient from './FooterClient.vue'
import FooterContacts from './FooterContacts.vue'

  export default {
    data() {
      return {
        footerMenu: menuList,
        footerMenuClient: menuClient,
      }
    },
    components: {
      FooterIcons, 
      FooterNav,
      FooterClient,
      FooterContacts
    }
  }
</script>