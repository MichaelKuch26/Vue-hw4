<template>
  
  <HeaderComponent/>

  <main class="main-blog-details">
    <section class="details__banner">
        <img src="../assets/img/banner-det.jpg" alt="banner">
    </section>
    <div class="blog-details container">
        <SortedComponent/>
    </div>
</main>

  <FooterComponent/>
  
</template>

<script>
import HeaderComponent from '@/components/HeaderComponent.vue';
import FooterComponent from '@/components/FooterComponent.vue';
import SortedComponent from '@/components/SortedComponent.vue';

  export default {
    name: 'BlogDetailsPage',
    comments: {
      HeaderComponent,
      FooterComponent,
      SortedComponent
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

.header{
  margin-top: 44px;
  display: flex;
  flex-direction: row;
  flex-wrap: nowrap;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 57px;
}

.header__logo{
  height: 50px;
}

.header__links {
  display: flex;
  text-align: center;
  gap: 50px;
  font-size: 20px;
  line-height: 25px;
  align-items: center;
  font-family: "Jost";
  font-weight: 400;
  color: #292F36;
}

.bd__article-one_title{
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0.02em;
  text-align: left;
  color: #292F36;
  margin-bottom: 21px;
  width: 686px;
}

.bd__article-one_img{
  border-radius: 50px;
  margin-bottom: 46px;
}

.bd__article-one_date{
  font-family: "Jost";
  font-size: 16px;
  font-weight: 400;
  line-height: 24px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  display: flex;
  justify-content: space-between;
  margin-bottom: 48px;
  width: 800px;
}

.bd__article-one_text{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  margin-bottom: 35px;
  width: 800px;
}

.blockquote{
  margin-bottom: 27px;
  background-color: #F4F0EC;
  border-radius: 50px;
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 800px;
}

.blockquote__sign{
  /* font-family: "DM Serif Display";
  font-size: 200px;
  font-style: italic;
  font-weight: 400;
  line-height: 250px;
  letter-spacing: 0.02em; */
  text-align: center;
  color: #CDA274;
  /* -webkit-transform: rotate(180deg); */
  padding-top: 83px;
  margin-left: 40px;
}

.blockquote__text{
  font-family: "DM Serif Display";
  font-size: 25px;
  font-style: italic;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0.02em;
  text-align: center;
  color: #CDA274;
  max-width: 345px;
  align-items: center;
  /* margin-top: -40px; */
  padding-bottom: 73px;;
}

.bd__article-two_title{
  font-family: "DM Serif Display";
  font-size: 50px;
  font-weight: 400;
  line-height: 63px;
  letter-spacing: 0.02em;
  text-align: left;
  color: #292F36;
  margin-bottom: 20px;
}

.bd__article-two_text{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  width: 800px;
  margin-bottom: 24px;
}

ol {
  list-style-type: none; 
  counter-reset: my-counter; 
}

li::before {
  content: counter(my-counter); 
  counter-increment: my-counter; 
  color: #CDA274;
  margin-right: 0.5em;
}

.bd__article-two_points{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  margin-bottom: 44px;
  width: 730px;
  display: flex;
}

.blog-details__number{
  color: #CDA274;
  margin-right: 10px;
}

.bd__article-two_img{
  border-radius: 50px;
  margin-bottom: 35px;
}

.bd__article-two_subtext{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  color: #4D5053;
  width: 800px;
}

.blog-details__tags{
  margin-left: 52px;
}

.bd__tags_title{
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0.02em;
  text-align: left;
  color: #292F36;
  margin-bottom: 24px;
}

.bd__tags_aside {
  display: flex;
  flex-direction: column;
  gap: 23px;
  margin-left: 52px;
}
.bd__tags_buttons {
  display: flex;
  flex-direction: row;
  gap: 10px;
  flex-wrap: wrap;
}
.bd__tags_button {
  display: flex;
  flex-direction: row;
  flex-wrap: wrap;
  gap: 10px;
  padding: 10px 30px;
  color: #292f36;
  text-align: center;
  font-family: Jost;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: 125%;
  letter-spacing: 0.36px;
  border-radius: 10px;
  background: #f4f0ec;
  border: none;
}
.bd__tags_button input[type=radio] {
  display: none;
}
.bd__tags_button-active {
  background: #292f36;
  color: #ffffff;
}

.footer{
  display: flex;
  margin-bottom: 134px;
  justify-content: space-between;
  color: #4D5053;
}

.footer__interno_logoImg{
  height: 50px;
  margin-bottom: 18px;
}

.footer__interno_about{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
  margin-bottom: 31px;
}

.footer__inyerno_social{
  display: flex;
  gap: 55px;
}

.footer__pages_subtitle{
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 10px;
}

.footer__pages_items{
  display: flex;
  flex-direction: column;
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 66px;
  letter-spacing: 0.01em;
  text-align: left;
}

.footer__contact_subtitle{
  font-family: "DM Serif Display";
  font-size: 25px;
  font-weight: 400;
  line-height: 31px;
  letter-spacing: 0em;
  text-align: left;
  margin-bottom: 26px;
}

.footer__contact_address{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 33px;
  letter-spacing: 0.01em;
  text-align: left;
}

.footer__contact_mail{
  font-family: "Jost";
  font-size: 22px;
  font-weight: 400;
  line-height: 100px;
  letter-spacing: 0.01em;
  text-align: left;
}
</style>