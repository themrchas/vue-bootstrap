<template>

  <div class="h3 mt-2">Column and Row Examples</div>

    <div class="container">
      <div class="row">
        <div class="col text-start h5">
        Three div elements with 'col' class applied - &lt;div class&equals;container&gt;&lt;div class&equals;"col border..."&gt;.
        <br/>Note that using the .container class will make container responsive but the columns are set to be non-responsive and equal in width.
        </div>
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
          Example showing responsive breakpoint using .container class. The .container class is responsive and columns are set be responsive at lg and sm breakpoints respectively.
       </div>
       <div class="col-12 h6 text-start mt-1">
          Large breakpoint occurs by default when browser is less than 992px.
       </div>
      </div>
      <div class="row">
        <div class="col-lg-4 border bg-warning-subtle">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-primary bg-warning-subtle">
          .col-lg-4
        </div>
        <div class="col-lg-4 border text-dark-emphasis bg-warning-subtle">
            .col-lg-4
        </div>
      </div>
      <div class="row mt-1">
        Small breakpoint occurs by default when browser is less than 576px.
      </div>
      <div class="row">
        <div class="col-sm-4 border border-dark-subtle bg-secondary-subtle">
          .col-sm-4
        </div>
        <div class="col-sm-4 border border-dark-subtle text-primary bg-secondary-subtle">
          .col-sm-4
        </div>
        <div class="col-sm-4 border border-dark-subtle text-dark-emphasis bg-secondary-subtle">
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