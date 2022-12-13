<template>
	<div class="backdrop">
		<div class="modal">
			<h1>{{ header }}</h1>
			<p>{{ text }}</p>
		</div>
	</div>
</template>

<script>
	
	export default {
		props:['header','text']
	}

</script>

<style scoped>

	.modal{
		width:400px;
		padding:20px;
		margin:100px auto;
		background-color:white;
		border-radius:10px;
	}

	.backdrop{
		top:0px;
		position:fixed;
		background:rgb(0,0,0,0.5);
		width:100%;
		height:100%;
	}
	h1{
		color:#03cfb4;
		padding:0px;
		border:none;
	}
</style>