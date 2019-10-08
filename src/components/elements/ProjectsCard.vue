<template>
  <div class="card project col-md-3">
    <a :href="link" target="_blank">
      <h3 class="card-title">{{title}}</h3>
    </a>
    <br/>
    <a :href="gitLink" target="_blank">
      <h3 class="card-title">Github</h3>
    </a>
    </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    link: String,
    gitLink: String
  }
}
</script>
