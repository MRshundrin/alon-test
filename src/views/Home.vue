<template>
  <div class="home">
   <Header/>
   <Main/>
   <Footer/>
  </div>
</template>

<script>

import Header from '@/components/header/Header'
import Main from '@/components/main/Main'
import Footer from '@/components/footer/Footer'

export default {
  name: 'home',
  components: {
   Header, Main, Footer
  }
}
</script>
