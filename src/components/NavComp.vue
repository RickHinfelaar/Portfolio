<template>
  <div class="home">
    <div class="container-fluid">
      <div class="row justify-content-center">
        <Card
            :title="me.title"
            :router="me.router"/>
        <Card
            :title="skills.title"
            :router="skills.router"/>
        <Card
            :title="projects.title"
            :router="projects.router"/>
        </div>
      </div>
  </div>
</template>

<script>
// @ is an alias to /src
import Card from '@/components/elements/NavCard.vue'
export default {
  name: 'home',
  components: {
    Card
  },
  data () {
    return {
      me: {
        title: 'About me',
        router: '/'
      },
      skills: {
        title: 'Skills',
        router: '/skills'
      },
      projects: {
        title: 'Projects',
        router: '/projects'
      }
    }
  }
}
</script>
