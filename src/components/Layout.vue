<template>

    <div class="container text-end ">
      <div class="row">
        <div class="col border bg-info">
          Column 1
        </div>
        <div class="col border text-primary border-dark">
          Column 2
        </div>
        <div class="col border text-white bg-dark">
          Column 3
        </div>
      </div>
    </div>


    <div class="container text-end ">
      <div class="row">
        <div class="col-lg-4 border ">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-primary">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-white">
            .col-lg-4
        </div>
      </div>
    </div>

    <h2>Screensize {{ screenSize }}</h2>

</template>
  
    
    <script>
import { ref } from 'vue';



export default {
  name: 'Layout',
 
  setup() {

        const screenSize = ref(window.innerWidth);

        return {screenSize}
        


  },
  mounted() {
    console.log("Layout component is mounted");
    console.log("this.$refs is",this.$refs);
   // window.addEventListener('resize',() => {console.log('screen size is ',window.innerWidth)});
   window.addEventListener('resize',() => { this.screenSize = window.innerWidth});
  }

}

</script>