<template>
  <v-app id="Home">
    <NavBar />
    <v-container fluid>
      <div class="head">
            <v-row>
              <v-col cols="5">
                <div style="position: relative" class="mt-16">
                <h1 class="text-grey">Hello,</h1>
                <h1 class="text-grey">I'm Dicky Iswandy</h1>
                <span class="text-grey">Mahasiswa Teknik Informatika</span><br />
                <v-btn tile dark class="text-yellow mt-8" variant="outlined">Contact Me</v-btn>
              </div>
              </v-col>
              <v-col cols="2">
                <div style="position: absolute;z-index: 9999;bottom:0;margin-left: auto;margin-right: auto;left: 0;right: 0;text-align: center;">
                    <v-icon>fas fa-angle-double-down</v-icon>
                </div>
              </v-col>
              <v-col cols="5">
                <div style="position: relative;z-index: 9999;" class="mt-16">
                  <v-img src="fotosaya.png" contain max-height="300"></v-img>
                </div>
              </v-col>
            </v-row>
      </div>
      <v.col cols="12" class="mt-16" id="about">
        <div>
          <v-row>
            <v-col cols="12" sm="6">
              <div class="egg">
                <v-img src="part3.png" max-height="400"></v-img>
              </div>
            </v-col>
            <v-col  cols="12" sm="6">
              <h5 class="mt-16">About Me</h5>
              <div style="width: 120px;">
              <v-slider v-model="slider2" color="yellow"

              </v-slider>
            </div>
            <h4 class="mt-n4">I am an informatics engineering student</h4>
            <p class="text-grey">I am a student at Islamic University of Riau, Faculty of Engineering, majoring in Informatics Engineering. 
              I am currently in my fourth semester. 
              I was born on April 2, 2004. I have three siblings and I am the eldest. 
              The reason I chose this major is because it offers vast opportunities in computer programming, software development, information security analysis, data analysis, database design and maintenance, up to IT consultancy. 
              Furthermore, I also find informatics engineering fascinating and enjoyable because it deals with computers, code, logical software, hardware, and everything related to technology.
            </p>
            <br />
            <p class="text-grey">
              My experience when I was active in the scouts, I often participated in various competitions. 
              One of them was when we competed in a camping competition. 
              We had to demonstrate survival skills in nature, such as making fire and navigating difficult terrain. 
              Despite fierce competition, our team managed to win several categories.
            </p>
            <br />
            <p class="text-grey">
              My experience participating in the school marching band was incredible. 
              I had the opportunity to learn and perform music alongside my peers. 
              We spent countless hours practicing formations, perfecting our technique, and synchronizing our movements to create captivating performances during school events and competitions. 
              Being part of the marching band not only improved my musical skills but also taught me the value of teamwork, discipline, and dedication.
              </p>
              <v-btn tile dark color="yellow" class="mt-4">
                Download Resume 
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v.col>
      <div class="text-center mr-4">
        <h2>Hobby</h2>
        <div style="width:120px; margin: 0 auto">
          <v-slider v-model="slider2" color="yellow"></v-slider>
        </div>
      </div>
      <v-col cols="12" class="padd" id="portfolio">
        <div class="first" id="project">
          <v-row>
            <v-col cols="12">
              <div class="child">
                <v-btn icon="fas fa-laptop" color="#FBDF7E" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Bermain Game</h3>
                <v-img src="valorant.png" max-height="400"></v-img>
              </div>
              <div class="child">
                <v-btn icon="fas fa-mobile-alt" color="#FBDF7E" class="text-white"></v-btn>
                <h3 class="ml-3 mt-4">Badminton</h3>
                <v-img src="badminton.png" max-height="550"></v-img>
              </div>
            </v-col>
          </v-row>
          <v-divider></v-divider>
        </div>
      </v-col>
      <v-col cols="12" sm="12" class="px-16" id="Contact">
        <v-row>
          <v-col cols="12" sm="4">
            <div class="child">
              <h1>Contact Info.</h1>
              <v-btn icon="fas fa-map-marker-alt" class="mt-10" variant="outlined"></v-btn><br />
              <span class="text-caption">Jl.Karya, Marpoyan, Pekanbaru, Indonesia</span> <br />
              <v-btn icon="fas fa-phone-alt" class="mt-10" variant="outlined"></v-btn><br/>
              <span class="text-caption">0895-6184-38875</span> <br />
              <v-btn icon="fas fa-envelope" class="mt-10" variant="outlined"></v-btn><br/>
              <span class="text-caption">dickyiswandy@student.uir.ac.id </span> <br />
            </div>
          </v-col>
        </v-row>
      </v-col>
    </v-container>
    <FooterView />
  </v-app>
  <v-footer>
        <v-card elevation="0" rounded="0" width="100%" class="bg-grey text-center">
            <v-card-text>
                <v-btn class="mw-4" icon="fas fa-comment" variant="plain" color="white"></v-btn>
                <v-btn
                class="mx-4"
                icon="fas fa-university"
                variant="plain"
                color="white"
            ></v-btn>
            <v-btn
                class="mx-4"
                icon="fas fa-wifi"
                variant="plain"
                color="white"
            ></v-btn>
            <v-btn
                class="mx-4"
                icon="fas fa-podcast"
                variant="plain"
                color="white"
            ></v-btn>
            </v-card-text>
            <v-card-text class="text-white">
                    @{{ new Date().getFullYear() }}
                    <strong>CopyRight by Dicky Iswandy</strong>
            </v-card-text>
        </v-card>
    </v-footer>
</template>

<script>
import { defineComponent } from 'vue';

// Components
import NavBar from '@/components/NavBar.vue';

export default defineComponent({
  name: 'HomeView',
  setup(){
    return {
      slider2: 50,

items: [
  {
    img: "2.jpg",
  },
  {
    img: "part2.png",
  },
  {
    img: "part4.jpg",
  },
  {
    img: "part5.jpg",
  },
  {
    img: "part6.jpg",
  },
  {
    img: "part7.jpg",
  },
],        
    } 
  },

  components: {
   
    NavBar
  },
});
</script>
<style scoped>
.v-container{
  padding: 16px 0;
}
.head {
  position: relative;
  text-align: center;
  padding:12px;
  margin-bottom: 6px;
  height:400px;
  width: 100%;
  color: white;
}
.head::before {
  content: " ";
  position: absolute;
  top:0;
  left: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, 6deg);
}
.head::after {
  content: " ";
  position: absolute;
  top:0;
  right: 0;
  height: 100%;
  width: 50%;
  background: black;
  transform: skew(0deg, -6deg)
}
.egg{
  display: block;
  margin-left: 100px;
  margin-top: 50%;
  width: 360px;
  height: 400px;
  background-color: #FBDF7E;
  border-radius: 50% 50% 50% 50% / 60% 60% 40% 40%;
}
.first {
  width: 100%;
  height: 280;
  text-align: center;
  padding: 2rem 2rem;
}
.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: center;
  margin-right: 8px;
}
.imgHover {
  padding: 0 200px;
}
.pre {
  width: 100%;
  height: 300px;
  text-align: center;
  padding: 0 200px;
  background-color: #f5f5f5;
}
.hire {
  width: 100%;
  height: 200px;
  padding: 0 200px;
  background-color: #e9e9e9;
  margin-top: -24px;
}
.v-footer{
    padding: 8px 0 !important;
}
</style>
