<template>

<div class="container">
    <h3>.container</h3>
    <div class="text-start">This example shows the use of .container class. This class will cause container to be at width 100% at all responsive breakpoints. Did not see a max-width property in developer tools per docs.</div>
    <div class="border bg-danger-subtle mt-2">.container</div>
</div>

<div class="container-lg mt-2">
    <h3>.container-{breakpoint}</h3>
    <div class="text-start mt-2">This example shows the use of .container-{breakpoint} class. This class will cause container to be at width 100% for all higher breakpoints and applies a max-width for breakpoints below. </div>
     <div class="border bg-info-subtle mt-2">.container-lg</div>
</div>

<div class="container-sm mt-2">
   <div class="border bg-info-subtle mt-2">.container-sm</div>
</div>

</template>


<script>

export default {
    name: "Container"
}


</script>