<template>

    <div>
        <BaseAlert
          v-if="showAlert"
          :variant="variant"
          @close="onClose()"
        >
            {{ text }}
        </BaseAlert>
    </div>
</template>

<script>

import BaseAlert from '@/components/BaseAlert.vue'

export default {
  name: 'App',
  components: { BaseAlert },
  data(){
    return {
      showAlert: true,
      variant: 'success',
      text: 'Seu formulário foi enviado com sucesso!',
    }
  },
  beforeUpdate() {},
  updated() {},
  beforeCreate() {},
  created() {},
  beforeMount() {},
  watch: {},
  computed: {},
  methods: {
    onClose(){
        this.showAlert = false
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
