<template>
  <div id="work">
    <section class="project-wrap project-1">
      <div class="container">
        <div class="grid">
          <div class="col-lg-5 col-md-6 col-sm-12">
            <div class="project-info">
              <h3>Aditya Automotive Systems</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Sapiente nostrum magni qui aliquam. Ipsum facilis, molestias
                reiciendis quod reprehenderit quaerat modi cupiditate.
              </p>
              <p>My role was UI / UX</p>
              <a href="#" class="btn"><span>See Project →</span></a>
            </div>
          </div>
          <div class="col-lg-7 col-md-6 col-sm-12">
            <img
              class="animated fadeIn"
              src="~/static/aditya-auto.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section class="project-wrap project-2">
      <div class="container">
        <div class="grid">
          <div class="col-lg-5 col-md-6 col-sm-12">
            <div class="project-info">
              <h3>Stellify GmbH</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Sapiente nostrum magni qui aliquam. Ipsum facilis, molestias
                reiciendis quod reprehenderit quaerat modi cupiditate.
              </p>
              <p>My role was UI / UX</p>
              <a href="#" class="btn"><span>See Project →</span></a>
            </div>
          </div>
          <div class="col-lg-7 col-md-6 col-sm-12">
            <img
              class="animated fadeIn"
              src="~/static/stellify-gmbh.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section class="project-wrap project-3">
      <div class="container">
        <div class="grid">
          <div class="col-lg-5 col-md-6 col-sm-12">
            <div class="project-info">
              <h3>Feast - Rachel Cole</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Sapiente nostrum magni qui aliquam. Ipsum facilis, molestias
                reiciendis quod reprehenderit quaerat modi cupiditate.
              </p>
              <p>My role was UI / UX</p>
              <a href="#" class="btn"><span>See Project →</span></a>
            </div>
          </div>
          <div class="col-lg-7 col-md-6 col-sm-12">
            <img
              class="animated fadeIn"
              src="~/static/rachel-cole.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </section>

    <section class="project-wrap project-4">
      <div class="container">
        <div class="grid">
          <div class="col-lg-5 col-md-6 col-sm-12">
            <div class="project-info">
              <h3>Yola</h3>
              <p>
                Lorem ipsum dolor sit amet, consectetur adipisicing elit.
                Sapiente nostrum magni qui aliquam. Ipsum facilis, molestias
                reiciendis quod reprehenderit quaerat modi cupiditate.
              </p>
              <p>My role was UI / UX</p>
              <a href="#" class="btn"><span>See Project →</span></a>
            </div>
          </div>
          <div class="col-lg-7 col-md-6 col-sm-12">
            <img class="animated fadeIn" src="~/static/yola.jpg" alt="" />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: "HomeProjects"
};
</script>

<style lang="stylus" scoped>
.project-1 {
    background-color: #932c25;
}

.project-2 {
	background-color: #317d58;
}

.project-3 {
	background-color: #242633;
}

.project-4 {
	background-color: #2f4c6f;
}

.project-info {
	color: #ffffff;
}

.project-wrap img {
	-webkit-box-shadow: 0px 0px 70px 5px rgba(0,0,0,0.55);
	-moz-box-shadow: 0px 0px 70px 5px rgba(0,0,0,0.55);
	box-shadow: 0px 0px 70px 5px rgba(0,0,0,0.55);
}

.project-info h3 {
	font-size: 2rem;
	margin-top: 0;
}


.btn {
	display: inline-block;
	position: relative;
	z-index: 1;
	padding: 15px 35px;
	margin-top: 15px;
	font-weight: 600;
	color: #ffffff;
	text-decoration: none;
	border: 1px solid #ffffff;
}

.btn:hover {
	color: #000;
}

.btn:after {
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
}

.btn:hover:after {
	width: 100%;
	transition: 0.2s all ease;
}
</style>
