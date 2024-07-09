<script>

import { RouterLink } from 'vue-router'
export default {
    components: {
        RouterLink
    }
}

</script>


<template>

    <div class="headerArea">
        <RouterLink class="routeItem" to="/">Home</RouterLink>
        <RouterLink class="routeItem" to="/VtextAndVmodel">VtextAndVmodel</RouterLink>
        <RouterLink class="routeItem" to="/test_new">test_new</RouterLink>
    </div>


</template>


<style scoped>

.headerArea {
    width: 100%;
    height: 100%;
    background-color: aqua;
    display: flex;
    align-items: center;
    .routeItem{
        margin: 3%;
        font-size: 36px;
        color: white;
        text-decoration: none;
        cursor: pointer;
    }
}

</style>