<template>
    <section class="contact" id="contact">
		<div class="container">
			<div class="contact-intro">
				<h3 class="section-heading">Contact</h3>
				<p>I'm available for freelance work and remote jobs.</p>
				<a href="mailto:hello@website.com">Contact Me</a>
			</div>
			<div class="social-links">
				<!-- <a href="#" id="linkedin"><i class="fab fa-linkedin"></i> LinkedIn</a> -->
				<a href="#" id="behance"><i class="fab fa-behance"></i> Behance</a>
				<!-- <a href="#" id="dribbble"><i class="fab fa-dribbble"></i> Dribbble</a> -->
				<a href="#" id="instagram"><i class="fab fa-instagram"></i> Instagram</a>
				<a href="#" id="facebook"><i class="fab fa-facebook"></i> Facebook</a>
				<!-- <a href="#" id="twitter"><i class="fab fa-twitter"></i> Twitter</a> -->
			</div>
		</div>
	</section>
</template>

<script>
export default {
    name: 'contact'
}
</script>

<style lang="stylus" scoped>
.contact {
	text-align: center;
}

.social-links {
	display: flex;
	flex-wrap: wrap;
	justify-content: center;
	align-items: center;
	margin-top: 50px;
	border: 1px solid #EEEDEE;
	border-width: 1px 0 0 1px;
}

.social-links>a {
	flex-basis: 33%;
	flex-grow: 1;
	position: relative;
	font-size: 1.6rem;
	text-align: center;
	color: #262626;
	padding: 40px 0;
    border: 1px solid #EEEDEE;
    border-width: 0 1px 1px 0;
    z-index: 1;
}

.social-links>a:after {
	display: block;
	content: "";
	position: absolute;
	top: 0;
	left: 0;
	height: 100%;
	width: 0;
	z-index: -1;
	transition: 0.2 all ease;
}

.social-links>a:hover:after {
	width: 100%;
	transition: 0.2s all ease;
}

.social-links>a:hover {
	color: #fff;
	transition: 0.2s all ease;
}

.social-links>a:hover i {
	color: #fff;
	transition: 0.2s all ease;
}

#linkedin:after {background-color: #0077B5;}
#behance:after {background-color: #1769FF;}
#dribbble:after {background-color: #EA4C89;}
#instagram:after {background: #f09433; background: -moz-linear-gradient(45deg, #f09433 0%, #e6683c 25%, #dc2743 50%, #cc2366 75%, #bc1888 100%); background: -webkit-linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%); background: linear-gradient(45deg, #f09433 0%,#e6683c 25%,#dc2743 50%,#cc2366 75%,#bc1888 100%);}
#facebook:after {background-color: #3B5998;}
#twitter:after {background-color: #1DA1F2;}

.fa-linkedin {color: #0077B5;}
.fa-behance {color: #1769FF;}
.fa-dribbble {color: #EA4C89;}
.fa-instagram {color: #212745;}
.fa-facebook {color: #3B5998;}
.fa-twitter {color: #1DA1F2;}
</style>