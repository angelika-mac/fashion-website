<template>
  <div id="inspo-component-main">
    <div id="inspo-header">
        <div id="inspo-title">your next inspo</div>
        <div id="inspo-text">Checkout who’s wearing what by using #THREADEDInspo on Instagram</div>
    </div>
    <div id="inspo-content">
        <div class="inspo-item" v-for="(inspo, index) in aInspo" :key="index">
            <img :src="inspo">
        </div>
    </div>
    <div id="inspo-button">
        <button>VIEW ALL POSTS</button>
    </div>
  </div>
</template>

<script>
export default {
    data() {
        return {
            aInspo: [
                '../src/assets/inspo/inspo-1.png',
                '../src/assets/inspo/inspo-2.png',
                '../src/assets/inspo/inspo-3.png',
                '../src/assets/inspo/inspo-4.png',
                '../src/assets/inspo/inspo-5.png',
            ]
        }
    }
}
</script>

<style>
#inspo-component-main {
    width: 100vw;
    height: 550px;
}

#inspo-title {
    text-transform: capitalize;

    font-weight: 800;
color: #000000;
font-size: 36px;
line-height: 44px;
    text-align: center;
    margin-bottom: 50px;
}

#inspo-text {
    text-align: center;

color: #000000;
font-weight: 400;
font-size: 14px;
    margin-bottom: 50px;
}

#inspo-content {
    display: flex;
    justify-content: center;
    align-content: center;
    gap: 20px;
    margin-bottom: 50px;
}

#inspo-button {
text-align: center;
align-items: center;
display: flex;
justify-content: center;

}
#inspo-button >button {
    
background: #000000;
font-weight: 600;
font-size: 18px;
color: #FFFFFF;
padding: 10px 20px;
}
</style>