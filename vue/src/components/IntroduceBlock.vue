<template>
    <section class="introduce">
        <div class="main_introduce">
        <div class="introduce_left">
            <h2>{{article.title}}</h2>
            <h3>{{article.subtitle}}</h3>
            <p>{{article.paragraph}}</p>
            <div class="button_area">
            <div class="button_with_text">
                <a class="button" :href="button.link">{{button.hintText}}</a>
                <span>Don't worry. It's free.</span>
            </div>
            </div>
        </div>
        <div class="introduce_right">
            <img :src="article.image" alt="收納大箱子" />
        </div>
        </div>
    </section>
</template>

<script>
export default {
    data(){
        return{
            article:{
                title: 'IDEAS?',
                subtitle: 'This is just a place holder.',
                paragraph: `You can remove any link to our website from this website template, you're free to use this website template without linking back to us.`,
                image: require('../assets/box.png')
            },
            button:{
                hintText: 'TRY IT NOW!',
                link: '#'
            }
        }
    }
};
</script>

<style>

    .introduce {
    background-color: #FDFDFD;
    padding: 60px 0 100px;
    }

    .main_introduce {
    width: 950px;
    margin: 0 auto;
    font-size: 0;
    }

    .introduce_left {
    display: inline-block;
    width: 425px;
    margin-left: 25px;
    vertical-align: top;
    }

    h2 {
    font-size: 64px;
    font-weight: 400;
    margin: 0 0 -15px;
    }

    h3 {
    font-size: 34px;
    font-weight: 400;
    color: #333;
    margin: 0;
    
    }

    p {
    font-size: 18px;
    line-height: 28px;
    color: #777;
    text-align: justify;
    margin: 0;
    }

    .button_area {
    margin-top: 24px;
    }

    .button_with_text {
    width: 260px;
    margin: 0 auto;
    }

    .button {
    display: inline-block;
    width: 260px;
    height: 70px;
    background: linear-gradient(#FFBA55 55%, #F99600 45%);
    border-radius: 10px;
    cursor: pointer;
    text-align: center;
    line-height: 70px;
    color: white;
    font-size: 24px;
    letter-spacing: 2px;
    text-decoration: none;
    }

    .button:hover {
    color: white;
    }

    .button_with_text span {
    font-size: 15px;
    color:  #777;
    }

    .introduce_right {
    display: inline-block;
    width: 450px;
    margin-left: 50px;
    }

    .introduce_right img{
    width: 100%;
    }

</style>