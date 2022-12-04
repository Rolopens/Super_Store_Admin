<template>
	<div class="margin-block-start page-margin-inline">
		<div class="cs-orders-wrapper">
			<CSAveProcessing />
			<div class="header-text">
				<h1>Customer Service Orders</h1>
				<button @click="() => ToggleAddProduct('addButtonTrigger')">
					Add <i class="fa-solid fa-plus"></i>
				</button>
			</div>
			<div class="umbrella-sections">
				<input
					type="radio"
					name="umbrella-options"
					id="customer-approval"
					value="customer-approval"
					v-model="umbrellaTerms"
				/>
				<label for="customer-approval">Customer Approval</label>
				<input
					type="radio"
					name="umbrella-options"
					id="endorsement-artist"
					v-model="umbrellaTerms"
					value="endorsement-artist"
				/>
				<label for="endorsement-artist">Endorsement to Artist</label>
				<input
					type="radio"
					name="umbrella-options"
					id="endorsement-production"
					v-model="umbrellaTerms"
					value="endorsement-production"
				/>
				<label for="endorsement-production">Endorsement to Production</label>
				<input
					type="radio"
					name="umbrella-options"
					id="pick-up"
					v-model="umbrellaTerms"
					value="pick-up"
				/>
				<label for="pick-up">Pick-Up</label>
			</div>
			<AddProduct
				v-if="addTrigger.addButtonTrigger"
				:ToggleAddProduct="() => ToggleAddProduct('addButtonTrigger')"
			/>
			<div class="cs-order-table">
				<table v-if="umbrellaTerms == 'customer-approval'">
					<thead>
						<tr>
							<th>Date</th>
							<th>Order #</th>
							<th>Customer Details</th>
							<th>Specifications</th>
							<th>Other Instructions</th>
							<th>Total Amount</th>
							<th>File</th>
							<th>Status</th>
							<th>Graphic Design</th>
							<th>Production</th>
							<th>Actions</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>10/11/2022</td>
							<td>###</td>
							<td>
								<ul>
									<li>Name: ###</li>
									<li>Contact #: ###</li>
									<li>Email###</li>
									<li>Address: ###</li>
								</ul>
							</td>
							<td>###</td>
							<td>
								<ul>
									<li>Size: ###</li>
									<li>Qty: ###</li>
									<li>Color: ###</li>
									<li>Additional: ###</li>
								</ul>
							</td>
							<td>###</td>
							<td>
								<a
									download="Sample"
									href="https://picsum.photos/200/300"
									target="_blank"
								>
									<img src="https://picsum.photos/200/300" alt="" />
								</a>
							</td>
							<td>
								<select>
									<option>Confirmation</option>
									<option>Quotation</option>
									<option>Approval</option>
									<option>Pending</option>
									<option>Endorsed to Artist</option>
									<option>Customer Approval</option>
									<option>Endorsed to Production</option>
									<option>Ready</option>
								</select>
							</td>
							<td>
								<select>
									<option>NAME HERE</option>
								</select>
							</td>
							<td>
								<select>
									<option>NAME HERE</option>
								</select>
							</td>
							<td>
								<select>
									<option>ACTION HERE</option>
								</select>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
	</div>
</template>

<script>
import CSAveProcessing from "../../../popups/CSAveProcessing.vue";
import AddProduct from "../../../popups/CSAddProduct.vue";
import { ref } from "vue";
export default {
	name: "CSOrders",
	components: {
		CSAveProcessing,
		AddProduct,
	},
	data() {
		return {
			umbrellaTerms: "customer-approval",
		};
	},
	setup() {
		const addTrigger = ref({
			addButtonTrigger: false,
		});

		const ToggleAddProduct = (trigger) => {
			addTrigger.value[trigger] = !addTrigger.value[trigger];
		};

		return {
			addTrigger,
			ToggleAddProduct,
		};
	},
};
</script>

<style lang="scss">
@import "../../../styles/global-variables.scss";
@import "../../../styles/Staff/Customer Service/CSOrders.scss";
</style>
