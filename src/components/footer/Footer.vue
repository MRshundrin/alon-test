<template>
	<footer id="footer" dir="rtl">
		<FooterContacts/>
		<FooterMenu/>
		<SecondFooter/>
	</footer>
</template>

<style lang="scss">
@import '@/variables.scss';


</style>

<script>

import FooterContacts from '@/components/footer/FooterContacts'
import FooterMenu from '@/components/footer/FooterMenu'
import SecondFooter from '@/components/footer/SecondFooter'


export default {
  name: 'footer-site',
  components: {
   FooterContacts, FooterMenu, SecondFooter
  }
}
</script>