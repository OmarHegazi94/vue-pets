<template>
    <div id="dogs">
        <h1 class="mb-3">Dogs for Adoption</h1>
        <b-table striped hover :items="dogs">
          <template #cell(name)="data">
            <router-link :to="`/pets/dogs/${data.index}`">
              {{ data.value }}
            </router-link>
          </template>
        </b-table>
    </div>
</template>

<script>
import { mapState } from 'vuex'

export default {
  data () {
    return {}
  },
  computed: {
    ...mapState([
      'dogs'
    ])
  }
}
</script>
