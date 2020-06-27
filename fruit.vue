<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<script src="https://cdn.staticfile.org/vue/2.2.2/vue.min.js"></script>
</head>
<body>
<div id="app">
  <button v-on:click="counter += 1">买一斤苹果</button>
  <button v-on:click="dragon += 1"> 买一个火龙果</button>
  <p>苹果买了 {{ counter }} 斤。火龙果买了 {{ dragon }} 个。</p>
	 <button v-on:click="pear += 1">买一斤梨子</button>
  <p>梨子买了 {{ pear}} 斤。</p>
  <button v-on:click="counter=0">初始化苹果</button>
   <button v-on:click="pear=0">初始化梨子</button>
	<button v-on:click="dragon=0">初始化火龙果</button>
	<button v-on:click="sum=pear*2+counter*3+dragon*5">算钱</button>
	<p>您应付款 {{sum}} 元。</p>
</div>

<script>
new Vue({
  el: '#app',
  data: {
    counter: 0,
	pear:0,
	dragon:0,
	sum:0  
  }
})
</script>
</body>
</html>
