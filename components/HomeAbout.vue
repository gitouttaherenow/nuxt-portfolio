<template>
    <section class="about" id="about">
		<div class="container">
			<h3 class="section-heading">About</h3>
			<div class="grid">
				<div class="col-lg-6 col-md-6 col-sm-12">
					<div class="about-photo">
						<img src="~/static/person.jpg" alt="">
					</div>
				</div>
				<div class="col-lg-6 col-md-6 col-sm-12 about-text">
					<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Tempora accusantium laudantium debitis nobis officiis sit, est nulla modi consequuntur assumenda dolore error voluptatibus? Eos, illo ipsam iste sint. Ipsa, libero.</p>
					<p>Corporis eos veritatis sint possimus fugiat!</p>
				</div>
			</div>
		</div>
	</section>
</template>

<script>
export default {
    name: 'HomeAbout'
}
</script>

<style lang="stylus" scoped>
.flex-wrap {
	display: flex;
	justify-content: space-between;
}

.about-photo {
	max-width: 475px;
}

.about-text {
	display: inline-flex;
	flex-direction: column;
	justify-content: center;
}
</style>