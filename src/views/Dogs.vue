<template>
  <PetTable :pets="dogs" species="Dogs" />
</template>

<script>
import { mapState } from "vuex";
import PetTable from "@/components/PetTable.vue"
export default {
  components: {
    PetTable
  },
  data() {
    return {};
  },
  computed: {
    ...mapState(["dogs"])
  }
};
</script>
