<template>

 <div class="container mt-3 fs-5">

    <div>Screensize {{ screenSize }} {{ currentBreakPoint }} </div>

 </div> 

</template>




<script>


import { computed, ref } from 'vue';


export default {

  name: 'browser-info',
 
  setup() {

        const screenSize = ref(window.innerWidth);  
  
        const currentBreakPoint = computed(() => {

            let bootstrapBreakpoint;

            switch (true) {

                case  (screenSize.value > 1400 ):
                    bootstrapBreakpoint = "No breakpoint invoked.";
                    break;
                case (screenSize.value > 1200):
                    bootstrapBreakpoint = "Currently at xxl breakpoint which starts at 1400px";
                    break;
                case (screenSize.value > 992):
                    bootstrapBreakpoint = "Currently at xl breakpoint which starts at 1200px";
                    break;
                case (screenSize.value > 768):
                    bootstrapBreakpoint = "Currently at lg breakpoint which starts at 992px";
                    break;
                case (screenSize.value > 576):
                    bootstrapBreakpoint = "Currently at md breakpoint which starts at 768px";
                    break;   
                case (screenSize.value > 0):
                    bootstrapBreakpoint = "Currently at sm breakpoint which starts at 576px";
                    break; 
                default:
                    bootstrapBreakpoint = "Currently at xs breakpoint which starts at 0px";

            } //switch

            return bootstrapBreakpoint;

        });

        return {screenSize, currentBreakPoint}
        


  },
  mounted() {
    //console.log("Layout component is mounted");
    console.log("this.$refs is",this.$refs);
   // window.addEventListener('resize',() => {console.log('screen size is ',window.innerWidth)});
   window.addEventListener('resize',() => { this.screenSize = window.innerWidth});
  } //mounted

}


</script>