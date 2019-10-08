<template>
  <div class="card skill col-xl-2">
      <h3 class="card-title skill">{{title}}</h3>
  </div>
</template>

<script>
export default {
  name: 'Card',
  props: {
    title: String
  }
}
</script>
