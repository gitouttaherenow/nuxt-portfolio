<template>
  <div id="work">
    <section class="project-wrap">
      <div class="container">
        <div class="grid">
          <!-- <div class="col-lg-6 col-md-6 col-sm-12"> -->
          <!-- <WorkCard :workImageURL="imageURL" /> -->
          <WorkCard
            v-for="work in workList"
            :key="work.id"
            :title="work.title.rendered"
            :workImageURL="work._embedded['wp:featuredmedia']['0'].source_url"
          ></WorkCard>
          <!-- </div> -->
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import WorkCard from "@/components/Workcard";
import axios from 'axios'

// const url = "https://reqres.in/api/users";
const url = "http://www.thoshikesh.com/wp-json/wp/v2/posts?_embed";

export default {
  components: {
    WorkCard
  },
  
  data() {
    return {workList: []}
    /*return {
      workList: [
        {
          id: 1,
          title: "Aditya Auto Systems",
          imageURL: require("~/static/work/work1.jpg")
        },
        {
          id: 2,
          title: "Stellify GmbH",
          imageURL: require("~/static/work/work2.jpg")
        },
        {
          id: 3,
          title: "Rachel Cole",
          imageURL: require("~/static/work/work3.jpg")
        },
        {
          id: 4,
          title: "Webkriya",
          imageURL: require("~/static/work/work4.jpg")
        }
      ]
    };*/
  },
  mounted() {
    axios.get(url)
    .then(response => {
      this.workList = response.data
    })
  },
};
</script>
