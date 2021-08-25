<template>
    <div class="post-box">
        <span class="post-views"> {{views}} </span>
        <h1 class="post-title">
            {{title}} 
        </h1>
        <div class="post-content">
            {{content}}
        </div>
        <div class="row">
                <div class="col-sm-6">
                 <span class="post-auther">  {{auther}} </span>
                </div>
                <div class="col-sm-6">
                    <span class="post-category"> {{category}} </span>
                </div>
            </div>
            <span class="post-data"> {{date}} </span>
    </div>
    
</template>

<script>
export default {
    props : ["views","title","content","auther","date","category"],
    name : "post",
};
</script>


