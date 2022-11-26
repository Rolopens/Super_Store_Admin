<template>
	<div>
		<!-- ADMIN VIEWS -->
		<AdminNavigationBar />
		<!-- <AdminHome /> -->
		<AdminOrders />
		<!-- <AdminProducts /> -->
		<!-- <AdminSales /> -->

		<!-- STAFF -->
		<!-- <StaffNavigationBar /> -->
		<!-- ARTIST -->
		<!-- <ArtistView /> -->
		<!-- PRODUCTION PERSONNEL -->
		<!-- MERCHANDISER -->
		<!-- CUSTOMER SERVICE -->
		<Footer />
	</div>
</template>

<script>
// ADMIN SCRIPTS
import AdminNavigationBar from "./components/Admin/AdminNavigationBar.vue";
// import AdminHome from "./components/Admin/AdminHome.vue";
import AdminOrders from "./components/Admin/AdminOrders.vue";
// import AdminProducts from "./components/Admin/AdminProducts.vue";
// import AdminSales from "./components/Admin/AdminSales.vue";
// STAFF
// import StaffNavigationBar from "./components/Staff/StaffNavigation.vue";
// import ArtistView from "./components/Staff/Artist.vue";
import Footer from "./components/Admin/Footer.vue";
export default {
	name: "App",
	components: {
		// ADMIN COMPONENTS
		AdminNavigationBar,
		// AdminHome,
		AdminOrders,
		// AdminProducts,
		// AdminSales,
		// STAFF COMPONENTS
		// StaffNavigationBar,
		// ArtistView,
		Footer,
	},
};
</script>

<style lang="scss">
// @import "@/styles/global-variables.scss";
@import "@/styles/global-variables.scss";
</style>
