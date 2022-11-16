<template>
	<div class="primary-footer-navigation">
		<div class="primary-footer-wrapper">
			<div class="company-description text-color-white">
				<div>
					<img src="../assets/whitelogo.svg" alt="Super Store Logo" />
					<p>
						Office, School Supplies, Superstore, Inc. is your friendly
						neighborhood store that aims to meet your every need. We keep
						Honesty, Respect, and Trust at our core to ensure you experience our
						Super customer service and quality results every time you work with
						us.
					</p>
				</div>
				<div class="footer-options">
					<a href="#">
						<p>PRODUCTS</p>
					</a>
					<a href="#">
						<p>OUR WORKS</p>
					</a>
					<a href="#">
						<p>EMAIL US</p>
					</a>
				</div>
				<div class="social-list">
					<span class="text-bold">Socials</span>
					<ul>
						<li>
							<a aria-label="Facebook" href="#"
								><img src="../assets/Facebook.svg" alt="Facebook Icon"
							/></a>
						</li>
						<li>
							<a aria-label="Instagram" href="#"
								><img src="../assets/Instagram.svg" alt="Instagram Icon"
							/></a>
						</li>
						<li>
							<a aria-label="Viber" href="#"
								><img src="../assets/Viber.svg" alt="Viber Icon"
							/></a>
						</li>
					</ul>
				</div>
			</div>
			<div class="company-details text-color-white">
				<section>
					<h2 class="fw-bold">CONTACT US</h2>
					<p>Email: sales@superstoreph.com</p>
					<p>Landline: (+632) 8772 0012</p>
					<p>Viber: (+63) 915 498 4690</p>
				</section>
				<section>
					<h2 class="fw-bold">VISIT US</h2>
					<p>
						Superstore Bldg. 29 President's Avenue, Tahanan Village, BF Homes,
						Parañaque City, 1720
					</p>
				</section>
				<section>
					<h2 class="fw-bold">OFFICE HOURS</h2>
					<p>Mondays - Saturdays</p>
					<p>9AM - 6PM</p>
				</section>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: "FooterNav",
};
</script>

<style lang="scss">
@import "../styles/global-variables.scss";
@import "../styles/footer.scss";
</style>
