<template>
  <section>
    <p class="text-right pa-2">{{ time }}</p>
  </section>
</template>

<script>
export default {
  data() {
    return {
      time: "",
    };
  },
  mounted() {
    setInterval(this.setTime, 1000);
  },
  methods: {
    setTime() {
      let now = new Date();
      let mon = now.getMonth() + 1;
      let day = now.getDate();
      let hour = now.getHours();
      let min = now.getMinutes();
      let sec = now.getSeconds();
      this.time = `${mon} 月 ${day} 日 ${hour} 點 ${min} 分 ${sec} 秒`;
    },
  },
};
</script>

<style></style>
