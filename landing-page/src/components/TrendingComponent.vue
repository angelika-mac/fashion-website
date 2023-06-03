<template>
    <div id="trending-component-main">
        <div id="trend-wrapper">
            <div id="trend-header">
                <span id="tr-header-title">Now Trending</span>
                <span id="tr-header-sub">See what everyone’s wearing right now</span>  
            </div>
            <div class="trend-categ">
                <div class="categ-row" v-for="(categ1, index) in aCateg1" :key="index">
                    <div class="categ-image">
                        <img :src="categ1.image" />
                    </div>
                    <div class="categ-name">
                        {{ categ1.name }}
                    </div>
                </div>
            </div>
            <div class="trend-categ">
                <div class="categ-row" v-for="(categ2, index) in aCateg2" :key="index">
                    <div class="categ-image">
                        <img :src="categ2.image" />
                    </div>
                    <div class="categ-name">
                        {{ categ2.name }}
                    </div>
                </div>
            </div>
            <div id="trend-tags">
                <div class="trend-tags" v-for="(tag, index) in aHashtags" :key="index">
                    {{ tag }}
                </div>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
    data() {
        return {
            aCateg1: [
                {
                    name: 'Winter Fashion',
                    image: '../src/assets/trending/trend-1.png'
                },
                {
                    name: 'Boots',
                    image: '../src/assets/trending/trend-2.png'
                },
                {
                    name: 'Night out',
                    image: '../src/assets/trending/trend-3.png'
                },
                {
                    name: 'Holidays',
                    image: '../src/assets/trending/trend-4.png'
                },
            ],

            aCateg2: [
                {
                    name: 'Outerwear',
                    image: '../src/assets/trending/trend-5.png'
                },
                {
                    name: 'White dress',
                    image: '../src/assets/trending/trend-6.png'
                },
                {
                    name: 'Sweaters',
                    image: '../src/assets/trending/trend-7.png'
                },
                {
                    name: 'Party',
                    image: '../src/assets/trending/trend-8.png'
                },
            ],

            aHashtags: [
                '#Thanksgiving',
                '#NewYears',
                '#Knitted',
                '#Pajamas',
                '#WFH',
                '#FallFashion'
            ]
        }
    }
}
</script>

<style>
#trending-component-main{
    display: flex;
    flex-direction: column;
    width: 103vw;
    height: 1040px;
    align-items: center;
}


#trend-header {
    margin-top: 50px;
    display: flex;
    align-items: center;
    flex-direction: column;
    gap: 50px;
}

#tr-header-title {
    font-weight: 800;
    font-size: 36px;
    color: #000000;
}

#tr-header-subtitle {
    margin-bottom: 50px;
}

.trend-categ {
    display: flex;
    align-items: center;
}

.categ-row {
    display: flex;
    align-items: center;
    flex-direction: column;
    width: 265px;
    height: 390px;
    padding: 20px;

}

.categ-name {
    text-align: center;
text-transform: uppercase;

color: #000000; 
font-weight: 600;
font-size: 24px;
}

#trend-tags {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
}

.trend-tags {
    box-sizing: border-box;
    padding: 10px 20px;
    height: 37px;
    background: #FFFFFF;
    border: 1px solid #000000;
    border-radius: 50px;
    font-weight: 600;
    font-size: 14px;
    color: #000000;
}
</style>