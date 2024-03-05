<template>
  <div>
    <footer class="footer container">
    <div class="footer__interno_logo">
      <img class="footer__interno_logoImg" src="../assets/img/logo.png" alt="logo">
      <p class="footer__interno_about">It is a long established fact that a reader <br> will be distracted lookings.</p>
      <div class="footer__inyerno_social">
        <a href="#">
          <img src="../assets/img/tweeter.svg" alt="tweeter">
        </a>
        <a href="#">
          <img src="../assets/img/insta.svg" alt="instagram">
        </a>
      </div>
    </div>
    <div class="footer__pages">
      <h4 class="footer__pages_subtitle">Pages</h4>
      <div class="footer__pages_items">
        <a class="footer__pages_item" href="#">Home</a>
        <a class="footer__pages_item" href="#">Project</a>
        <a class="footer__pages_item" href="#">Blog</a>
      </div>
    </div>
    <div class="footer__contact">
      <h4 class="footer__contact_subtitle">Contact</h4>
      <p class="footer__contact_address">55 East Birchwood Ave. <br> Brooklyn, New York 11201 <br><span class="footer__contact_mail">contact@interno.com </span><br>
        (123) 456 - 7890</p>  
    </div>
  </footer>
  </div>
</template>

<script>
  export default {
    
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