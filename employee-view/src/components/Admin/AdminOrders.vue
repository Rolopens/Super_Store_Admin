<template>
	<div class="margin-block-start page-margin-inline">
		<div class="admin-order-wrapper">
			<div class="header-text">
				<h1>Orders</h1>
			</div>

			<div class="orders-wrapper">
				<h2>Supplies</h2>
				<table>
					<thead>
						<tr>
							<th>Order #</th>
							<th>Title</th>
							<th>Price</th>
							<th>Representative</th>
							<th>Address</th>
							<th>Status</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>Calling Card</td>
							<td>PHP 120</td>
							<td>Mikazuki Augus</td>
							<td>26 Highland Drive Blue Ridge A</td>
							<td>Confirming</td>
						</tr>
						<tr>
							<td>2</td>
							<td>Printing Thesis</td>
							<td>PHP 600</td>
							<td>Kudelia Bernstein</td>
							<td>26 Highland Drive Blue Ridge A</td>
							<td>Producing</td>
						</tr>
					</tbody>
				</table>
			</div>

			<div class="orders-wrapper margin-top">
				<h2>Services</h2>
				<table>
					<thead>
						<tr>
							<th>Order #</th>
							<th>Title</th>
							<th>Price</th>
							<th>Representative</th>
							<th>Address</th>
							<th>Status</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>Calling Card</td>
							<td>PHP 120</td>
							<td>Mikazuki Augus</td>
							<td>26 Highland Drive Blue Ridge A</td>
							<td>Confirming</td>
						</tr>
						<tr>
							<td>2</td>
							<td>Printing Thesis</td>
							<td>PHP 600</td>
							<td>Kudelia Bernstein</td>
							<td>26 Highland Drive Blue Ridge A</td>
							<td>Producing</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "AdminOrders",
};
</script>

<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Admin/admin-orders.scss";
</style>
