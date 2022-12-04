<template>
	<div class="margin-block-start page-margin-inline">
		<div class="admin-home-wrapper">
			<AveProcessing />
			<div class="admin-home-sales home-portion">
				<h1 class="fs-1300">Weekly Sales</h1>
				<div class="sales-container container-portion">
					<select v-model="salesSection">
						<option value="customer service">Customer Service</option>
						<option value="graphic artist">Graphic Artist</option>
						<option value="production">Production</option>
					</select>
					<table
						class="sales-selected"
						v-if="salesSection == 'customer service'"
					>
						<thead>
							<tr>
								<th>Revenue</th>
								<th>Visitors</th>
								<th>Conversion Rate</th>
								<th>Revenue per Buyer</th>
								<th>Average Order Value</th>
								<th>Basket Size</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rafael Cruz</td>
								<td>Graphic Artist</td>
								<td>PHP 1,000.00</td>
								<td>50</td>
								<td>1 Hour</td>
								<td>Always Complete</td>
							</tr>
						</tbody>
					</table>
					<table class="sales-selected" v-if="salesSection == 'graphic artist'">
						<thead>
							<tr>
								<th>Revenue</th>
								<th>Visitors</th>
								<th>Conversion Rate</th>
								<th>Revenue per Buyer</th>
								<th>Average Order Value</th>
								<th>Basket Size</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rafael Cruz</td>
								<td>Graphic Artist</td>
								<td>PHP 1,000.00</td>
								<td>50</td>
								<td>1 Hour</td>
								<td>Always Complete</td>
							</tr>
						</tbody>
					</table>
					<table class="sales-selected" v-if="salesSection == 'production'">
						<thead>
							<tr>
								<th>Revenue</th>
								<th>Visitors</th>
								<th>Conversion Rate</th>
								<th>Revenue per Buyer</th>
								<th>Average Order Value</th>
								<th>Basket Size</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rafael Cruz</td>
								<td>Graphic Artist</td>
								<td>PHP 1,000.00</td>
								<td>50</td>
								<td>1 Hour</td>
								<td>Always Complete</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="admin-home-best home-portion">
				<h1 class="fs-1300">Best Sellers</h1>
				<div class="best-container container-portion">
					<table>
						<thead>
							<tr>
								<th>Supplies</th>
								<th>Services</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
							</tr>
							<tr>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
								<td>PRODUCT HERE</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="admin-top-customers home-portion">
				<h1 class="fs-1300">Top Customers</h1>
				<div class="customers-container container-portion">
					<!-- <div>
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
					</div> -->
					<table>
						<thead>
							<tr>
								<th>Names</th>
								<th>Revenue</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Isabel Ip</td>
								<td>1,000,000.00</td>
							</tr>
							<tr>
								<td>Boyfriend of Isabel</td>
								<td>500,000.00</td>
							</tr>
							<tr>
								<td>Dog of Isabel</td>
								<td>250,000.00</td>
							</tr>
							<tr>
								<td>Rolo Pena</td>
								<td>100,000.00</td>
							</tr>

							<tr>
								<td>Rafael Cruz</td>
								<td>50,000.00</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="admin-customer-journey home-portion">
				<h1 class="fs-1300">Customer Journey</h1>
				<div class="journey-container container-portion">
					<!-- <div>
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
					</div> -->
					<table>
						<thead>
							<tr>
								<th>Visits</th>
								<th>Add to Cart</th>
								<th>Proceed with Order</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="real-time-revenue home-portion">
				<h1 class="fs-1300">Real Time Performance</h1>
				<div class="performance-container container-portion">
					<!-- <div>
						<h3>Revenue</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Visitors</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Buyers</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Orders</h3>
						<p>NUMBER HERE</p>
					</div>
					<div>
						<h3>Units Sold</h3>
						<p>NUMBER HERE</p>
					</div> -->
					<table>
						<thead>
							<tr>
								<th>Revenue</th>
								<th>Visitors</th>
								<th>Buyers</th>
								<th>Orders</th>
								<th>Units Sold</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
								<td>NUMBER HERE</td>
							</tr>
						</tbody>
					</table>
				</div>
				<div class="second-performance-container container-portion">
					<div class="active-data">
						<select>
							<option value="yesterday">Yesterday</option>
						</select>
						<button>Download</button>
					</div>
					<table>
						<thead>
							<tr>
								<th>Revenue</th>
								<th>Visitors</th>
								<th>Conversion Rate</th>
								<th>Revenue per Buyer</th>
								<th>Average Order Value</th>
								<th>Basket Size</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rafael Cruz</td>
								<td>Graphic Artist</td>
								<td>PHP 1,000.00</td>
								<td>50</td>
								<td>1 Hour</td>
								<td>Always Complete</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="traffic home-portion">
				<h1 class="fs-1300">Traffic Per Page</h1>
				<div class="container-portion">
					<table>
						<thead>
							<tr>
								<th></th>
								<th>Homepage</th>
								<th>Products</th>
								<th>Our Work</th>
								<th>Email Us</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<th>Visitors</th>
								<td>###</td>
								<td>###</td>
								<td>###</td>
								<td>###</td>
							</tr>
							<tr>
								<th>Proportions</th>
								<td>###</td>
								<td>###</td>
								<td>###</td>
								<td>###</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="staff-performance home-portion">
				<h1 class="fs-1300">Staff Performance</h1>
				<div class="container-portion">
					<table>
						<thead>
							<tr>
								<th>Name</th>
								<th>Department</th>
								<th>Revenue</th>
								<th>Orders</th>
								<th>AVE Job Duration</th>
								<th>Fulfillment Rate</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rafael Cruz</td>
								<td>Graphic Artist</td>
								<td>PHP 1,000.00</td>
								<td>50</td>
								<td>1 Hour</td>
								<td>Always Complete</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="customer-performance home-portion">
				<h1 class="fs-1300">Customer Overview</h1>
				<div class="active-data">
					<p>Account Creation: <bold>#</bold></p>
					<p>New Account Creation: <bold>#</bold></p>
				</div>
				<div class="container-portion">
					<table>
						<thead>
							<tr>
								<th>Customer</th>
								<th>Revenue</th>
								<th># Of Orders</th>
								<th>Loyalty Points</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Rolo Pena</td>
								<td>PHP 1,000,000.00</td>
								<td>100</td>
								<td>50000</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div class="product-dashboard home-portion">
				<h1 class="fs-1300">Product Dashboard</h1>
				<div class="active-data">
					<p>Active SKUs: <bold>#</bold></p>
					<p>Purchasable SKUs: <bold>#</bold></p>
				</div>
				<div class="container-portion">
					<table>
						<thead>
							<tr>
								<th>Product Name</th>
								<th>Revenue</th>
								<th>Units Sold</th>
								<th>Visitors</th>
								<th>Add to Cart</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>Calling Card</td>
								<td>PHP 1,000,000.00</td>
								<td>100</td>
								<td>50000</td>
								<td>50000</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
import AveProcessing from "../../popups/AveProcessing.vue";
export default {
	name: "AdminHome",
	components: {
		AveProcessing,
	},
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
