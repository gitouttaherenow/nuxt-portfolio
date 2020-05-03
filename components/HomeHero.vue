<template>
  <section class="hero">
    <div class="container">
      <div class="intro">
        <h1>I'm Thoshikesh</h1>
        <p>An UI/UX designer from Bengaluru with focus on well converting designs.</p>
      </div>
      <a class="scroll-down" href="#work">See My Work</a>
    </div>
  </section>
</template>

<script>
export default {
  name: "HomeHero"
};
</script>

<style lang="stylus" scoped>
.hero
	display: flex
	min-height: 100vh
	align-items: center
	justify-content: center
	flex-direction: column
	text-align: center
	padding-top: 0
	background-color: #fff9c4
	background-image: url('~assets/home-hero.jpg')
	background-size cover
	color #fff


.intro
	margin 150px 0

.intro h1
	font-size 4rem;

.intro p
	font-size 1.6rem

.scroll-down
	color #ffffff
	font-weight 600

section:last-of-type
	padding-bottom 120px

</style>
