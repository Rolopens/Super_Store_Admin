<template>
	<div class="margin-block-start page-margin-inline">
		<div class="admin-home-wrapper">
			<div class="admin-home-sales home-portion">
				<h1 class="fs-1300">Weekly Sales</h1>
				<div class="sales-container container-portion">
					<select v-model="salesSection">
						<option value="customer service">Customer Service</option>
						<option value="graphic artist">Graphic Artist</option>
						<option value="production">Production</option>
					</select>
					<div class="sales-selected" v-if="salesSection == 'customer service'">
						<div>
							<h3>Number of Orders</h3>
							<p>500,000.00</p>
						</div>
						<div>
							<h3>Revenue</h3>
							<p>PHP 1,000,000.00</p>
						</div>
						<div>
							<h3>Revenue Per Buyer</h3>
							<p>PHP 1,000,000.00</p>
						</div>
						<div>
							<h3>Number of Orders</h3>
							<p>PHP 1,000,000.00</p>
						</div>
						<div>
							<h3>Number of Customers</h3>
							<p>PHP 1,000,000.00</p>
						</div>
					</div>
					<div class="sales-selected" v-if="salesSection == 'graphic artist'">
						<div>
							<h3>TEST</h3>
							<p>500,000.00</p>
						</div>
						<div>
							<h3>Revenue</h3>
							<p>PHP 1,000,000.00</p>
						</div>
					</div>
					<div class="sales-selected" v-if="salesSection == 'production'">
						<div>
							<h3>TEST 2</h3>
							<p>500,000.00</p>
						</div>
						<div>
							<h3>Revenue</h3>
							<p>PHP 1,000,000.00</p>
						</div>
					</div>
				</div>
			</div>
			<div class="admin-home-best home-portion">
				<h1 class="fs-1300">Best Sellers</h1>
				<div class="best-container container-portion">
					<div>
						<h3>Supplies</h3>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
					</div>
					<div>
						<h3>Services</h3>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
						<p>PRODUCT HERE</p>
					</div>
				</div>
			</div>
			<div class="admin-top-customers home-portion">
				<h1 class="fs-1300">Top Customers</h1>
				<div class="customers-container container-portion">
					<div>
						<h3>Names</h3>
						<ol>
							<li>Isabel Ip</li>
							<li>Boyfriend of Isabel</li>
							<li>Dog of Isabel</li>
							<li>Rolo Pena</li>
							<li>Rafael Cruz</li>
						</ol>
					</div>
					<div>
						<h3>Revenue</h3>
						<ol>
							<li>1,000,000.00</li>
							<li>500,000.00</li>
							<li>250,000.00</li>
							<li>100,000.00</li>
							<li>50,000.00</li>
						</ol>
					</div>
				</div>
			</div>
			<div class="admin-customer-journey home-portion">
				<h1 class="fs-1300">Customer Journey</h1>
				<div class="journey-container container-portion">
					<div>
						<h3>Visits</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Added to Cart</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Proceed with Order</h3>
						<p>NUMBER HERE</p>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "AdminHome",
	data() {
		return {
			salesSection: "customer service",
		};
	},
};
</script>

<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Admin/admin-home.scss";
</style>
