<template>
	<div class="flex flex-col gap-2 justify-center items-center mt-[20%]">
		<strong>{{ name }}</strong>
		<p>Explore <a target="_blank" rel="noopener noreferrer" href="https://ionicframework.com/docs/components">UI Components</a></p>
		<div class="flex gap-2">
			<Button label="Button A"></Button>
			<Button label="Button B"></Button>
			<Button label="Button C"></Button>
		</div>
	</div>
</template>

<script setup lang="ts">
	import Button from "primevue/button"

	defineProps({
		name: String
	})
</script>

<style scoped>
	#container {
		text-align: center;
		position: absolute;
		left: 0;
		right: 0;
		top: 50%;
		transform: translateY(-50%);
	}

	#container strong {
		font-size: 20px;
		line-height: 26px;
	}

	#container p {
		font-size: 16px;
		line-height: 22px;
		color: #8c8c8c;
		margin: 0;
	}

	#container a {
		text-decoration: none;
	}
</style>
