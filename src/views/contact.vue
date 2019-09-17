<html>
  <head>
    <script src="https://cdn.jsdelivr.net/npm/vue/dist/vue.js"></script>
  </head>
  <body>
    <div id="app">
      <span v-html="msg"></span>
    </div>
  </body>
</html>
<script>
  var obj = {
    msg: '<span style="color:blue">HTMLコードとしてタグが判断され、青くなる</span>'
  }
 
  new Vue({
    el: '#app',
    data: obj
  })
</script>