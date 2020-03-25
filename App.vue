<template>
    <div class="container">
        <div class="loading" v-if="isLoading">
            <div class="loading-spinner"></div>
        </div>
        <h1 class="title">Weather App<span> made with Vue.js</span></h1>
        <h5>@douglasabnovato</h5>
        <div class="container-content">
           
            <div class="content-temp">
                <span class="content-temp-current">17 ºC</span>
                <div class="content-temp-minmax">
                    <p>Min: 11 ºC</p>
                    <p>Max: 28 ºC</p>
                </div>
            </div>
            <button class="btn">Load Weather</button>
        </div>        
        
    </div>
</template>

<script>
    export default {
    
    }
</script>

<style scoped>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
        outline: none;
    }

    html, body{
        width: 100%;
        height: 100%;
        font-family: helvetica;        
    }

    .appear-enter-active, .appear-leave-active{
        transition: all .9s cubic-bezier(0.17, 1.03, 0.23, 1.25);
    }

    .appear-enter, .appear-leave-to{
        transform: translate(-10px);        
    }

    @keyframes spin{
        to{
            transform: rotate(360deg);
        }
    }

    .loading{
        position: absolute;
        z-index: 9999;
        width: 100%;
        height: 100%;
        display: flex;
        background-color: rgba(0,0,0,.8);
        justify-content: center;
        align-items: center;
    }

    .loading-spinner{
        border: 8px solid rgba(255,255,255);
        border-radius: 50%;
        border-left-color: lightcoral;
        width: 50px;
        height: 50px;
        animation: spin .2s linear infinite;
    }    

    .container{
        width: 100%;
        height: 100%;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        background-color: #f4f4f4;
    }

    .container-content{
        width: 320px;
        margin-top: 50px;
        display: flex;
        flex-direction: column;
        justify-content: center;
    }

    .content-temp{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 25px;
    }

</style>