<template>
  <div class="home">
    <div class="container">
    </div>
  </div>
</template>

<script>
import { apiService } from "../common/api.service.js";
export default {
  name: "home",

  data(){
    return {
      questions: []
    }
  },

  methods: {
    getQuestions(){
      let endpoint = "/api/questions/";
      apiService(endpoint).then(data => { this.questions.push(...data.results) })
    }
  },

  created(){
    this.getQuestions()
    console.log(this.questions)
  }
};
</script>
