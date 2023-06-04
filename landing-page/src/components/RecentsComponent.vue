<template>
    <div id="recents-component-main">
        <div id="recents-header">
            Recently Bought
        </div>
        <div id="recents-content">
            <div class="recent-item" v-for="(recent, index) in aRecents" :key="index">
                <div class="recent-img">
                    <img :src="recent.image">
                </div>
                <div class="recent-name">
                    {{ recent.name }}
                </div>
                <div class="recent-price">
                    <div class="recent-sale" v-if="recent.sale_price !== null">
                        {{ recent.sale_price }}
                    </div>
                    <div class="recent-og" :style="recent.sale_price == null ? '' : 'text-decoration: line-through'">
                        {{ recent.price }}
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            aRecents: [
                {
                    image: '../src/assets/recent/recent-1.png',
                    name: 'Festive Looks Rust Red Ribbed Velvet Long Sleeve Bodysuit',
                    sale_price: null,
                    price: '$38'
                },
                {
                    image: '../src/assets/recent/recent-2.png',
                    name: 'Chevron Flap Crossbody Bag',
                    sale_price: '$5.77',
                    price: '$7.34',
                },
                {
                    image: '../src/assets/recent/recent-3.png',
                    name: 'Manilla Tan Multi Plaid Oversized Fringe Scarf',
                    sale_price: '$29',
                    price: '$39',
                },
                {
                    image: '../src/assets/recent/recent-4.png',
                    name: 'Diamante Puff Sleeve Dress - Black',
                    sale_price: null,
                    price: '$45.99',
                },
                {
                    image: '../src/assets/recent/recent-5.png',
                    name: 'Banneth Open Front Formal Dress in Black',
                    sale_price: '$69',
                    price: '$99.95',
                }
            ]}
    }
    
}
</script>

<style>
#recents-component-main {
    width: 103vw;
}
#recents-header {
    margin-top: 50px;
    text-transform: capitalize;
    color: #000000;
    font-weight: 800;
    font-size: 36px;
    color: #000000;
    text-align: center;
}

#recents-content{
    display: flex;
    justify-content: center;
}
.recent-item {
    width: 225px;
    height: 400px;
    padding: 20px;
    display: flex;
    flex-direction: column;
    cursor: pointer;
}

.recent-price {
    display: flex;
    align-items: flex-start !important;
    justify-content: flex-start !important;
    gap: 20px;
}

.recent-name {
    font-weight: 400;
font-size: 14px;
text-transform: capitalize;

color: #000000;
}

.recent-og {
    font-weight: 600;
    font-size: 14px;
    text-transform: capitalize;

    color: #000000;
}

.recent-sale {
    font-weight: 800;
font-size: 14px;
text-transform: capitalize;

color: #C1272D;

}
</style>