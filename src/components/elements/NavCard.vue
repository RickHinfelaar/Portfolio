<template>
  <div class="card nav col-md-3">
    <router-link :to="router">
      <h3 class="card-title nav">{{title}}</h3>
    </router-link>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String,
    router: String
  }
}
</script>
