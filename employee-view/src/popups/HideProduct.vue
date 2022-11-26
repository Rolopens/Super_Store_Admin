<template>
	<div class="hide-popup">
		<div class="hide-inner">
			<p>
				Are you sure you want to <br />
				confirm that action?
			</p>
			<div class="hide-buttons">
				<button
					aria-label="cancel"
					@click="() => ToggleHideProduct('hideButtonTrigger')"
				>
					No
				</button>

				<button @click="() => ToggleHideProduct('hideButtonTrigger')">
					Yes
				</button>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "HideProduct",
	props: ["ToggleHideProduct"],
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";

.hide-popup {
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

	.hide-inner {
		background: #fff;
		width: 200px;
		height: 20vh;
		border-radius: 14px;
		padding: $size-600;

		p {
			// margin-top: 1rem;
			text-align: center;
		}

		.hide-buttons {
			display: flex;
			justify-content: space-between;
			margin-top: 2rem;

			button {
				&[aria-label="cancel"] {
					color: red;
				}

				color: green;
			}
		}
	}
}
</style>
