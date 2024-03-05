<template>
  
  <HeaderComponent/>

  <section class="top">
    <div class="top__about">
      <h2 class="top__title">Articles & News</h2>
      <p class="top__text">Home / Blog</p>
    </div>
    <img class="top__img" src="../assets/img/banner-blog.jpg" alt="banner">
  </section>

  <section class="blog container">
    <h2 class="blog__title">Latest Post</h2>
    <div class="blog__latest">
      <img class="blog__latest_img" src="../assets/img/blog-latest.jpg" alt="blogImg">
      <div class="blog__latest_about">
        <h5 class="blog__latest_subtitle">Low Cost Latest Invented Interior Designing Ideas</h5>
        <p class="blog__latest_text">Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpis dignissim maximus.posuere in.Contrary to popular belief. <br><br> Lorem Ipsum is not simply random text. It has roots in a piece of classica.
        </p>
        <div class="blog__date_info">
          <p class="blog__date">26 December,2022</p>
          <a href="#" class="blog__button">
            <img class="blog__arrow background_dark" src="../assets/img/arrow-r-blog.svg" alt="arrow">
          </a>
        </div>
      </div>
    </div>
    <div class="blog__news">
      <h2 class="blog__title">Articles & News</h2>
      <div class="blog__items" id="hwork">
        <div v-for="article in articles" :key="article.id">
          <div class="blog__cart">
            <p class="blog__tag">{{ ArticlesComponent.imgText }}</p>
            <img class="blog__img" :src= "ArticlesComponent.image" :alt="blogImg">
            <h4 class="blog__subtitle">{{ ArticlesComponent.itemTitle }}</h4>
            <div class="blog__date_info">
              <p class="blog__date"> {{ ArticlesComponent.itemData }}</p>
              <a href="#" class="blog__button">
                <img class="blog__arrow background_dark" src="../assets/img/arrow-r-blog.svg" alt="arrow">
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <FooterComponent/>  

</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';
import ArticlesComponent from '@/components/ArticlesComponent.vue';

  export default {
    name: 'BlogPage',
    comments: {
      HeaderComponent,
      FooterComponent,
      ArticlesComponent
    }
  }
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

a {
  text-decoration: none;
  color: inherit;
}

ul {
  list-style: none;
}

.container {
  max-width: 1200px;
  margin: 0 auto;
}

  .top{
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 200px;
}

.top__about{
  position: absolute;
  padding: 41px 78px;
  background-color: #FFFFFF;
  border-radius: 37px 37px 0 0;
  margin-top: 178px;
}

.top__title{
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0em;
  text-align: left;
  color: #292F36;
}

.top__text{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  text-align: center;
}

.blog{
  margin-bottom: 300px;
}

.blog__title{
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0.02em;
  text-align: left;
  margin-bottom: 27px;
  color: #292F36;
}

.blog__latest{
  display: flex;
  padding: 22px;
  border: 1px solid #E7E7E7;
  border-radius: 62px;
  margin-bottom: 150px;
}

.blog__latest_img{
  border-radius: 50px;
  margin-right: 65px;
}

.blog__latest_about{
  max-width: 470px;
}

.blog__latest_subtitle{
  margin-top: 51px;
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0.02em;
  text-align: left;
  color: #292F36;
  margin-bottom: 22px;
}

.blog__latest_text{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  margin-bottom: 41px;
}

.details__banner{
  display: flex;
  justify-content: center;
  margin-bottom: 200px;
}

.blog-details{
  display: flex;
  margin-bottom: 96px;
}
</style>