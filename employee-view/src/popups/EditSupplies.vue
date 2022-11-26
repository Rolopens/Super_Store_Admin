<template>
	<div class="add-supply-popup">
		<div class="add-popup-inner">
			<div class="add-popup-header">
				<h2>Edit Product</h2>
				<button @click="() => ToggleSupplyEdit('buttonTrigger')">
					<i class="fa-solid fa-xmark"></i>
				</button>
			</div>
			<div class="add-popup-details">
				<div class="add-popup-image">
					<img src="https://picsum.photos/200/300" />
					<input type="file" name="file" />
				</div>
				<div class="add-popup-fields">
					<section>
						<label for="name">Product Name</label>
						<input type="text" value="Product Name" id="name" />
					</section>
					<section>
						<label for="price">Price</label>
						<input type="number" value="5000" id="price" />
					</section>
					<section>
						<label for="supply">Supply</label>
						<input type="number" value="20" id="supply" />
					</section>
				</div>
			</div>
			<div class="add-popup-description">
				<label for="description">Product Description</label>
				<input type="number" id="description" />
			</div>
			<div class="add-popup-calculator">
				<label for="calculator">Calculate Formula</label>
				<input type="number" id="calculator" />
			</div>
			<div class="add-popup-save">
				<button @click="() => ToggleSupplyEdit('buttonTrigger')">
					Save <i class="fa-solid fa-floppy-disk"></i>
				</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "EditPopup",
	props: ["ToggleSupplyEdit"],
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.add-supply-popup {
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
		.add-popup-inner {
			width: 70vw !important;
			height: fit-content !important;
		}
	}

	@media (max-width: 650px) {
		.add-popup-inner {
			width: 100vw !important;
		}
	}

	.add-popup-inner {
		background: #fff;
		width: 30vw;
		height: 60vh;
		padding: $size-600;

		.add-popup-header {
			display: flex;
			justify-content: space-between;
			align-content: center;

			h2 {
				font-size: $fs-900;
			}

			button {
				background-color: transparent;
				border: none;
				font-size: 1.5rem;
			}
		}

		@media (max-width: 450px) {
			.add-popup-details {
				display: flex !important;
				flex-direction: column !important;
				height: fit-content;
			}
		}

		.add-popup-details {
			margin-top: 1rem;
			display: grid;
			grid-template-columns: 1.2fr 2fr;
			align-content: center;
			// gap: 1rem;

			.add-popup-image {
				width: 200px;
				display: flex;
				flex-direction: column;
				gap: 10px;

				img {
					height: 220px;
					width: fit-content;
				}
			}

			.add-popup-fields {
				display: flex;
				flex-direction: column;
				justify-content: space-between;

				section {
					label {
						display: block;
						font-size: $fs-1000;
					}
					input {
						width: 100%;
						padding-inline: 1rem;
						border-radius: 14px;
					}
				}
			}
		}

		.add-popup-description,
		.add-popup-calculator {
			margin-top: 1.5rem;
			label {
				display: block;
				font-size: $fs-1000;
			}
			input {
				width: 100%;
				padding-inline: 1rem;
				border-radius: 14px;
			}
		}

		.add-popup-save {
			margin-top: 2rem;
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
}
</style>
