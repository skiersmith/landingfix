<template>
  <div class="outerDiv">
    <div class="header-container">

      <!-- <div><p>yo</p></div> -->
      <div class="header2-text">
        <transition name="fade">
          <h1 v-if="!scrolled">Welcome!</h1>
          <!-- <h1 v-if="scrolled4">Thank you for visiting.</h1> -->
        </transition>
      </div>
      <!-- <img src="../assets/rainbow.jpg" alt=""> -->
      <transition name="fade">
        <div v-if="scrolled" class="header-text">
          <h1>Hunter Smith</h1>
          <h4>Software Developer</h4>
          <h5>Boise, Id</h5>
        </div>
      </transition>

    </div>
    <div v-if="scrolled6" title="My Github" class="github">
      <a href="http://github.com/skiersmith" target="_blank">
        <img class="githubimg skill-image grow" src="../assets/GitHub-Mark.png" alt="github">
      </a>
    </div>
    <div class="projmain-container">
      <transition name="fade2">
        <div class="projBody" v-if="scrolled2">
          <h1>Projects</h1>
          <div class="skills-container">
            <!-- <div class="row"> -->
            <a href="https://jht-vue-kanban.herokuapp.com/#/" target="_blank">
              <div v-if="mobile === false" class=" skills grow">
                <img class="projPhoto" src="../assets/photo.png" alt="placeholder">
                <h6 class="proj-title text-center">Kanban Board</h6>
              </div>
              <div v-else>
                <h6 class="proj-title text-center">Kanban Board</h6>
              </div>
            </a>
            <a href="#">
              <div v-if="mobile === false" class="skills grow">
                <img src="http://placehold.it//150x150" alt="placeholder">
                <h6 class="proj-title text-center">Custom App for Transportation Complience Service</h6>
              </div>
              <div v-else>
                <h6 class="proj-title text-center">Custom App for Transportation Complience Service</h6>
              </div>
            </a>
            <a href="#">
              <div v-if="mobile === false" class="skills grow">
                <img src="http://placehold.it//150x150" alt="placeholder">
                <h6 class="proj-title text-center">Castle Grimtol Console Game</h6>
              </div>
              <div v-else>
                <h6 class="proj-title text-center">Castle Grimtol Console Game</h6>
              </div>
            </a>
          </div>
          <div class="skills-container">
            <a href="#">
              <div v-if="mobile === false" class="skills grow">
                <img src="http://placehold.it//150x150" alt="placeholder">
                <h6 class="proj-title text-center">Inventory Organizer</h6>
              </div>
              <div v-else></div>
            </a>
            <a href="#">
              <div v-if="mobile === false" class="skills grow">
                <img src="http://placehold.it//150x150" alt="placeholder">
                <h6 class="proj-title text-center">Project Title</h6>
              </div>
              <div v-else></div>
            </a>
            <a href="#">
              <div v-if="mobile === false" class="skills grow">
                <img src="http://placehold.it//150x150" alt="placeholder">
                <h6 class="proj-title text-center">Project Title</h6>
              </div>
              <div v-else></div>
            </a>
            <!-- </div> -->
          </div>
        </div>
      </transition>
    </div>
    
      <div class="skillsmain-container">
        <div v-if="" class="container box three h-center">
          <!-- <transition name="fade">
          </transition> -->
          <div class="skills-container">
            <transition-group name="fade">
              <h1 class="sTitle" key="05" v-if="scrolled3">Skills</h1>
              <div title="VueJS" v-if="scrolledI.scrolledI1" class="inline margin05" key="1">
                <img class="grow2 skill-image2" src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/53/Vue.js_Logo.svg/1000px-Vue.js_Logo.svg.png"
                  alt="">
              </div>
              <div title="HTML" v-if="scrolledI.scrolledI2" class="inline margin05" key="2">
                <img class="grow skill-image" src="https://www.w3.org/html/logo/downloads/HTML5_Logo_512.png" alt="html5 Logo">
              </div>
              <div title="CSS" v-if="scrolledI.scrolledI3" class="inline margin05" key="3">
                <img class="grow skill-image" src="http://w3widgets.com/responsive-slider/img/css3.png" alt="css3 Logo">
              </div>
              <div title="Javascript" v-if="scrolledI.scrolledI4" class="inline margin05" key="4">
                <img class="grow skill-image" src="https://seeklogo.com/images/J/javascript-logo-E967E87D74-seeklogo.com.png" alt="js5 Logo">
              </div>
              <div title="MySQL" v-if="scrolledI.scrolledI5" class="inline margin05" key="5">
                <img class="grow skill-image" src="https://www.mysql.com/common/logos/logo-mysql-170x115.png" alt="MySql Logo">
              </div>
              <div title=".NETCORE" v-if="scrolledI.scrolledI6" class="inline margin05" key="6">
                <img class="grow skill-image" src="https://developer.fedoraproject.org/static/logo/csharp.png"
                  alt="">
              </div>
              <div title="NodeJs" v-if="scrolledI.scrolledI7" class="inline margin05" key="7">
                <img class="grow skill-image" src="https://seeklogo.com/images/N/nodejs-logo-FBE122E377-seeklogo.com.png" alt="">
              </div>
              <div title="Bootstrap" v-if="scrolledI.scrolledI8" class="inline margin05" key="8">
                <img class="grow skill-image" src="https://logoepscdnphoto.b-cdn.net/wp-content/uploads/2016/12/bootstrap-logo.png" alt="Adobe PS Logo">
              </div>
              <div title="AdobePhotoshop" v-if="scrolledI.scrolledI9" class="inline margin05" key="9">
                <img class="grow skill-image" src="data:image/jpeg;base64,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"
                  alt="Adobe PS Logo">
              </div>
              <div title="AdobeIllustrator" v-if="scrolledI.scrolledI10" class="inline margin05" key="10">
                <img k class="grow skill-image" src="data:image/png;base64,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"
                  alt="Adobe PS Logo">
              </div>
            </transition-group>
          </div>
        </div>
     </div>

    <!-- <div class="pipe">

    </div> -->
  </div>
</template>

<script>
  export default {
    name: 'Home',
    data() {
      return {
        mobile: false,
        scrolled: false,
        scrolled2: false,
        scrolled3: false,
        scrolled4: false,
        scrolled5: false,
        scrolled6: false,
        hide: false,
        scrolledI: {
          scrolledI1: false,
          scrolledI2: false,
          scrolledI3: false,
          scrolledI4: false,
          scrolledI5: false,
          scrolledI6: false,
          scrolledI7: false,
          scrolledI8: false,
          scrolledI9: false,
          scrolledI10: false
        }
      }
    },
    methods: {
      enterEl(el, done) {
        //entrance animation
        done();
      },
      leaveEl(el, done) {
        //exit animation
        done();
      },
      topFunction() {
        document.body.scrollTop = 0; // For Safari
        document.documentElement.scrollTop = 0; // For Chrome, Firefox, IE and Opera
      },
      bottomFunction() {
        document.body.scrollTop = document.body.scrollHeight;
        document.documentElement.scrollTop = document.documentElement.scrollHeight
      },
      scrolled4Toggle() {
        console.log("yo")
        this.scrolled4 = true
      },
      handleScroll() {

        var isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent);
        if (isMobile) {

          this.scrolled6 = window.scrollY > 0
          this.scrolled4 = window.scrollY > 0;
          this.scrolled = window.scrollY > 50;

          this.scrolled3 = window.scrollY > 200 && window.scrollY < 700;
          this.scrolledI.scrolledI1 = window.scrollY > 820 && window.scrollY < 1600;
          this.scrolledI.scrolledI2 = window.scrollY > 850 && window.scrollY < 1600;
          this.scrolledI.scrolledI3 = window.scrollY > 880 && window.scrollY < 1600;
          this.scrolledI.scrolledI4 = window.scrollY > 910 && window.scrollY < 1600;
          this.scrolledI.scrolledI5 = window.scrollY > 940 && window.scrollY < 1600;
          this.scrolledI.scrolledI6 = window.scrollY > 970 && window.scrollY < 1600;
          this.scrolledI.scrolledI7 = window.scrollY > 1000 && window.scrollY < 1600;
          this.scrolledI.scrolledI8 = window.scrollY > 1030 && window.scrollY < 1600;
          this.scrolledI.scrolledI9 = window.scrollY > 1070 && window.scrollY < 1600;
          this.scrolledI.scrolledI10 = window.scrollY > 1100 && window.scrollY < 1600;
          this.scrolled2 = window.scrollY > 1600 && window.scrollY < 2450;
        }
        else {
          this.scrolled6 = window.scrollY > 0
          this.scrolled4 = window.scrollY > 0;
          this.scrolled = window.scrollY > 50;

          this.scrolled3 = window.scrollY > 200 && window.scrollY < 1000;
          this.scrolledI.scrolledI1 = window.scrollY > 520 && window.scrollY < 1200;
          this.scrolledI.scrolledI2 = window.scrollY > 550 && window.scrollY < 1200;
          this.scrolledI.scrolledI3 = window.scrollY > 580 && window.scrollY < 1200;
          this.scrolledI.scrolledI4 = window.scrollY > 610 && window.scrollY < 1200;
          this.scrolledI.scrolledI5 = window.scrollY > 640 && window.scrollY < 1200;
          this.scrolledI.scrolledI6 = window.scrollY > 670 && window.scrollY < 1200;
          this.scrolledI.scrolledI7 = window.scrollY > 700 && window.scrollY < 1200;
          this.scrolledI.scrolledI8 = window.scrollY > 730 && window.scrollY < 1200;
          this.scrolledI.scrolledI9 = window.scrollY > 770 && window.scrollY < 1200;
          this.scrolledI.scrolledI10 = window.scrollY > 800 && window.scrollY < 1200;
          this.scrolled2 = window.scrollY > 1750 && window.scrollY < 2600;
          if (window.scrollY > 3700) {
            // this.topFunction()
          }
        }
        // if (window.scrollY < 850) {
        //   this.scrolled2 = false

        // }
      }
    },
    mounted() {
      var isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent);
      if (isMobile) {
        console.log(this.mobile)
        this.mobile = true
      }
    },
    created() {
      window.addEventListener('scroll', this.handleScroll);
    },
    destroyed() {
      window.removeEventListener('scroll', this.handleScroll);
    }
    // computed: {

    //   myScrollFunc() {
    //     // myID = document.getElementById("myID");
    //     var y = window.scrollY;
    //     if (y >= 50) {
    //       this.show11 = true
    //     } else {
    //       this.show11 = false
    //     }
    //   }
    // },

  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  h1,
  h2 {
    font-weight: normal;
  }
  /* .sTitle{
    display: inline;
  } */
  .outerDiv {
    /* position: relative;
    top: -5rem; */
    display: grid;
    grid-template-columns: repeat(4, f1);
    grid-auto-rows: minmax(100vh, auto);
    grid-template-areas: "header header header header"". main1 main1 ."". main main . "". . . ."" . . . . "". main3 main3 .";
    grid-gap: 10rem
  }

  .header-container {
    color: black;
    background-image: url("../assets/Artboard5.jpg");
    background-size: 100%;

    background-repeat: no-repeat;
    grid-column-start: 1;
    grid-column-end: 5;
    grid-row-start: 1;
    grid-row-end: 2;
    /* align-content: center; */
    /* justify-content: center; */
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
    grid-template-rows: 1fr 1fr 1fr;
    /* margin-bottom: 10rem; */
  }

  .header2-text {
    grid-column-start: 2;
    grid-row-start: 1;
    grid-column-end: 2;
    grid-row-end: 1;
    display: grid;
    grid-template-rows: 1fr 1fr 1fr;
  }

  .header2-text>h1 {
    grid-row-start: 2;
  }

  .header-text {
    position: sticky;
    top: 5rem;
    grid-column-start: 2;
    grid-row-start: 2;
    grid-column-end: 2;
    grid-row-end: 2;
  }

  .projmain-container {
    grid-area: main;
  }

  .skillsmain-container {

    grid-area: main1;
  }

  .projBody {

    /* background-color: rgb(177, 71, 71); */
    /* width: 100vw; */
  }

  /* .header2-container{
    display: grid;
    grid-template-columns: repeat(3, f1);
    grid-template-rows: repeat(3, f1);
  } */

  .header-container>div {
    /* display: inline;
    grid-column-start: 2;
    grid-row-start: 2;
    grid-column-end: 2;
    grid-row-end: 2; */
  }

  .pipe {
    grid-area: main3;
    background-image: url("https://vignette.wikia.nocookie.net/fantendo/images/4/41/Green_Warp_Pipe_NSMBU.png/revision/latest?cb=20121214214119");
    background-repeat: no-repeat;
  }

  .github {
    position: fixed;
    top: 5px;
    right: 5px;
  }

  .skill-image {
    height: 100px;
    margin: 1rem;
    transform: scale(0.9)
  }

  .grow:hover {
    transform: scale(1.1);
  }

  .rainImg {
    width: 100vw;
  }

  /* .skillsmain-container{
    justify-content: center
  } */

  .outDiv {
    position: absolute;
    top: 0;
  }



  .margin05 {
    margin-left: 1rem;
    margin-right: 1rem
  }

  .inline {
    display: inline;
  }

  .skills-container {
    color: rgb(0, 3, 2);
    display: flex;
    justify-content: center;
    /* background-color: rgba(84, 148, 108, 0.171); */
    /* background-size: 100%; */
    /* border-color: rgba(0, 0, 0, 0.534);
    border-width: 1px;
    border-style: dotted; */
    border-radius: 50px;

  }

  .bgImg {
    /* background-image: url("../assets/Artboard5.jpg"); */
    /* background-size: 100%; */
    /* background-repeat: no-repeat; */
  }

  .section1 {
    height: 100rem
  }

  .section2 {
    height: 120rem;
    /* background-image: url("../assets/Artboard.jpg"); */
    background-size: 100%;
  }

  .section3 {
    height: 50rem;
  }

  .margin-b {
    margin-bottom: 20rem;
  }

  .head-text {
    color: white;
    position: sticky;
    top: 40rem;
  }

  .fade-enter-active,
  .fade-leave-active {
    transition: opacity .5s ease-out;
  }

  .fade-enter,
  .fade-leave-to {
    opacity: 0;
  }

  .fade2-enter-active,
  .fade2-leave-active {
    transition: opacity 2s ease-out;
  }

  .fade2-enter,
  .fade2-leave-to {
    opacity: 0;
  }


  h1,
  h2 {
    font-weight: normal;
  }

  ul {
    list-style-type: none;
    padding: 0;
  }

  li {
    display: inline-block;
    margin: 0 10px;
  }

  a {
    color: #42b983;
  }



  .grow:hover {
    transform: scale(1.1);
  }

  .grow2 {
    transition: all .2s ease-in-out;
  }

  .grow2:hover {
    transform: scale(1.6);
  }

  .skills {
    height: 20rem;
    margin: 1rem;
  }

  .landHead {
    margin: 4rem;
    height: 50vh;
    /* background-color: #9fc7b557; */
    width: 100vw;
  }

  .skill-image2 {
    height: 100px;
    margin: 1rem;
    transform: scale(1.4)
  }

  .spacer {
    height: 20rem;
  }

  .spacer3 {
    height: 12rem;
  }

  .spacer2 {
    height: 30rem;
  }

  .projPhoto {
    width: 250px;
  }

  .landFoot {
    height: 20vh;
    background-color: rgba(119, 136, 153, 0.479);
    width: 100vw;

  }



  /* always present */

  .expand-transition {
    transition: all .3s ease;
    height: 30px;
    padding: 10px;
    background-color: #eee;
    overflow: hidden;
  }

  /* .expand-enter defines the starting state for entering */

  /* .expand-leave defines the ending state for leaving */

  .expand-enter,
  .expand-leave {
    height: 0;
    padding: 0 10px;
    opacity: 0;
  }

  .meImg {
    max-width: 25vw;
    height: auto;
    /* padding: 3rem; */
  }

  .text-container {
    display: inline;
    /* justify-content: space-around; */
    /* align-content: center; */
    /* background-color: rgba(255, 255, 255, 0.432); */
    position: relative;
    top: 15rem;
    left: 35vw;
    /* width: 100rem; */
    border-radius: 10px;


  }
</style>