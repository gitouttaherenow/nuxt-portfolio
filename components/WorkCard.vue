<template>
  <!-- <div class="work-card" v-bind:style="{ backgroundImage: `url(${bgImg})` }"> -->
  <div class="col-lg-6 col-md-6 col-sm-12">
    <div class="work-card">
      <div class="work-card-thumb">
        <a href="#">
          <img :src="workImageURL" alt="" class="work-img" />
        </a>
      </div>
      <div class="work-card-link">
        <!-- We use v-html to bind title so it renders as HTML and not print unitext code -->
        <div class="work-card-info">
          <h3  v-html="title">{{ title }}</h3>
          <div class="work-category">
            <h4>Cateogries:</h4>
            <ul>
              <li>UI/UX</li>
              <li>Front-End</li>
            </ul>
            <a :href="workImageURL" class="btn"><span>View →</span></a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "WorkCard",
  props: ["title", "workImageURL"]
};
</script>

<style lang="stylus" scoped>

.work-card
  position relative
  color #fff
  margin-bottom 1rem

.work-card ul
  padding 0

.work-card li
  list-style-type none

.work-card-thumb
  position relative
  object-fit cover

.work-card-link
  position absolute
  display grid
  justify-content center
  align-items center
  text-align center
  background-color rgba(0,0,0,0.8)
  height 100%
  width 100%
  top 0
  opacity: 0
  transition: all .2s ease

.work-card-link:hover
  opacity 1

.project-info
	color: #ffffff

.project-info h3
	font-size: 2rem;
	margin-top: 0;

.btn
	display: inline-block;
	position: relative;
	z-index: 1;
	padding: 15px 35px;
	margin-top: 15px;
	font-weight: 600;
	color: #ffffff;
	text-decoration: none;
	border: 1px solid #ffffff;

.btn:hover
	color: #000;

.btn:after
	display: block;
	content: "";
	height: 100%;
	width: 0;
	position: absolute;
	top: 0;
	left: 0;
	background-color: #ffffff;
	z-index: -1;
	transition: 0.2s all ease;

.btn:hover:after
	width: 100%;
	transition: 0.2s all ease;
</style>
