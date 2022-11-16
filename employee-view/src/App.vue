<template>
	<div>
		<NavigationBar />
		<Footer />
	</div>
</template>

<script>
import NavigationBar from "./components/NavigationBar.vue";
import Footer from "./components/Footer.vue";
export default {
	name: "App",
	components: {
		NavigationBar,
		Footer,
	},
};
</script>

<style lang="scss">
@import "@/styles/global-variables.scss";
</style>
