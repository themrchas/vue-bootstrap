<template>

<div class="container">
    <h3>.container</h3>
    <div class="text-start">This example shows the use of .container class. This class will put a max-width in px on the container and width:100% on children (by default).</div>
    <div class="border bg-danger-subtle mt-2">.container</div>
</div>

<div class="container-lg mt-2">
    <h3>.container-{breakpoint}</h3>
    <div class="text-start mt-2">This example shows the use of .container-{breakpoint} class. This class will put a max-width in px on container and set container and children at width:100% (by default) for all 'lower' breakpoints and applies a width: 100% to container for breakpoints above.</div>
    <div class="border bg-info-subtle mt-2">.container-lg</div>
</div>

<div class="container-sm mt-2">
   <div class="border bg-info-subtle mt-2">.container-sm</div>
</div>

<ViewportInfo />

<div class="container-fluid mt-3">
    <h3>.container-{fluid}</h3>
    <div class="text-start mt-2">This class will put width:100% on the container through all viewport sizes.  Children are assigned width:100% by default.</div>
    <div class="border bs-gray-400 mt-2">.container-fluid</div>
</div>

</template>


<script>

import ViewportInfo from './ViewportInfo.vue';

export default {
    name: "container",
    components: { ViewportInfo }

}


</script>