<template>
	<div id="app">
    <h1 align="center">Welcome.....</h1>
    <hr>
    <textarea rows="10" v-model="text" class="textarea"></textarea>
    <br>
		<text-reader @load="text = $event"></text-reader>
	</div>
</template>

<script>
import TextReader from "./TextReader";

export default {
  name: "app",
  data: () => ({ text: "" }),
  components: {
    TextReader
  }
};
</script>
<style type="text/css">
  .textarea{
    background-color: #FFCECE;
    border:5px;
  }
</style>
