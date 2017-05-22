<template>
	<div id="input">
		<div @input="input2">
			
			<Input ref="input" size="small" name="dd" placeholder="placeholder" @input="input2">
				<span slot="prepend">dsssss</span>
			</Input>

			<Input ref="input" name="dd" placeholder="placeholder">
				<span slot="prepend">dsssss</span>
			</Input>
		</div>
	</div>
</template>
<script>

	export default {
		data,
		methods: {
			input2(i,l){
				console.log(i)
				console.log(l)
			}
		},
		mounted,
	}
	function data (){
		return {

		}
	}
	function mounted() {
		var _vm = this;
		console.log(_vm.$refs)
		setTimeout(function(){
			// _vm.$refs.input.$el.innerHTML='<div>ss</div>'
			
		},100)

	}

	// methods

</script>
<style>
	
</style>