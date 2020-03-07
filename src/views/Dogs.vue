<template>
  <PetTable :pets="dogs" species="Dogs" />
 
</template>

<script>
import { mapState } from "vuex";
export default {
  data() {
    return {};
  },
  computed: {
    ...mapState(["dogs"])
  }
};
</script>
