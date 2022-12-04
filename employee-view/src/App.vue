<template>
	<div>
		<!-- ADMIN VIEWS -->
		<!-- <AdminNavigationBar /> -->
		<!-- <AdminHome /> -->
		<!-- <AdminOrders /> -->
		<!-- <AdminProducts /> -->
		<!-- <AdminSales /> -->

		<!-- STAFF -->
		<StaffNavigationBar />
		<!-- ARTIST -->
		<!-- <ArtistView /> -->
		<!-- PRODUCTION PERSONNEL -->
		<!-- <ProductionView /> -->
		<!-- MERCHANDISER -->
		<!-- <MerchandiserProducts /> -->
		<!-- <MerchandiserOrders /> -->
		<!-- CUSTOMER SERVICE -->
		<CSOrders />
		<Footer />
	</div>
</template>

<script>
// ADMIN SCRIPTS
// import AdminNavigationBar from "./components/Admin/AdminNavigationBar.vue";
// import AdminHome from "./components/Admin/AdminHome.vue";
// import AdminOrders from "./components/Admin/AdminOrders.vue";
// import AdminProducts from "./components/Admin/AdminProducts.vue";
// import AdminSales from "./components/Admin/AdminSales.vue";
// STAFF
import StaffNavigationBar from "./components/Staff/StaffNavigation.vue";
// import ArtistView from "./components/Staff/Artist/Artist.vue";
// import ProductionView from "./components/Staff/Production Personnel/ProductionPersonnel.vue";
// import MerchandiserProducts from "./components/Staff/Merchandiser/MerchandiserProducts.vue";
// import MerchandiserOrders from "./components/Staff/Merchandiser/MerchandiserOrders.vue";
import CSOrders from "./components/Staff/Customer Service/CSOrders.vue";
import Footer from "./components/Admin/Footer.vue";
export default {
	name: "App",
	components: {
		// ADMIN COMPONENTS
		// AdminNavigationBar,
		// AdminHome,
		// AdminOrders,
		// AdminProducts,
		// AdminSales,
		// STAFF COMPONENTS
		StaffNavigationBar,
		// ArtistView,
		// ProductionView,
		// MerchandiserProducts,
		// MerchandiserOrders,
		CSOrders,
		Footer,
	},
};
</script>

<style lang="scss">
// @import "@/styles/global-variables.scss";
@import "@/styles/global-variables.scss";
</style>
