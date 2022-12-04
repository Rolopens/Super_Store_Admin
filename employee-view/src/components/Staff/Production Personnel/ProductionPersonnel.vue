<template>
	<div class="margin-block-start page-margin-inline">
		<div class="production-personnel-wrapper">
			<StaffAveProcessing />
			<div class="header-text">
				<h1>Production Personnel</h1>
			</div>
			<div class="production-table">
				<table>
					<thead>
						<tr>
							<th>Date</th>
							<th>Order #</th>
							<th>Service</th>
							<th>Specifications</th>
							<th>Other Instructions</th>
							<th>File</th>
							<th>Status</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>1</td>
							<td>3.5 x 2</td>
							<td>Black and White</td>
							<td>Matte</td>
							<td>Instructions Here</td>
							<td>
								<input type="file" />
								<button>Save <i class="fa-solid fa-floppy-disk"></i></button>
							</td>
							<td>
								<a
									download="Sample"
									href="https://picsum.photos/200/300"
									target="_blank"
								>
									<img src="https://picsum.photos/200/300" alt="" />
								</a>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</template>

<script>
import StaffAveProcessing from "../../../popups/StaffAveProcessing.vue";
export default {
	name: "ProductionProcessing",
	components: {
		StaffAveProcessing,
	},
};
</script>

<style lang="scss">
@import "../../../styles/global-variables.scss";
@import "../../../styles/Staff/Production Personnel/production-view.scss";
</style>
