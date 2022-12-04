<template>
	<div class="cs-ave-wrapper">
		<table>
			<thead>
				<tr>
					<th>Total # of Revenue for the Month</th>
					<th>Total # of Accepted Orders</th>
					<th>Pending Orders w/ Artist</th>
					<th>Pending Orders w/ Production</th>
					<th>Fulfillment Rate</th>
					<th>AVE Processing Time</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>###</td>
					<td>###</td>
					<td>###</td>
					<td>###</td>
					<td>###</td>
					<td>###</td>
				</tr>
			</tbody>
		</table>
	</div>
</template>

<script>
export default {
	name: "CSOrderAveProcessing",
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.cs-ave-wrapper {
	overflow-x: auto;
	table {
		min-width: 25%;
		// max-width: 50%;
		margin-right: 0px;
		margin-right: auto;
		white-space: nowrap;
		border-collapse: collapse;
	}
}
</style>
