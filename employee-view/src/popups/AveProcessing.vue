<template>
	<div class="ave-processing-wrapper">
		<table>
			<thead>
				<tr>
					<th>Cancellation Rate</th>
					<th>AVE Processing Time</th>
				</tr>
			</thead>
			<tbody>
				<tr>
					<td>10 Orders</td>
					<td>15:01 Minutes</td>
				</tr>
			</tbody>
		</table>
	</div>
</template>

<script>
export default {
	name: "AveProcessing",
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.ave-processing-wrapper {
	table {
		min-width: 25%;
		max-width: 50%;
		margin-right: 0px;
		margin-left: auto;
		white-space: nowrap;
		border-collapse: collapse;
	}
}
</style>
