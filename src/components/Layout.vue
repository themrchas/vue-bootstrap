<template>

  <h4>Column and Row Examples</h4>

    <div class="container">
      <div class="text-start h5 ">
        Three div elements with 'col' class applied - &lt;div class&equals;"col border..."&gt;
      </div>
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


    <div class="container">
      <div class="row">
        <div class="col h5 text-start mt-3">
          Example showing responsive breakpoint. 
       </div>
       <div class="col-12 h6 text-start mt-1">
          Large breakpoint occurs by default when browser is less than 992px.
       </div>
      </div>
      <div class="row">
        <div class="col-lg-4 border ">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-primary">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-dark-emphasis">
            .col-lg-4
        </div>
      </div>
      <div class="row mt-1">
        Small breakpoint occurs by default when browser is less than 540px.
      </div>
      <div class="row">
        <div class="col-sm-4 border ">
          .col-sm-4
        </div>
        <div class="col-sm-4 border text-primary">
          .col-sm-4
        </div>
        <div class="col-sm-4 border text-dark-emphasis">
          .col-sm-4
        </div>
      </div>
    </div>

    

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