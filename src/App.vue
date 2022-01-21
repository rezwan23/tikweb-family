<template>
  <div>
    <h1 style="text-align:center" class="shake display_none">Rocking Works from Some Rocking Persons.</h1>
    <div class="play_btn" @click="init">
      <img src="dist/images/play.png" class="animate__animated animate__zoomInDown" alt />
    </div>
    <div class="container display_none shake">
      <div class="c1 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__backInDown">Ashraful Shohag</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/ashrafulshohag.jpg" class="animate__backInUp" alt />
        </div>
      </div>
      <div class="c2 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/brishtisarker.jpg" class="animate__backInLeft" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__backInRight">Brishti Sarker</h1>
        </div>
      </div>
      <div class="c3 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__bounceIn">Tahmina Sultana Shinti</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/tahminasultanashinti.jpg" class="animate__bounceInUp" alt />
        </div>
      </div>
      <div class="c4 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/marzaan.jpg" class="animate__bounceInLeft" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__bounceInRight">Mar Zaan</h1>
        </div>
      </div>
      <div class="c5 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__flipInX">Tahomina Jahan</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/tahominajahan.jpg" class="animate__flipInY" alt />
        </div>
      </div>
      <div class="c6 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/fazlulpalash.jpg" class="animate__lightSpeedInLeft" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__lightSpeedInLeft">Fazlul Palash Sir</h1>
        </div>
      </div>
      <div class="c7 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__rotateInDownLeft">Tania Afrin Risa</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/taniaafrinrisa.jpg" class="animate__rotateInDownRight" alt />
        </div>
      </div>
      <div class="c8 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/mofazahmed.jpg" class="animate__slideInDown" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__slideInUp">Mofaz Ahmed</h1>
        </div>
      </div>
      <div class="c9 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__backInDown">NJ Ahnaaf</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/njahnaaf.jpg" class="animate__backInUp" alt />
        </div>
      </div>
      <div class="c10 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/abubakersiddique.jpg" class="animate__backInDown" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__backInUp">Abu Baker Siddique</h1>
        </div>
      </div>
      <div class="c11 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__backInLeft">Rayhan Hossen</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/rayhanhossen.jpg" class="animate__backInRight" alt />
        </div>
      </div>
      <div class="c12 component" style="width:100%;height:100%">
        <div class="left_col">
          <img src="dist/images/works/kabidhassan.jpg" class="animate__bounceInLeft" alt />
        </div>
        <div class="right_col">
          <h1 class="animate__bounceInRight">Kabid Hassan</h1>
        </div>
      </div>
      <div class="c13 component" style="width:100%;height:100%">
        <div class="left_col">
          <h1 class="animate__flipInX">Tanisa Mohona</h1>
        </div>
        <div class="right_col">
          <img src="dist/images/works/tanisamohona.jpg" class="animate__flipInY" alt />
        </div>
      </div>
      <div class="c14 component" style="width:100%;height:100%;text-align:center">
        <img src="dist/images/works/ghani.jpg" class="ghani animate__zoomIn" alt />
        <h1 style="margin-top:0px" class="fadeInLeft">Ghani Razwanul</h1>
        <h2 class="fadeInRight">github.com/rezwan23</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      audio: {},
      interval: 0,
      intervalObj: {},
      deviceWidth: 0
    };
  },
  methods: {
    magic() {
      if (this.interval >= 0 && this.interval < 5000) {
        this.animate1()
      } else if (this.interval >= 5000 && this.interval < 10000) {
        this.animate2()
      } else if (this.interval >= 10000 && this.interval < 15000) {
        this.animate3()
      } else if (this.interval >= 15000 && this.interval < 20000) {
        this.animate4()
      } else if (this.interval >= 20000 && this.interval < 25000) {
        this.animate5()
      } else if (this.interval >= 25000 && this.interval < 30000) {
        this.animate6()
      } else if (this.interval >= 30000 && this.interval < 35000) {
        this.animate7()
      } else if (this.interval >= 35000 && this.interval < 40000) {
        this.animate8()
      } else if (this.interval >= 40000 && this.interval < 45000) {
        this.animate9()
      } else if (this.interval >= 45000 && this.interval < 50000) {
        this.animate10()
      } else if (this.interval >= 50000 && this.interval < 55000) {
        this.animate11()
      } else if (this.interval >= 55000 && this.interval < 60000) {
        this.animate12()
      } else if (this.interval >= 60000 && this.interval < 65000) {
        this.animate13()
      } else if (this.interval >= 65000 && this.interval < 70000) {
        this.animate14()
      }else{
        clearInterval(this.intervalObj)
      }
    },
    init() {
      if (this.deviceWidth < 1300) {
        alert(
          "Please View from a Wider Screen! May be You Are Watching from Mobile or Tablet"
        )
      } else {
        $(".play_btn").addClass("display_none")
        $(".container").removeClass("display_none")
        $("h1.shake").removeClass("display_none")
        this.audio.play()
        const self = this
        self.magic()
        this.intervalObj = setInterval(function() {
          self.magic()
        }, 5000)
      }
    },
    animate1() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c1 .right_col img").addClass("animate__animated")
      $(".component.c1 .left_col h1").addClass("animate__animated")
      $(".component.c1").removeClass("display_none")
      this.interval += 5000;
    },
    animate2() {
      $(".container").css("background", "#37373D")
      $(".component").addClass("display_none")
      $(".component.c2 .left_col img").addClass("animate__animated")
      $(".component.c2 .right_col h1").addClass("animate__animated")
      $(".component.c2").removeClass("display_none")
      this.interval += 5000;
    },
    animate3() {
      $(".container").css("background", "#C49166")
      $(".component").addClass("display_none")
      $(".component.c3 .right_col img").addClass("animate__animated")
      $(".component.c3 .left_col h1").addClass("animate__animated")
      $(".component.c3").removeClass("display_none")
      this.interval += 5000;
    },
    animate4() {
      $(".container").css("background", "#451B59")
      $(".component").addClass("display_none")
      $(".component.c4 .left_col img").addClass("animate__animated")
      $(".component.c4 .right_col h1").addClass("animate__animated")
      $(".component.c4").removeClass("display_none")
      this.interval += 5000;
    },
    animate5() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c5 img").addClass("animate__animated")
      $(".component.c5 h1").addClass("animate__animated")
      $(".component.c5").removeClass("display_none")
      this.interval += 5000;
    },
    animate6() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c6 img").addClass("animate__animated")
      $(".component.c6 h1").addClass("animate__animated")
      $(".component.c6").removeClass("display_none")
      this.interval += 5000;
    },
    animate7() {
      $(".container").css("background", "#451B59")
      $(".component").addClass("display_none")
      $(".component.c7 img").addClass("animate__animated")
      $(".component.c7 h1").addClass("animate__animated")
      $(".component.c7").removeClass("display_none")
      this.interval += 5000;
    },
    animate8() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c8 img").addClass("animate__animated")
      $(".component.c8 h1").addClass("animate__animated")
      $(".component.c8").removeClass("display_none")
      this.interval += 5000;
    },
    animate9() {
      $(".container").css("background", "#451B59")
      $(".component").addClass("display_none")
      $(".component.c9 img").addClass("animate__animated")
      $(".component.c9 h1").addClass("animate__animated")
      $(".component.c9").removeClass("display_none")
      this.interval += 5000;
    },
    animate10() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c10 img").addClass("animate__animated")
      $(".component.c10 h1").addClass("animate__animated")
      $(".component.c10").removeClass("display_none")
      this.interval += 5000;
    },
    animate11() {
      $(".container").css("background", "#451B59")
      $(".component").addClass("display_none")
      $(".component.c11 img").addClass("animate__animated")
      $(".component.c11 h1").addClass("animate__animated")
      $(".component.c11").removeClass("display_none")
      this.interval += 5000;
    },
    animate12() {
      $(".container").css("background", "#fff293")
      $(".component").addClass("display_none")
      $(".component.c12 img").addClass("animate__animated")
      $(".component.c12 h1").addClass("animate__animated")
      $(".component.c12").removeClass("display_none")
      this.interval += 5000;
    },
    animate13() {
      $(".container").css("background", "#451B59")
      $(".component").addClass("display_none")
      $(".component.c13 img").addClass("animate__animated")
      $(".component.c13 h1").addClass("animate__animated")
      $(".component.c13").removeClass("display_none")
      this.interval += 5000;
    },
    animate14() {
      $(".container").css("background", "#fff293")
      $(".container.shake").removeClass("shake")
      $("h1.shake").text("Created By..")
      $(".component").addClass("display_none")
      $(".component.c14 img").addClass("animate__animated")
      $(".component.c14 img").addClass("animate__slower")
      $(".component.c14 h1").addClass("animate__animated")
      $(".component.c14 h2").addClass("animate__animated")
      $(".component.c14").removeClass("display_none")
      this.interval += 5000;
    }
  },
  mounted() {
    let sound = new Audio()
    sound.src = "dist/audio/music1.mp3";
    this.audio = sound;
    this.deviceWidth = window.innerWidth;
  }
};
</script>
