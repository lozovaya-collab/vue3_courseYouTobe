<template>
  <!--разметка компонента-->
  <div class="app">
    
    
  </div>
</template>
<script>
// описываем логику, обьявляем данные, пишем функции

// экспортируем объект (компонент)
export default {
  data() {
    return {
      posts: [
        { id: 1, title: "JS 1", body: "Описание 1" },
        { id: 2, title: "JS 2", body: "Описание 2" },
        { id: 3, title: "JS 3", body: "Описание 3" },
        { id: 4, title: "JS 4", body: "Описание 4" },
        { id: 5, title: "JS 5", body: "Описание 5" },
      ],
      title: "",
      body: "",
    };
  },
  methods: {
     createPost(){
       const newPost = {
         id: Date.now(),
         title: this.title,
         body: this.body,
       }

       this.posts.push(newPost)
       this.title = ""
       this.body = ""
     },
     
  },
  
};
</script>
<style>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.app {
  padding: 20px;
}


</style>
