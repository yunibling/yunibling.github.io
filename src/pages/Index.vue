<template>
  <q-page class="">
    <div class="text-h1 q-pb-md shadow-1 cursor-pointer">yunibling</div>
    <div class="box">
      <q-btn color="red-3" text-color="black" label="button" icon="mail" outline :loading="loading" @click="onClick" />
      <q-input v-model="text" @input="onInput" label="name" />
    </div>
  </q-page>
</template>

<style lang="sass">
.box
  outline: 1px solid red
</style>

<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      loading: false,
      text: ''
    }
  },
  methods: {
    onClick () {
      this.loading = true
    },
    onInput () {
      console.log(this.text)
    }
  }
}
</script>
