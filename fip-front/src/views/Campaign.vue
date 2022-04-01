<template>
<Header />
  <div class="weTogether">
    <div class="campaign_promo" :style="campaign_promo">
      <div class="campaign_text">
       <h3>Join our #weTogether</h3>
       <p><b>Be with MSF with a simple donation method.</b></p>
       </div>
    </div>

    <div class="campaign_info">
        <div>
        <h3>WHAT IS THIS CAMPAIGN?</h3>
        <p>The inspiration of this campaign and surprise boxses design was produced
             from the interviews and photos from actual volunteers working place.
              We want to show how easy be part of MSF and help people. <br><br>
            Instead of casting famous designers, we pick freelance designers and
             entry-level designers who work in difficult environments and give them
              more opportunity to be a part of meaningful project and get a professinal
               experience.<br><br>Thanks to our partners who help us with this campaign.</p>
        </div>
        <div class="tagline">
            <img src="@/assets/images/tagline.png" alt="tagline">
            <p><b>Our partners:</b></p>
            <div class="partners">
                <img src="@/assets/images/cola.svg" alt="cola">
                <img src="@/assets/images/samsung.svg" alt="samsung">
                <img src="@/assets/images/canada.svg" alt="canada">
            </div>
        </div>
    </div>

    <div>
        <h3>HOW CAN I PARTICIPATE THIS</h3>
        <div class="activity">
            <h4>ACTIVITY 1</h4>
            <h4>MEET MSF AT THE SUBWAY STATION AND BUS STOP!</h4>
            <div class="step">
                <h4>STEP 1</h4>
                <p>On your way to work or school, look around subway
                     station and bus stops carefully and find some MSF posters.</p>
            </div>
            <div class="slider">
                <div class="item">
                   <img src="@/assets/images/art_gallery1.jpg" alt="art gallery">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/art_gallery1.jpg" alt="art gallery">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/art_gallery1.jpg" alt="art gallery">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/art_gallery1.jpg" alt="art gallery">
                 </div>
                 <a class="previous" onclick="previousSlide()">&#10094;</a>
                 <a class="next" onclick="nextSlide()">&#10095;</a>
            </div>

            <div class="step">
                <h4>STEP 2</h4>
                <p>Take a picture with a poster or scan a QR code on
                   the posters using your camera.</p>
            </div>
            <div class="slider">
                <div class="item">
                   <img src="@/assets/images/wall_posters.jpg" alt="wall posters">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/qr.jpg" alt="QR">
                 </div>
                 <a class="previous" onclick="previousSlide()">&#10094;</a>
                 <a class="next" onclick="nextSlide()">&#10095;</a>
            </div>

            <div class="step">
                <h4>STEP 3</h4>
                <p>Upload your photo to social media account with #weTogether hashtag.
                   $1.00 will be automatically donated per post. Free to share with
                    your friends.</p>
            </div>
            <div class="slider">
                <div class="item">
                   <img src="@/assets/images/insta_profile.jpg" alt="insta profile">
                   <img src="@/assets/images/insta_art_gallery1.jpg" alt="art gallery insta">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/Facebook.jpg" alt="Facebook">
                   <img src="@/assets/images/instagram-boxes.jpg" alt="Facebook">
                 </div>
            </div>

            <div class="step">
                <h4>STEP 4</h4>
                <p>Please follow our MSF official accounts. If you order our
                   $50 Limited Edition Surprise Boxes with random items from $1 to $2000,
                    you automatically become a donator. Proceeds from the sale of surprise
                     boxes will go to help COVID victims.</p>
            </div>
            <div class="slider">
                <div class="item">
                   <img src="@/assets/images/insta_profile.jpg" alt="insta profile">
                 </div>
                 <div class="item">
                   <img src="@/assets/images/Facebook.jpg" alt="Facebook">
                 </div>
            </div>
        </div>

        <div class="activity">
          <h4>ACTIVITY 2</h4>
          <h4>SURPRISE BOX</h4>
          <div class="box">
            <img src="@/assets/images/box_mockup.jpg" alt="box">
            <div class="plans">
              <div class="monthly_plan">
                <h5>MONTHLY PLAN</h5>
                <b>$2.99</b>
                <p>Free shipping <br>Free personalize Initial</p>
                <h5>BUY NOW</h5>
              </div>

              <div class="once_plan">
                <h5>ONCE PLAN</h5>
                <b>$3.99</b>
                <p>Random promo coupons with partnership companies</p>
                <h5>BUY NOW</h5>
              </div>

            </div>
          </div>
          <p>Surprise boxes with random items from $1 to $2000 range of worth.
             One of the best items is a new model of Samsung phone, galaxy buds,
              power banks and Coca-Cola lottery for 1 year. Our customers can order
               an engraving of their name or initials. The campaign's revenue will be
                used to help vulnerable people around the world in need.</p>
        </div>

        <div class="campaign_video">
          <h4>PROMOTIONAL VIDEO</h4>
          <video id="videoPromo" src="@/assets/images/fip_video.mp4" controls="controls">
          </video>
          <b>“We don’t need any borders to save lives. Use the easiest way to donate for
             needed people.”</b>
        </div>
    </div>
  </div>
<Footer />
</template>

<script>
// @ is an alias to /src
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';

export default {
  name: 'Campaignt',
  components: {
    Header,
    Footer,
  },

  data() {
    return {
      campaign_promo: { backgroundImage: 'url(https://i.ibb.co/fDh9TKn/wall-posters.jpg)' },
    };
  },
};
</script>

<style lang="scss">
 @import "src/assets/sass/main.scss";
</style>
