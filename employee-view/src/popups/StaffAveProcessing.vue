<template>
	<div class="staff-ave-wrapper">
		<table>
			<thead>
				<tr>
					<th>Total # of Orders</th>
					<th>Total # of Pending Orders</th>
					<th>Average Job Duration</th>
					<th>Fulfillment Rate</th>
				</tr>
			</thead>
			<tbody>
				<tr>
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
	name: "StaffAveProcessing",
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.staff-ave-wrapper {
	table {
		min-width: 25%;
		max-width: 50%;
		margin-right: 0px;
		margin-right: auto;
		white-space: nowrap;
		border-collapse: collapse;
	}
}
</style>
