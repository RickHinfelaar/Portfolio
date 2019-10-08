<template>
  <div class="jumbotron">
      <h2>Mijn vaardigheden [Modals in development]</h2>
      <div class="row justify-content-center">
          <SkillsCard v-for="skill in skills" :key="skill.id"
              :title="skill.title"
              />
          </div>
      </div>
</template>

<script>
// @ is an alias to /src
import SkillsCard from '@/components/elements/SkillsCard.vue'

export default {
  name: 'home',
  components: {
    SkillsCard
  },
  data () {
    return {
      skills: [
        {
          id: 1,
          title: 'Vue.js',
          description: 'Html is bla bla'
        },
        {
          id: 2,
          title: 'HTML',
          discription: 'Javascript is bla bla'
        },
        {
          id: 3,
          title: 'CSS - Sass',
          discription: 'Javascript is bla bla'
        },
        {
          id: 4,
          title: 'Javascript',
          discription: 'Javascript is bla bla'
        },
        {
          id: 5,
          title: 'jQuery',
          discription: 'Javascript is bla bla'
        },
        {
          id: 6,
          title: 'NPM',
          discription: 'Javascript is bla bla'
        },
        {
          id: 7,
          title: 'Git',
          discription: 'Javascript is bla bla'
        },
        {
          id: 8,
          title: 'Bootstrap',
          discription: 'Javascript is bla bla'
        },
        {
          id: 9,
          title: 'PHP',
          discription: 'Javascript is bla bla'
        },
        {
          id: 10,
          title: 'WordpPress',
          discription: 'Javascript is bla bla'
        },
        {
          id: 11,
          title: 'SCRUM',
          discription: 'Javascript is bla bla'
        },
        {
          id: 12,
          title: 'Photoshop',
          discription: 'Javascript is bla bla'
        },
        {
          id: 13,
          title: 'MS Office',
          discription: 'Javascript is bla bla'
        },
        {
          id: 14,
          title: 'Premiere Pro',
          discription: 'Javascript is bla bla'
        }
      ]
    }
  }
}

</script>
