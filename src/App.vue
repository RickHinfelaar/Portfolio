<template>
    <div id="app">
      <Header class="header"/>
      <transition
        name="fade"
        mode="out-in"
       @beforeLeave="beforeLeave"
       @enter="enter"
       @afterEnter="afterEnter"
      >
        <router-view/>
      </transition>
      <Footer/>
    </div>
</template>

<script>
import Header from '@/views/Header.vue'
import Footer from '@/components/Footer.vue'

export default {
  name: 'app',
  components: {
    Header,
    Footer
  },
  data () {
    return {
      prevHeight: 0
    }
  },
  methods: {
    beforeLeave (element) {
      this.prevHeight = getComputedStyle(element).height
    },
    enter (element) {
      const { height } = getComputedStyle(element)

      element.style.height = this.prevHeight

      setTimeout(() => {
        element.style.height = height
      })
    },
    afterEnter (element) {
      element.style.height = 'auto'
    }
  }
}
</script>

<style lang="scss">
@import '@/assets/css/style.scss';
</style>
