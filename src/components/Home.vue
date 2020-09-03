<template >
	<div class="box-start">
		заглушка
	</div>
</template>
<script >
	export default {
		computed: {
			total() {
				return this.$store.getters.total;
			}
		}
	}
</script>
<style>
	.t1 {
	font-size: 40px;
	}
	.t2 {
		margin-top: -12px;
		margin-bottom: 16px;
	font-size: 20px;
	}
	.box-start {
    margin: 0;
}
   .btn-main {
    background-color: transparent;
    border:1px solid ;
    border-color: black;
    font-size: 12px;
    color: black;
    text-decoration: none;
    padding: 0;
   }
   .btn-main:hover {
     background-color: black;
    color: white;
    text-decoration: none;
}
</style>