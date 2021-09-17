<template>
  <div>
    <input
        id="cameraFileInput"
        type="file"
        accept="image/*"
        capture="environment"
        @change="previewFiles"
      />
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  methods: {
  previewFiles(event) {
    console.log(event.target.files);
  }
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
