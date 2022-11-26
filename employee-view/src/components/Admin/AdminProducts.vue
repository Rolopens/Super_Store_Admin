<template>
	<div class="margin-block-start page-margin-inline">
		<div class="admin-products-wrapper">
			<div class="header-text">
				<h1>Products</h1>
			</div>
			<select v-model="productSelected">
				<option value="supplies">Supplies</option>
				<option value="services">Services</option>
			</select>
			<div
				v-if="productSelected == 'supplies'"
				class="services-container products-container"
			>
				<div class="product-header">
					<div class="supplies-add">
						<button @click="() => ToggleAddProduct('addButtonTrigger')">
							Add <i class="fa-solid fa-plus"></i>
						</button>
					</div>
					<AddProduct
						v-if="addTrigger.addButtonTrigger"
						:ToggleAddProduct="() => ToggleAddProduct('addButtonTrigger')"
					/>
					<div class="search-box">
						<input type="text" />
						<button><i class="fa-solid fa-magnifying-glass"></i></button>
					</div>
				</div>
				<div class="admin-products-table">
					<table>
						<thead>
							<tr>
								<th>Image</th>
								<th>Name</th>
								<th>Price</th>
								<th>Supply</th>
								<th>Description</th>
							</tr>
						</thead>
						<tbody>
							<tr>
								<td><img src="https://picsum.photos/200/300" /></td>
								<td>Gundam</td>
								<td>2000</td>
								<td>10</td>
								<td>Description here</td>
								<td>
									<button
										aria-label="edit"
										@click="() => ToggleSupplyEdit('buttonTrigger')"
									>
										Edit <i class="fa-solid fa-pen-to-square"></i>
									</button>
								</td>
								<EditSupplies
									v-if="editTrigger.buttonTrigger"
									:ToggleSupplyEdit="() => ToggleSupplyEdit('buttonTrigger')"
								/>
								<td>
									<button @click="() => ToggleHideProduct('hideButtonTrigger')">
										Hide <i class="fa-solid fa-eye-slash"></i>
									</button>
								</td>
								<HideProduct
									v-if="hideTrigger.hideButtonTrigger"
									:ToggleHideProduct="
										() => ToggleHideProduct('hideButtonTrigger')
									"
								/>
								<td>
									<button aria-label="delete">
										Delete <i class="fa-solid fa-trash"></i>
									</button>
								</td>
							</tr>
						</tbody>
					</table>
				</div>
			</div>
			<div
				v-if="productSelected == 'services'"
				class="supplies-container products-container"
			></div>
		</div>
	</div>
</template>

<script>
import EditSupplies from "../../popups/EditSupplies.vue";
import HideProduct from "../../popups/HideProduct.vue";
import AddProduct from "../../popups/AddProduct.vue";
import { ref } from "vue";
export default {
	name: "AdminProducts",
	components: {
		EditSupplies,
		HideProduct,
		AddProduct,
	},
	data() {
		return {
			productSelected: "supplies",
		};
	},
	setup() {
		// Button Triggers
		const editTrigger = ref({
			buttonTrigger: false,
		});

		const hideTrigger = ref({
			hideButtonTrigger: false,
		});

		const deleteTrigger = ref({
			deleteButtonTrigger: false,
		});

		const addTrigger = ref({
			addButtonTrigger: false,
		});

		// Trigger Actions
		const ToggleSupplyEdit = (trigger) => {
			editTrigger.value[trigger] = !editTrigger.value[trigger];
		};

		const ToggleHideProduct = (trigger) => {
			hideTrigger.value[trigger] = !hideTrigger.value[trigger];
		};

		const ToggleDeleteProduct = (trigger) => {
			deleteTrigger.value[trigger] = !deleteTrigger.value[trigger];
		};

		const ToggleAddProduct = (trigger) => {
			addTrigger.value[trigger] = !addTrigger.value[trigger];
		};

		return {
			editTrigger,
			hideTrigger,
			deleteTrigger,
			addTrigger,
			ToggleSupplyEdit,
			ToggleHideProduct,
			ToggleDeleteProduct,
			ToggleAddProduct,
		};
	},
};
</script>

<style lang="scss">
@import "../../styles/global-variables.scss";
@import "../../styles/Admin/admin-products.scss";
</style>
