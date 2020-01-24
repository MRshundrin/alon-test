<template>
	<main id="main">
		<Banner/>
    <Form/>
    <Areas/>
    <Recommendations/>
    <About/>
    <BlackBanner/>
    <MilitaryBanner/>
    <VideosSection/>
	</main>
</template>

<style lang="scss">
@import '@/variables.scss';
#main {
  position: relative;
}

</style>

<script>

import Banner from '@/components/main/BannerSection'
import Form from '@/components/main/ContactForm'
import Areas from '@/components/main/AreasOfPractice'
import Recommendations from '@/components/main/Recommendations'
import About from '@/components/main/About'
import BlackBanner from '@/components/main/BlackBanner'
import MilitaryBanner from '@/components/main/MilitaryBanner'
import VideosSection from '@/components/main/VideosSection'


export default {
  name: 'mainPart',
  components: {
   Banner, Form, Areas, Recommendations, About, MilitaryBanner, BlackBanner, VideosSection
  }
}
</script>