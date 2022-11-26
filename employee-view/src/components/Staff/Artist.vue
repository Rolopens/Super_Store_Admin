<template>
	<div class="margin-block-start page-margin-inline">
		<div class="artist-wrapper">
			<div class="header-text">
				<h1>Orders</h1>
			</div>
			<div class="artist-table">
				<table>
					<thead>
						<tr>
							<th>Order #</th>
							<th>Size</th>
							<th>Color</th>
							<th>Additional Services</th>
							<th>Notes</th>
							<th>Sample</th>
							<th>Upload</th>
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
								<a
									download="Sample"
									href="https://picsum.photos/200/300"
									target="_blank"
								>
									<img src="https://picsum.photos/200/300" alt="" />
								</a>
							</td>
							<!-- If statement. If there is a picture then it shows the preview, if not then the input option -->
							<td>
								<input type="file" />
								<button>Save <i class="fa-solid fa-floppy-disk"></i></button>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "ArtistView",
};
</script>

<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Staff/artist-view.scss";
</style>
