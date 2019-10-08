<template>
  <div class="jumbotron">
      <h2>Mijn Projecten [Modals in development]</h2>
      <div class="row justify-content-center">
          <ProjectsCard v-for="project in projects" :key="project.id"
              :title="project.title"
              :link="project.link"
              :gitLink="project.gitLink"
              />
          </div>
      </div>
</template>

<script>
// @ is an alias to /src
import ProjectsCard from '@/components/elements/ProjectsCard.vue'

export default {
  name: 'home',
  components: {
    ProjectsCard
  },
  data () {
    return {
      projects: [
        {
          id: 1,
          title: 'Stumpel',
          link: 'https://rickscreations.nl/stumpel/',
          gitLink: 'https://github.com/RickHinfelaar/Stumpel-Application'
        },
        {
          id: 2,
          title: 'CommerceTool',
          link: 'https://rickscreations.nl/commercetool/',
          gitLink: 'https://github.com/RickHinfelaar/CommerceTool'
        },
        {
          id: 3,
          title: 'CommerceToool - Vue',
          link: 'https://rickscreations.nl/commercetool/vue',
          gitLink: 'https://github.com/RickHinfelaar/Stumpel-Application'
        },
        {
          id: 4,
          title: 'PortFolio',
          link: 'https://rickscreations.nl',
          gitLink: 'https://github.com/RickHinfelaar/Portfolio'
        }
      ]
    }
  }
}

</script>
