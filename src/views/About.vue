<template>
    <div class="about">
        <h1>{{ pageName }}</h1>
        <p>{{ pageDescription }}</p>
        <form action="POST">
            
            <input type="text" v-model="name" >
        </form>
        <p> my  name is : "{{name}}" </p>
        <p>my age is : "{{age}}"</p>
        <!-- <p>methods in age</p>
        <p>{{calcAge()}}</p> -->
        <p>Computed Properties in age </p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <p>{{calcAge}}</p>
        <form action="">
            <label for="">syrian poinds</label>
            <input type="text" v-model="sy">
            <label for="">us Dolair </label>
            <input type="text" v-model="us">
        </form>

    </div>
</template>

<script>
export default {
    data: function () {
        return {
            pageName: "About us",
            pageDescription: "This is About us page ",
            name : "Enter your name",
            age : 19,
            sy : 0,
            us : 0,
        };

    },
    methods : {
         
    },
    computed: {
         calcAge : function (){
            console.log("run")
            return this.age * 2;
        }  
        }  ,
        watch : {
            sy : function (v){
                this.us = v / 3500;
                console.log('sy run');
            }  , 
            us : function (y){
                this.sy = y * 3500;
                console.log('us run')
            }
        },
    name: "About",
     
};
</script>

