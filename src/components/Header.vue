<template>
    <div class="header">
        
        <router-link to="/"></router-link>
        <div class="search" >
            <HeaderSearch/>
            <HeaderCategory/>
        </div>
        <HeaderCart/>
    </div>
    
</template>

<script>
import HeaderCart from './HeaderCart.vue'

import HeaderSearch from './HeaderSearch.vue'
export default {
    name: 'Header',
    components: {
        HeaderCart,
        HeaderSearch,
      
    },
}
</script>

<style scoped>
*{
    margin: 0;
    padding: 0;
}
.header {
    padding-left: 25%; 
    margin: 35px auto;
    height: 58px;
    width: 100%;
    overflow: hidden;
}
.header .search{
    width: 400px;
    height: 100%;
    overflow: hidden;
    float: left;
}
.header > a{
    float: left;
    margin-right: 60px;
    width: 142px; 
    height: 140px;
    text-decoration: none;
    background: url(../assets/logo.png) ;
    
    vertical-align: bottom;
}

</style>