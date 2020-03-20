<template>
  <div id="work">
    <section class="project-wrap">
      <div class="container">
        <div class="grid">
          <WorkCard
            v-for="work in portfolio"
            :key="work.id"
            :title="work.title.rendered"
            :workImageURL="work._embedded['wp:featuredmedia']['0'].source_url"
          ></WorkCard>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import WorkCard from "@/components/Workcard";
import axios from 'axios'

const url = "http://www.thoshikesh.com/wp-json/wp/v2/posts?_embed";

export default {
  components: {
    WorkCard
  },
  
  data() {
    return {workList: []}
  },
  mounted() {
    axios.get(url)
    .then(response => {
      this.workList = response.data
    })
  },
};
</script>
