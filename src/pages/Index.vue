<template>
  <q-page class="">
    <div class="col header text-center">
      <!-- <img src="assets/Music.jpg" width="200"> -->
      <h1 class="heading text-center">Welcome to online music store <q-icon name="music_note"></q-icon></h1><br>
      <q-btn unelevated rounded size="28px" color="secondary" label="See our Products" to="/Product"/>
    </div>
    <div class="">
      <div class="row section">
        <div class="col-12 col-md">
          <h3 class="text-center q-px-sm">Our Available Product</h3>
          <h6 class="text-center">Trust Me it will make u satified</h6>
        </div>
        <div class="col-12 col-md basket">
          <h1 class="text-center"><q-icon name="shopping_basket"></q-icon></h1>
        </div>
      </div>
      <q-separator class="line" />
      <!-- <p v-for="person in persons" :key="person">{{ person }}</p> -->
      <div class="row main">
        <div class="col-auto satu">
          <h4>Guitar</h4>
          <h6 class="text-justify">Gitar adalah sebuah alat musik berdawai yang dimainkan dengan cara dipetik, umumnya menggunakan jari maupun plektrum. Gitar terbentuk atas sebuah bagian tubuh pokok dengan bagian leher yang padat sebagai tempat senar yang umumnya berjumlah enam didempetkan. </h6>
        </div>
        <div class="col-auto satu">
         <h4 text-justify>Piano</h4>
         <h6 class="text-justify">Piano (yang juga disebut pianoforte) adalah instrumen musik yang diklasifikasikan sebagai instrumen perkusi yang dimainkan dengan menekan tuts – tuts pada piano.
           Setiap tuts tersambung ke hammer yang ada di dalam piano dan menekan senar di dalamnya
         </h6>
        </div>
        <div class="col-auto satu">
         <h4 text-justify>Drum</h4>
         <h6 class="text-justify">Piano (yang juga disebut pianoforte) adalah instrumen musik yang diklasifikasikan sebagai instrumen perkusi yang dimainkan dengan menekan tuts – tuts pada piano.
           Setiap tuts tersambung ke hammer yang ada di dalam piano dan menekan senar di dalamnya
         </h6>
        </div>
        <div class="col-auto satu">
         <h4 text-justify>Biola</h4>
         <h6 class="text-justify">Piano (yang juga disebut pianoforte) adalah instrumen musik yang diklasifikasikan sebagai instrumen perkusi yang dimainkan dengan menekan tuts – tuts pada piano.
           Setiap tuts tersambung ke hammer yang ada di dalam piano dan menekan senar di dalamnya
         </h6>
        </div>
      </div><br>
    </div>
  </q-page>
</template>

<script>
// import Test from 'Test.vue'
export default {
  data () {
    return {
      persons: ['jhon', 'cenna']
    }
  }
  // components: {
  //   'test': Test
  // }
}
</script>

<style scoped>
  .header {
    background-image:url('/statics/Music.jpg');
    padding: 80px;
    background-size: cover;
    background-position: right top;
  }
  .satu {
    /* border: 1px solid lightgray; */
    padding: 20px;
  }
  .basket {
    padding-top:50px;
  }
  .line {
    width: 30%;
    margin: auto;
    background-color: salmon;
    height: 3px;
  }
  h3 {
    padding: 30px;
    text-shadow: gray 2px 2px 4px;
  }
  h4 {
    padding: 10px;
    width: 70%;
    margin: auto;
  }
  .main {
    padding-top: 40px;
  }
  .section {
    /* border: 1px solid lightgray; */
    padding-bottom: 40px;
  }
  h6 {
    color: gray;
    font-weight: normal;
    padding: 20px;
    width: 70%;
    margin: auto;
  }
  h4 {
    letter-spacing: 2px;
  }
  h1 {
    color: sandybrown;
    letter-spacing: 2px;
    font-weight: bold;
    padding: 20px;
    margin: 10px auto;
    font-size: 65px;
  }
  @media (min-width: 768px) and (max-width: 1024px) {
     h1 {
      font-size: 55px;
    }
    h3 {
      font-size: 40px;
    }
  }

  @media (min-width: 451px) and (max-width: 767px) {
    h1 {
      font-size: 55px;
    }
    h3 {
      font-size: 45px;
    }
    .basket {
    padding-top:20px;
  }
  }
</style>
