<template>
	<header class="primary-header bg-primary">
		<div class="nav-wrapper">
			<div class="logo">
				<a href="#"
					><img src="../../assets/whitelogo.svg" alt="Super Store Logo"
				/></a>
			</div>
			<a href="#" class="toggle-nav">
				<i class="fa-solid fa-bars" @click="toggleNav"></i>
			</a>
			<div class="mobile-container" v-show="mobile">
				<div class="mobile-menu">
					<div class="store-options">
						<ul class="flex-row">
							<li><a href="#">Home</a></li>
							<li><a href="#">Products</a></li>
							<li><a href="#">Orders</a></li>
							<li><a href="#">Sales</a></li>
						</ul>
					</div>
				</div>
			</div>
		</div>
	</header>
</template>

<script>
export default {
	name: "NavigationBar",
	data() {
		return {
			mobile: true,
			mobileNav: true,
			windowWidth: null,
		};
	},
	created() {
		window.addEventListener("resize", this.checkScreen);
		this.checkScreen();
	},
	methods: {
		toggleNav() {
			this.mobile = !this.mobile;
		},

		checkScreen() {
			this.windowWidth = window.innerWidth;
			if (this.windowWidth <= 1280) {
				this.mobile = false;
				return;
			}

			this.mobile = true;
			this.mobileNav = false;
		},
	},
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Admin/navigationbar.scss";
</style>
