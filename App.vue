<template>
    <div class="container">
        <div class="loading" v-if="isLoading">
            <div class="loading-spinner"></div>
        </div>
        <h1 class="title">Weather App<span> made with Vue.js</span></h1>
        <div class="container-content">
            <div class="content-temp">
                <span class="content-temp-current">17 ºC</span>
                <div class="content-temp-minmax">
                    <p>Min: 11 ºC</p>
                    <p>Max: 28 ºC</p>
                </div>
            </div>
        </div>
        <h5>@douglasabnovato</h5>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>

</style>