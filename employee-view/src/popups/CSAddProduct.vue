<template>
	<div class="cs-add-popup">
		<div class="cs-add-inner">
			<div class="cs-add-header">
				<h2>Add Product</h2>
				<button @click="() => ToggleAddProduct('addButtonTrigger')">
					<i class="fa-solid fa-xmark"></i>
				</button>
			</div>
			<div class="cs-add-details">
				<section>
					<label for="service">Service</label>
					<input type="text" name="service" />
				</section>
				<section>
					<h3>Specifications</h3>
					<label for="size">Size:</label>
					<input type="text" name="size" />
					<label for="qty">QTY:</label>
					<input type="number" name="qty" />
					<label for="color">Color:</label>
					<input type="text" name="color" />
					<label for="add-services">Additional Services:</label>
					<input type="text" name="add-services" />
				</section>
				<section>
					<label for="other-instructions">Other Instructions</label>
					<input type="text" name="other-instructions" />
				</section>
				<section>
					<label for="image">Select Image File</label>
					<input type="file" name="file" />
				</section>
				<section>
					<label for="status">Status</label>
					<input type="text" name="status" />
				</section>
				<section>
					<label for="status">Status</label>
					<input type="text" name="status" />
				</section>
				<section>
					<label for="graphic-artist">Graphic Artist</label>
					<input type="text" name="graphic-artist" />
				</section>
				<section>
					<label for="production">Production</label>
					<input type="text" name="production" />
				</section>
			</div>
			<div class="cs-add-save">
				<button @click="() => ToggleAddProduct('addButtonTrigger')">
					Save <i class="fa-solid fa-floppy-disk"></i>
				</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "CSAddProduct",
	props: ["ToggleAddProduct"],
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.cs-add-popup {
	position: fixed;
	top: 0;
	left: 0;
	right: 0;
	bottom: 0;
	z-index: 99;
	background-color: rgba(0, 0, 0, 0.2);
	display: flex;
	align-items: center;
	justify-content: center;
	overflow-y: scroll;

	@media (max-width: 1550px) {
		.cs-add-inner {
			width: 70vw !important;
			height: fit-content !important;
		}
	}

	@media (max-width: 650px) {
		.cs-add-inner {
			width: 100vw !important;
		}
	}

	.cs-add-inner {
		background: #fff;
		width: 30vw;
		height: fit-content;
		padding: $size-600;
	}

	.cs-add-header {
		display: flex;
		justify-content: space-between;
		align-content: center;
		margin-bottom: 1rem;

		h2 {
			font-size: $fs-900;
		}

		button {
			background-color: transparent;
			border: none;
			font-size: 1.5rem;
		}
	}

	.cs-add-details {
		h3 {
			font-size: 20px;
		}
		section {
			margin-bottom: 0.8rem;
			label {
				display: block;
				font-weight: bold;
			}

			input {
				padding-left: 1rem;
				width: 100%;
				border-radius: 14px;
			}
		}
	}

	.cs-add-save {
		display: flex;
		justify-content: flex-end;
		button {
			// border: none;
			background-color: #67cf61 !important;
			color: white;
			padding: 0.5rem 1.2rem;
			border-radius: 14px;
		}
	}
}
</style>
