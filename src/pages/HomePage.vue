<template>

  <HeaderComponent/>

  <section class="promo container">
    <img class="bannerImg" src="../assets/img/banner.jpg" alt="banner">
    <div class="intro__content">
      <h1 class="intro__title">Let Your Home 
        Be Unique</h1>
      <p class="intro__text">There are many variations of the passages of
        lorem Ipsum fromavailable, majority.</p>
      <a class="intro__button" href="#">
        Get Started
        <img class="intro__arrow" src="../assets/img/arrow-r.svg" alt="arrow">
      </a>
    </div>
  </section>

  <section class="projects container">
    <h2 class="projects__subtitle">Follow Our Projects</h2>
    <p class="projects__text">It is a long established fact that a reader will be distracted by the of readable <br> content of page  lookings at its layouts  points.</p>
    <div class="projects__items">
      <div class="project__item">
        <img class="projectImg1" src="../assets/img/project1.jpg" alt="project">
        <div class="project__content">
          <div class="project__about">
            <p class="project__name_text">Modern Kitchan</p>
            <p class="project__about_text">Decor / Artchitecture</p> 
          </div>
          <a class="project__button" href="#" >
            <img class="project__arrow" src="../assets/img/arrow-r-proj.svg" alt="arrow">
          </a>
        </div>
        
      </div>
      <div class="project__item">
        <img class="projectImg2" src="../assets/img/project2.jpg" alt="project">
        <div class="project__content">
          <div class="project__about">
            <p class="project__name_text">Modern Kitchan</p>
            <p class="project__about_text">Decor / Artchitecture</p> 
          </div>
          <a class="project__button" href="#" >
            <img class="project__arrow" src="../assets/img/arrow-r-proj.svg" alt="arrow">
          </a>
        </div>
        
      </div>
      <div class="project__item">
        <img class="projectImg3" src="../assets/img/project3.jpg" alt="project">
        <div class="project__content">
          <div class="project__about">
            <p class="project__name_text">Modern Kitchan</p>
            <p class="project__about_text">Decor / Artchitecture</p> 
          </div>
          <a class="project__button" href="#" >
            <img class="project__arrow" src="../assets/img/arrow-r-proj.svg" alt="arrow">
          </a>
        </div>
        
      </div>
      <div class="project__item">
        <img class="projectImg4" src="../assets/img/project4.jpg" alt="project">
        <div class="project__content">
          <div class="project__about">
            <p class="project__name_text">Modern Kitchan</p>
            <p class="project__about_text">Decor / Artchitecture</p> 
          </div>
          <a class="project__button" href="#" >
            <img class="project__arrow" src="../assets/img/arrow-r-proj.svg" alt="arrow">
          </a>
        </div>
        
      </div>
    </div>
  </section>

  <section class="statistics">
    <div class="statistics__counter container">
      <div class="statistics__items">
        <div class="statistics__info">
          <p class="statistics__number">12</p>
          <p class="statistics__about">Years Of Experiance</p>
        </div>
        <img class="statistics__line" src="../assets/img/line.svg" alt="line">
      </div>
      <div class="statistics__items">
        <div class="statistics__info">
          <p class="statistics__number">85</p>
          <p class="statistics__about">Success Project</p>
        </div>
        <img class="statistics__line" src="../assets/img/line.svg" alt="line">
      </div>
      <div class="statistics__items">
        <div class="statistics__info">
          <p class="statistics__number">15</p>
          <p class="statistics__about">Active Project</p>
        </div>
        <img class="statistics__line" src="../assets/img/line.svg" alt="line">
      </div>
      <div class="statistics__items">
        <div class="statistics__info">
          <p class="statistics__number">95</p>
          <p class="statistics__about">Happy Customers</p>
        </div>
      </div>
    </div>
  </section>

  <section class="blog container">
    <h2 class="blog__title">Articles & News</h2>
    <p class="blog__text">It is a long established fact that a reader will be distracted by the of readable content <br> of a page when lookings at its layouts the points of using.</p>
    <div class="blog__items">
      <div class="blog__cart">
        <p class="blog__tag">Kitchan Design</p>
        <img class="blog__img" src="../assets/img/blogImg1.jpg" alt="blogImg">

        <h4 class="blog__subtitle">Let’s Get Solution For <br> Building Construction <br> Work</h4>
        <div class="blog__date_info">
          <p class="blog__date">26 December,2022</p>
          <a href="#" class="blog__button">
            <img class="blog__arrow background_dark" src="../assets/img/arrow-r-blog.svg" alt="arrow">
          </a>
        </div>
      </div>
      <div class="blog__cart background_dark">
        <p class="blog__tag">Living Design</p>
        <img class="blog__img" src="../assets/img/blogImg2.jpg" alt="blogImg">
        <h4 class="blog__subtitle">Low Cost Latest Invented <br> Interior Designing <br> Ideas.</h4>
        <div class="blog__date_info">
          <p class="blog__date">22 December,2022</p>
          <a href="#" class="blog__button">
            <img class="blog__arrow background_light" src="../assets/img/arrow-r-blog.svg" alt="arrow">
          </a>
        </div>
      </div>
      <div class="blog__cart">
        <p class="blog__tag">Interior Design</p>
        <img class="blog__img" src="../assets/img/blogImg3.jpg" alt="blogImg">
        <h4 class="blog__subtitle">Best For Any Office & <br> Business Interior <br> Solution</h4>
        <div class="blog__date_info">
          <p class="blog__date">25 December,2022</p>
          <a href="#" class="blog__button">
            <img class="blog__arrow background_dark" src="../assets/img/arrow-r-blog.svg" alt="arrow">
          </a>
        </div>
      </div>
    </div>
  </section>

  <FooterComponent/>
  
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';

export default {
  name: 'HomePage',
  components: {
    HeaderComponent,
    FooterComponent,
  }
}
</script>

<style lang="scss">
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

.promo{
  position: relative;
}

.bannerImg{
  border-radius: 60px;
  position: absolute;
  z-index: -999;
}

.intro__content{
  width: 490px;
}

.intro__title{
  padding: 208px 0 18px 52px;
  font-family: "DM Serif Display";
  font-weight: 400;
  font-size: 65px;
  color: #292F36;
}

.intro__text{
  padding: 0 0 47px 52px;
  font-family: "Jost";
  font-weight: 400;
  font-size: 22px;
  line-height: 33px;
  color: #4D5053;
}

.intro__button{
  margin-left: 52px;
  border-radius: 18px;
  padding: 26px 49px 26px 49px;
  background: #292F36;
  font-family: "Jost";
  font-weight: 600;
  font-size: 18px;
  line-height: 22.5px;
  color: #FFFFFF;
  cursor: pointer;
}

.intro__arrow{
  margin: 0px 0 -2px 10px;
}

.projects{
  margin-top: 304px;
  margin-bottom: 96px;
}

.projects__subtitle{
  text-align: center;
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0.02em;
  margin-bottom: 8px;
  color: #292F36;
}

.projects__text{
  text-align: center;  
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  margin-bottom: 93px;
  color: #4D5053;
}

.projects__items{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  gap: 80px;
  flex-wrap: wrap;
}

.project__item{
  max-width: 525px;
}

.projectImg1{
  border-radius: 0 80px 0 0;
  margin-bottom: 24px;
  width: 100%;
}

.project__content{
  display: flex;
  justify-content: space-between;
}

.project__name_text{
  margin-bottom: 4px;
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0.02em;
  text-align: left;
  color: #292F36;
}

.project__about_text{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
}

.project__button{
  border-radius: 50px;
  background: #F4F0EC;
  cursor: pointer;
}

.project__arrow{
  padding: 23px 31px 22px 32px;
}

.projectImg2{
  border-radius: 80px 0 0 0;
  margin-bottom: 24px;
  width: 100%;
}

.projectImg3{
  border-radius: 0 0 80px 0;
  margin-bottom: 24px;
  width: 100%;
}

.projectImg4{
  border-radius: 0 0 0 80px;
  margin-bottom: 24px;
  width: 100%;
}

.statistics{
  background-color: #F4F0EC;
  margin-bottom: 96px;
}

.statistics__counter{
  padding-top: 151px;
  padding-bottom: 151px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
}

.statistics__items{
  display: flex;
}

.statistics__info{
  margin-right: 44px;
}

.statistics__number{
  font-family: "DM Serif Display";
  font-size: 85px;
  font-weight: 400;
  line-height: 106px;
  letter-spacing: 0.02em;
  text-align: left;
  padding: 0 57px 16px 57px;
  color: #CDA274;
}

.statistics__about{
  font-family: "Jost";
  font-size: 22px;  
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: center;
  color: #4D5053;
}

.statistics__line{
  margin-right: 76px;
}

.blog{
  margin-bottom: 96px;
}

.blog__title {
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0.02em;
  text-align: center;
  margin-bottom: 12px;
}

.blog__text {
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: center;
  margin-bottom: 52px;
}

.blog__items{
  display: flex;
  justify-content: center;
  gap: 27px;
  flex-wrap: wrap;
}

.blog__cart{
  width: 382px;
  border-radius: 50px 50px 50px 50px;
  border: 1px solid #E7E7E7;
  padding: 20px;
}

.background_dark {
  background-color: #F4F0EC;
}

.background_light {
  background-color: #FFF;
}

.blog__tag{
  position: absolute;
  padding: 8px 11px 8px 11px;
  margin-top: 228px;
  margin-left: 20px; 
  border-radius: 8px 8px 8px 0px;
  background: #FFFFFF;
  font-family: "Jost";
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  color: #4D5053;
}

.blog__img{
  border-radius: 45px 45px 0px 0px;
}

.blog__date_info{
  display: flex;
  justify-content: space-between;
  align-items: center;
  text-align: center;
}

.blog__subtitle{
  margin-top: 10px;
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0.02em;
  text-align: left;
  margin-bottom: 30px;
  white-space: pre-line;
}

.blog__date{
  padding-top: 15px;
  font-family: "Jost";
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  padding-bottom: 15px;
}

.blog__arrow{
  padding: 20px 23px 20px 23px;
  border-radius: 50px;
  cursor: pointer;
}
</style>
