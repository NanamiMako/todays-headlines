	<template>
  <div class="video-container">
    <van-cell is-link @click="showPopup">展示弹出层</van-cell>
    <van-popup v-model="show" round closeable position="bottom" :style="{ height: '75%' }">内容</van-popup>
  </div>
</template>

		<script>
export default {
  name: 'VideoPage',
  data () {
    return {
      show: false,
    };
  },

  methods: {
    showPopup () {
      this.show = true;
    },
  },
}
</script>

		<style scoped></style>