<template>
	<div class="margin-block-start page-margin-inline">
		<div class="admin-sales-wrapper">
			<div class="header-text">
				<h1>Sales</h1>
			</div>
			<div class="time-period">
				<select>
					<option>Week No.</option>
				</select>
				<select>
					<option>2022 Date</option>
				</select>
			</div>
			<div class="sales-wrapper">
				<div class="yearly-summary sales-section">
					<section>
						<h2>Total Sales</h2>
						<p>PHP 1,000,000.00</p>
					</section>
					<section>
						<h2>Supplies Revenue</h2>
						<p>PHP 1,000,000.00</p>
					</section>
					<section>
						<h2>Services Revenue</h2>
						<p>PHP 1,000,000.00</p>
					</section>
				</div>
				<div class="customer-representative sales-section">
					<table>
						<thead>
							<tr>
								<th>Accepted By</th>
								<th>Total Amount</th>
								<th>Record Count</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
						</tbody>
					</table>
					<div class="pagination">
						<p>1/14</p>
						<button><i class="fa-solid fa-chevron-left"></i></button>
						<button><i class="fa-solid fa-chevron-right"></i></button>
					</div>
				</div>
				<div class="artist sales-section">
					<table>
						<thead>
							<tr>
								<th>Artist</th>
								<th>Total Amount</th>
								<th>Record Count</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
						</tbody>
					</table>
					<div class="pagination">
						<p>1/14</p>
						<button><i class="fa-solid fa-chevron-left"></i></button>
						<button><i class="fa-solid fa-chevron-right"></i></button>
					</div>
				</div>
				<div class="production sales-section">
					<table>
						<thead>
							<tr>
								<th>Production</th>
								<th>Total Amount</th>
								<th>Record Count</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
						</tbody>
					</table>
					<div class="pagination">
						<p>1/14</p>
						<button><i class="fa-solid fa-chevron-left"></i></button>
						<button><i class="fa-solid fa-chevron-right"></i></button>
					</div>
				</div>
				<div class="yearly-sales sales-section">
					<table>
						<thead>
							<tr>
								<th>Month</th>
								<th>2021 Sales</th>
								<th>2022 Conso Sales</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
							<tr>
								<td>April</td>
								<td>PHP 1000</td>
								<td>500</td>
							</tr>
						</tbody>
					</table>
					<div class="pagination">
						<p>1/14</p>
						<button><i class="fa-solid fa-chevron-left"></i></button>
						<button><i class="fa-solid fa-chevron-right"></i></button>
					</div>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "AdminSales",
};
</script>

<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Admin/admin-sales.scss";
</style>
