<template>
  <div class="col">
    <h3 class="footer__title">Contact Us</h3>
      <ul class="footer__list footer__list_capitalize">
        <li>
          <p>240 Central Park, London OR 10819</p>
        </li>
        <li>
          <p>FreePhone: +1 880 550 6500</p>
          <p>TelePhone: +1 880 550 6500</p>
          <p>FAX: +1 880</p>
        </li>
        <li>
          <a class="footer__link footer__link_red footer__link_underline" href="mailto:info@realhome.com" target="_blank">
            <p>info@realhome.com</p>
          </a>
        </li>
      </ul>
  </div>
</template>

<script>

export default {
    props: {
        footerMenu: {
         type: Array,
         required: true
        }
      }
  }
</script>
