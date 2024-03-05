<template>
  <div>
    <div class="blog-details__articles">
              <article class="bd__article-one" v-for="article in sortedArray" :key="article.id" :id="article.id">
              <h2 class="bd__article-one_title">{{ article.title }}</h2>
              <div class="blog-details__image-data-box">
                  <img :src="article.src" alt="article.alt" class="bd__article-one_img">
                  <div class="bd__article-one_date">
                      <p class="blog-details__date">{{ article.date }}</p>
                      <p class="blog-details__links">{{ article.link }}</p>
                  </div>
              </div>
              <p class="bd__article-one_text">{{ article.firstpargth }}</p>
              <p class="bd__article-one_text">{{ article.secondpargth }}</p>
              <div class="blockquote">
                  <div class="blockquote__sign">
                      <svg width="74" height="56" viewBox="0 0 74 56" fill="none" xmlns="http://www.w3.org/2000/svg">
                          <path
                              d="M58.7516 0.600003C63.1516 0.600003 66.7516 2.06667 69.5516 5C72.2182 7.93334 73.5516 11.8667 73.5516 16.8C73.5516 25.4667 70.6849 33 64.9516 39.4C59.0849 45.8 52.0849 51.0667 43.9516 55.2L41.9516 51.8C45.2849 49.6667 48.4182 46.9333 51.3516 43.6C54.1516 40.2667 56.3516 36.6667 57.9516 32.8L52.3516 28.6C50.0849 27.1333 48.2182 25.1333 46.7516 22.6C45.2849 20.2 44.5516 17.8667 44.5516 15.6C44.5516 11.3333 45.8849 7.73334 48.5516 4.8C51.0849 2 54.4849 0.600003 58.7516 0.600003ZM17.5516 0.599999C21.9516 0.6 25.5516 2.06667 28.3516 5C31.0182 7.93333 32.3516 11.8667 32.3516 16.8C32.3516 25.4667 29.4849 33 23.7516 39.4C17.8849 45.8 10.8849 51.0667 2.75156 55.2L0.751558 51.8C4.08489 49.6667 7.21823 46.9333 10.1516 43.6C12.9516 40.2667 15.1516 36.6667 16.7516 32.8L11.1516 28.6C8.88489 27.1333 7.01823 25.1333 5.55156 22.6C4.08489 20.2 3.35156 17.8667 3.35156 15.6C3.35156 11.3333 4.6849 7.73333 7.35156 4.8C9.8849 2 13.2849 0.599999 17.5516 0.599999Z"
                              fill="#CDA274" />
                      </svg>
                      <p class="blockquote__text">{{ article.quote }}</p>
                  </div>
              </div>
              <h3 class="bd__article-two_title">{{ article.subtitle }}</h3>
              <p class="bd__article-two_text">{{ article.thirdpargth }}</p>
              <div v-for="numberandtext in numbersandtexts" class="bd__article-two_points">
                  <p class="blog-details__number">{{ numberandtext.number }}</p>
                  <p class="blog-details__text">{{ numberandtext.text }}</p>
              </div>
              <img class="bd__article-two_img" :src="article.secondsrc" :alt="article.alt">
              <p class="bd__article-two_subtext">{{ article.thirdpargth }}</p>
              </article>
          </div>
          
          <div class="bd__tags_aside">
              <h3 class="bd__tags_title">{{title}}</h3>
              <div class="bd__tags_buttons"> 
                  <div v-for="button in buttons"                class="bd__tags_button">
                  <label :data-id="button.id" @change="sortArticles"><input  :data-id="button.id" @click="filters" class="blog-details__input" type="radio" name="radio">
                  {{button.text}}</label>
                  </div>
              </div>
          </div>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        sortedArray: [
            {
              id: 'kitchen', 
              title: 'Let’s Get Solution for Building Construction Work', date: '26 December,2022', 
              link: 'Interior / Home / Decore', 
              firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don’t look even slightly believable.', 
              secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
              src: '../assets/img/articleImg-one.jpg', 
              alt: 'photo', 
              quote: 'The details are not the details. They make the design.', 
              subtitle: 'Design sprints are great', 
              thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
              firstnumber: '1', 
              secondnumber: '2', 
              thirdnumber: '3', 
              fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
              secondsrc: '../assets/img/articleImg-two.jpg' 
            }],

          articles: [
              { 
                id: 'kitchen',           
                title: 'Let’s Get Solution for Building Construction Work', date: '26 December,2022', 
                link: 'Interior / Home / Decore', 
                firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don’t look even slightly believable.', 
                secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
                src: '../assets/img/articleImg-one.jpg', 
                alt: 'photo', 
                quote: 'The details are not the details. They make the design.', 
                subtitle: 'Design sprints are great', 
                thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                firstnumber: '1', 
                secondnumber: '2', 
                thirdnumber: '3', 
                fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                secondsrc: '../assets/img/articleImg-two.jpg' 
              },
              { 
                id: 'bedroom', 
                title: 'Low Cost Latest Invented Interior Designing Ideas.', date: '22 December,2022', 
                link: 'Interior / Home / Decore', 
                firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don t look even slightly believable.', 
                secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
                src: '../assets/img/blogImg6.jpg', 
                alt: 'photo', 
                quote: 'The details are not the details. They make the design.', 
                subtitle: 'Design sprints are great', 
                thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                firstnumber: '1', 
                secondnumber: '2', 
                thirdnumber: '3', 
                fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                secondsrc: '../assets/img/blogImg6.jpg' 
              },
              { 
                id: 'building', 
                title: 'Building, a usually roofed and walled structure built for permanent use.', 
                date: '20 December,2022', 
                link: 'Country / City / Building', 
                firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don t look even slightly believable.', 
                secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
                src: '../assets/img/blogImg5.jpg', 
                alt: 'photo',
                quote: 'Good buildings come from good people, and all problems are solved by good design.', 
                subtitle: 'We shape our buildings; thereafter, they shape us.', 
                thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                firstnumber: '1', 
                secondnumber: '2', 
                thirdnumber: '3', 
                fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                secondsrc: '../assets/img/blogImg5.jpg' 
              },
              { 
                id: 'architecture', 
                title: 'Our paper emphasizes the importance of the kitchen layout in facilitating consumers food hygiene practices.', date: '29 December,2022', 
                link: 'Country / City / Architecture', 
                firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don t look even slightly believable.', 
                secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
                src: '../assets/img/blogImg4.jpg', 
                alt: 'photo', 
                quote: 'Architecture is a visual art, and the buildings speak for themselves.', 
                subtitle: 'Architecture around the world by contemporary architects including cutting-edge houses, skyscrapers, cultural buildings, hotels, airports, apartments.', 
                thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                firstnumber: '1', 
                secondnumber: '2', 
                thirdnumber: '3', 
                fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                secondsrc: '../assets/img/blogImg4.jpg' 
              },
              { 
                id: 'kitchen-planning', 
                title: 'Kitchen Planning: Selecting the Right Layout', 
                date: '25 December,2022', 
                link: 'Interior / Home / Kitchen', 
                firstpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered alteration in some form, by injecthumour, or randomised words which don t look even slightly believable.', 
                secondpargth: 'Embarrassing hidden in the middle of text. All the Lorem Ipsum generators on the Internet tend to repeat predefined chunks as necessary.', 
                src: '../assets/img/blogImg3.jpg', 
                alt: 'photo', 
                quote: 'The kitchen is the heart of the home.', 
                subtitle: 'Kitchens should be designed around whats truly important – fun, food, and life.', 
                thirdpargth: 'Lorem ipsum dolor sit amet, adipiscing Aliquam eu sem vitae turpmaximus.posuere in.Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                firstnumber: '1', 
                secondnumber: '2', 
                thirdnumber: '3', 
                fourthpargth: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.', 
                secondsrc: '../assets/img/blogImg3.jpg' 
              }],

          numbersandtexts: [
              { 
                number: '1', 
                text: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.' 
              },
              { 
                number: '2', 
                text: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.' 
              },
              { 
                number: '3', 
                text: 'Contrary to popular belief.There are many variations of passages of Lorem Ipsum available, but the majority have suffered.' 
              }],
          buttons: [
            { 
              id: 'kitchen', 
              text: 'Kitchen' 
            }, 
            { 
              id: 'bedroom', 
              text: 'Bedroom' 
            }, 
            {
              id: 'building', 
              text: 'Building' 
            }, 
            { 
              id: 'architecture', 
              text: 'Architecture' 
            }, 
            { 
              id: 'kitchen-planning', 
              text: 'Kitchen Planning' 
            }],
          title: 'Tags'
      };
  },
  methods: {
    sortArticles(e) {
        console.log(e.target);
        if (document.querySelector('.bd__tags_button-active') !== null) {
            document.querySelector('.bd__tags_button-active').classList.remove('bd__tags_button-active');
        }
        const divButton = e.target.closest('.bd__tags_button');
        divButton.classList.add('bd__tags_button-active');
    },
    filters(e) {
        this.sortedArray = this.articles.filter(article => article.id === e.target.dataset.id);
    }
  },  
}
    
</script>

<style scoped>

</style>