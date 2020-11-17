<template>
        <section class="description">
            <article>
            <h3>This is just a place holder.</h3>
            <p v-for="(p,index) in article.paragraph" :key="p+index">{{p}}</p>

            </article>
        </section>
</template>

<script>
export default {
    data:  function(){
        return{
            article:{
                title: 'This is just a place holder.',
                paragraph:[
                    `You can remove any link to our website from this website template, you're free to use this website template without linking back to us.`,
                    `This is just a place holder, so you can see what the site would look like.`,
                    `You can remove any link to our website from this website template, you're free to use this website template without linking back to us. This is just a place holder, so you can see what the site would look like.`,
                    `You can remove any link to our website from this website template, you're free to use this website template without linking back to us. This is just a place holder, so you can see what the site would look like.`,
                    `This is just a place holder, so you can see what the site would look like.`,
                    `You can remove any link to our website from this website template, you're free to use this website template without linking back to us.`
                ],
            }
        }
    }
};
</script>


<style>
    .description {
    padding: 50px 0 235px;
    }

    article {
    width: 950px;
    margin: 0 auto;
    column-count: 2;
    column-gap: 50px;
    }

    article h3{
    column-span: all;
    margin-bottom: 20px;
    }

    article p:not(:nth-of-type(3n)) {
    margin-bottom: 20px;
    }
</style>