<template>
    <div class="blog">
        <h1> {{pageName}} </h1>
        <div class="container">
          <div class="row">
              <div class="col-md-8">
                <div class="posts-area">
                    <blog-posts v-for="post in posts" v-bind:key="post.id" :views="post.views"  :title="post.title" :content="post.content" :auther="post.auther" :date="post.date" :category="post.category" />
                </div>
              </div>
              <div class="col-md-4">
                  <div class="sidebar">
                      <sidebar/>
                  </div>
              </div>
          </div>
        </div>        
    </div>
</template>

<script>
import BlogPosts from '../components/BlogPosts.vue';
import sidebar from '../components/sidebar.vue';
import json from '../json/BlogPost.json';
export default {
    name: "blog",
    components: {
        BlogPosts,
        sidebar
    } ,
    
    data : function(){
        return{
            pageName : "Blog Page",
            posts : json
        }
    }

};
</script>

<style lang="scss" scoped>
.blog {
    overflow: hidden;
    color: #fff;
    h1 {
        height: 300px;
        display: inline-block;
        font-size: 50px;
        padding: 100px;
    }
}
</style>
