<template>
  <div>
    <h1>Create an Event, {{ user.id }}</h1>
    created by {{ user.name }}
    <p>{{ getEventById(3) }}</p>
  </div>
</template>

<script>
import { mapState, mapGetters } from 'vuex'

export default {
  computed: {
    ...mapGetters(['getEventById']),
    ...mapState(['user', 'categories'])
  }
}
</script>

<style lang="scss" scoped></style>
