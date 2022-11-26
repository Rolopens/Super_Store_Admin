<template>
	<div class="add-product-popup">
		<div class="add-product-inner">
			<div class="add-product-header">
				<h2>Add Product</h2>
				<button @click="() => ToggleAddProduct('addButtonTrigger')">
					<i class="fa-solid fa-xmark"></i>
				</button>
			</div>
			<div class="add-product-details">
				<section>
					<label for="image">Select Image File</label>
					<input type="file" name="file" />
				</section>
				<section>
					<label for="name">Product Name</label>
					<input type="text" name="name" />
				</section>
				<section>
					<label for="price">Price</label>
					<input type="text" name="price" />
				</section>
				<section>
					<label for="supply">Supply</label>
					<input type="text" name="supply" />
				</section>
				<section>
					<label for="description">Product Description</label>
					<input type="text" name="description" />
				</section>
				<section>
					<label for="calculator">Calculate Formula</label>
					<input type="text" name="formula" />
				</section>
			</div>
			<div class="add-popup-save">
				<button @click="() => ToggleAddProduct('addButtonTrigger')">
					Save <i class="fa-solid fa-floppy-disk"></i>
				</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "AddProduct",
	props: ["ToggleAddProduct"],
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.add-product-popup {
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
		.add-product-inner {
			width: 70vw !important;
			height: fit-content !important;
		}
	}

	@media (max-width: 650px) {
		.add-product-inner {
			width: 100vw !important;
		}
	}

	.add-product-inner {
		background: #fff;
		width: 30vw;
		height: fit-content;
		padding: $size-600;
	}

	.add-product-header {
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

	.add-product-details {
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

	.add-popup-save {
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
