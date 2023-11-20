<template>

    <h3 class="mt-3">Vertical column alignment within a container</h3>
    <div class="container mt-1.5">
        <div>align-items-start</div>
         <div class="row align-items-start border border-dark row-height">
            <div class="col border border-dark-subtle">Column 1</div>
            <div class="col border border-dark-subtle">Column 2</div>
            <div class="col border border-dark-subtle">Column 3</div>
        </div>
         <div>align-items-center</div>
         <div class="row align-items-center border border-dark row-height">
            <div class="col border border-dark-subtle">Column 1</div>
            <div class="col border border-dark-subtle">Column 2</div>
            <div class="col border border-dark-subtle">Column 3</div>
        </div>
        <div class="mt-1">align-items-end</div>
        <div class="row align-items-end border border-dark row-height mt-1">
            <div class="col border border-dark-subtle">Column 1</div>
            <div class="col border border-dark-subtle">Column 2</div>
            <div class="col border border-dark-subtle">Column 3</div>
        </div>
    </div>


    <h3 class="mt-3">Indivdual column alignment within a container</h3>
    <div class="container mt-1.5">
        <div>align-items-start</div>
         <div class="row border border-dark row-height">
            <div class="col border border-dark-subtle align-self-center">col1 align-self-center</div>
            <div class="col border border-dark-subtle align-self-start">col2 align-self-start</div>
            <div class="col border border-dark-subtle align-self-end">col3 align-self-end</div>
        </div>
    </div>

    <h3 class="mt-3">Horizontal column alignment </h3>
    <div class="container mt-1.5">
        <div>justify-content-start</div>
            <div class="row border border-dark flex-row-height justify-content-start">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
        <div>justify-content-center</div>
            <div class="row border border-dark flex-row-height justify-content-center">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
        <div>justify-content-end</div>
            <div class="row border border-dark flex-row-height justify-content-end">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
        <div>justify-content-around</div>
            <div class="row border border-dark flex-row-height justify-content-around">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
        <div>justify-content-between</div>
            <div class="row border border-dark flex-row-height justify-content-between">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
        <div>justify-content-evenly</div>
            <div class="row border border-dark flex-row-height justify-content-evenly">
            <div class="col-4 border border-dark w-25">col1</div>
            <div class="col-4 border border-dark w-25">col2</div>
            
        </div>
    </div>




</template>





<script>
export default {
    name: "column-flex",
    components: { }

}
</script>


<style>

    .row-height {
        min-height: 5rem;
        background-color: rgb(143  104 143 / .2)
    }

    .flex-row-height {
        min-height: 2rem;
        background-color: rgba(14, 117, 14, 0.4)
    }


</style>