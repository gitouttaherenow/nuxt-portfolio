<template>
  <div id="app">
    <Navbar />
    <ProjectHero />
    <div class="container">
      <section class="project-images">
        <div class="grid">
          <div class="col-lg-12 col-md-12 col-sm-12">
            <img src="@/assets/stellify-gmbh.png" alt="" />
          </div>
          <div class="col-lg-6 col-md-6 col-sm-12">
            <img src="@/assets/blogger.jpg" alt="" />
          </div>
          <div class="col-lg-6 col-md-6 col-sm-12">
            <img src="@/assets/tumblr.jpg" alt="" />
          </div>
        </div>
      </section>
    </div>
    <nuxt />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar";
import ProjectHero from "@/components/ProjectHero";

export default {
  name: "app",
  components: {
    Navbar,
    ProjectHero
  }
};
</script>

<style lang="stylus" scoped>
.hero {
	display: flex;
	min-height: 100vh;
	align-items: center;
	justify-content: center;
	flex-direction: column;
	text-align: center;
	padding-top: 0;
	background-color: #fff9c4;
}

.intro {
	margin: 150px 0;
}

.intro h1 {
	font-size: 4rem;
}

.intro p {
	font-size: 1.6rem;
}

.scroll-down {
	font-weight: 600;
}

section:last-of-type {
	padding-bottom: 120px;
}
</style>
