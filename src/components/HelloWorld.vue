<template>
  <canvas id="c" width="500" height="300" style="border: 1px solid #ccc">
  </canvas>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  mounted() {
    const cnv = document.getElementById('c');
    const cxt = cnv.getContext('2d');

    cxt.moveTo(20, 100);
    cxt.lineTo(200, 100);

    cxt.moveTo(20, 120.5);
    cxt.lineTo(200, 120.5);

    // cxt.moveTo(50, 50);
    // cxt.lineTo(200, 50);
    // cxt.lineWidth = 10;
    // cxt.strokeStyle = 'pink';
    // cxt.lineCap = 'round';

    // cxt.moveTo(200, 50);
    // cxt.lineTo(200, 200);

    // cxt.moveTo(50, 50);
    // cxt.lineTo(50, 200);

    // cxt.moveTo(50, 200);
    // cxt.lineTo(200, 200);
    cxt.stroke();
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
