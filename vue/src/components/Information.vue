<template>
    <div class="information">
        <p class="copyrights"><small>&copy; 2023 Zerotype. All Rights Reserved.</small></p>
        <div class="social_media">
            <a 
                v-for="media in social_medias"
                :key="media.media"
                :href="media.link">
                <i :class="media.class"></i>
            </a>
        </div>    
    </div> 
</template>

<script>
export default {
    data:function(){
        return{
            social_medias:[
                {media:'facebook',class:['fab','fa-facebook-square'],link:'#'},
                {media:'googleplus',class:['fab','fa-google-plus-square'],link:'#'},
                {media:'twitter',class:['fab','fa-twitter-square'],link:'#'},
                {media:'pinterest',class:['fab','fa-pinterest-square'],link:'#'}
            ]
        }
    }
};
</script>

<style>

    .information {
    width: 990px;
    font-size: 0;
    margin: 0 auto;
    }

    .copyrights {
    display: inline-block;
    font-size: 14px;
    color: #888;
    line-height: 40px;
    }

    .social_media {
    float: right;
    }

    .social_media a {
    display: inline-block;
    font-size: 40px;
    line-height: 40px;
    }

    .social_media a + a {
    margin-left: 20px;
    }

    .fab {
    color: #222;
    }

    .fab:hover {
    color: orange;
    }

    .information:after { 
    content: "";
    display: block; 
    clear: both;
    }


</style>