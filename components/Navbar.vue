<template>
  <nav id="navigation" class="main-menu">
		<div class="main-menu">
			<nuxt-link to="/">Home</nuxt-link>
			<a href="#about">About</a>
			<!-- <a href="#work">Work</a> -->
			<nuxt-link to="/work">Work</nuxt-link>
			<a href="#contact">Contact</a>
		</div>
	</nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style lang="stylus">
.main-menu {
	display: flex;
    justify-content: center;
    align-items: center;
    width: 100%;
    height: 80px;
    position: absolute;
    background-color: transparent;
    z-index: 99;
}

.main-menu a {
	margin: 0 30px;
	color: #fff;
	text-transform: lowercase;
	font-weight: 600;
}
</style>