<template>
    <PetTable
        :pets="dogs"
        species="doog" />
</template>

<script>
import { mapState } from 'vuex'
import PetTable from '@/components/petTable.vue'

export default {
  data () {
    return {
    }
  },
  components: {
    PetTable
  },
  computed: {
    ...mapState([
      'dogs'
    ])
  }
}
</script>
