<script>
  export default {
    name: "AppFooter",
    data() {
      return {
        footerLinkLists: [
        {
          title: "DC COMICS",
          links: [
            'Characters', 'Comics', 'Movies', 'TV', 'Games', 'Videos', 'News'
          ],
        },
        {
          title: "SHOP",
          links: [
            'Shop DC', 'Shop DC Collectibles'
          ],
        },
        {
          title: "DC",
          links: [
            'Terms of Use', 'Privacy Policy', 'Ad Choices', 'Advertising', 'Jobs', 'Talent Workshop', 'Subscriptions', 'CPSC Certificates', 'Ratings', 'Shop Help', 'Contact Us'
          ],
        },
        {
          title: "SITES",
          links: [
            'DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'
          ]
        },
      ],
      }
    },
  }
</script>

<template>
  <footer>
    <div class="container">

      <div id="footer-links">

        <div v-for="footerLinkList in footerLinkLists " class="footer-link">
          <div class="title">{{ footerLinkList.title }}</div>
          <ul class="links">
            <li v-for="link in footerLinkList.links" class="link">{{link}}</li>
          </ul>
        </div>

        

      </div>

    </div>
    
    <div id="dc-logo-bg">
      <img src="/img/dc-logo-bg.png" alt="">
    </div>

  </footer>

  <!-- sign-up-now -->
  <div id="sign-up-now">
    
    <div id="flex-sign-up" class="container">

        
            <button id="btn-sign">SIGN-UP-NOW!</button>


        

        <div id="flex-left-social">
            <H3 style="color: #0282f9;"> FOLLOW US</H3>
            <div id="img-container-social">
                <img src="/public/img/footer-facebook.png" alt="">
                <img src="/public/img/footer-twitter.png" alt="">
                <img src="/public/img/footer-youtube.png" alt="">
                <img src="/public/img/footer-pinterest.png" alt="">
                <img src="/public/img/footer-periscope.png" alt="">
            </div>    

        </div>



    </div>




  </div>

<!-- fine sign-up-now  -->
</template>

<style lang="scss" scoped>
// footer links
footer {
  position: relative;
  overflow-y: hidden;
  background-image: url('/img/footer-bg.jpg');
  background-size: cover;
  background-position: center;
  #footer-links {
    display: flex;
    flex-flow: column wrap;
    justify-content: flex-start;
    align-items: flex-start;
    align-content: flex-start;
    gap: 30px;
    position: relative;
    height: 400px;
    padding: 40px 0;
    z-index: 1;
    .footer-link  {
      width: 200px;
      .title {
        font-size: 1.2em;
        font-weight: bold;
        text-transform: uppercase;
      }
      .link {
        color: gray;
        font-size: .8em;
      }
    }
  }
  ul {
    list-style-type: none;
  }
  #dc-logo-bg {
    position: absolute;
    right: 100px;
    top: 50%;
    transform: translateY(-50%);
    z-index: 0;
  }
}
  // fine footer links
#sign-up-now{
    background-color: #30303030;



}

#flex-sign-up {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 40px 0;

}

#flex-left-social{
    display: flex;
    gap: 30px;
    align-items: center;

}

#img-container-social{
    display: flex;
    gap: 20px;



}

#btn-sign{
    background-color: #30303030;
    color: white;
    padding: 20px;
    border-color: #0282f9;

}


</style>