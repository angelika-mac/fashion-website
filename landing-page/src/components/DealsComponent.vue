<template>
    <div id="deals-component-main">
        <div id="deals-wrapper">
            <div class="deal-item" v-for="(deal, index) in aDeals" :key="index">
                <div class="deal-area-1">
                    <div class="deal-price">
                        {{ deal.price }}
                    </div>
                    <div class="deal-off">
                        OFF
                    </div>
                </div>
                <div class="deal-area-2">
                    {{ deal.description }}
                </div>
            </div>
            <div id="check-deals" class="deal-item">
                <button >CHECKOUT ALL SITE-WIDE DEALS</button>
            </div>
        </div>
        <div id="excl-wrapper">
            <img src="../assets/vip-sparkle.svg">
            <div id="excl-title">
                BLACK FIRDAY ECLUSIVE
            </div>
            <div id="excl-subtitle">
                free shipping on all orders for VIP 2 and up!
            </div>
            <div id="excl-button">
                <button>SHOP NOW</button>
            </div>
        </div>
        
    </div>
</template>

<script>
export default {
data() {
    return {
        aDeals: [
            {
                price: '$5',
                description: 'on orders above $50'
            },
            {
                price: '$15',
                description: 'on orders above $75'
            },
            {
                price: '$20',
                description: 'on orders above $75'
            },
            {
                price: '$30',
                description: 'on orders above $1200'
            }
        ]
    }
}
}
</script>

<style>
#deals-component-main {
    width: 100vw;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 10px;
    padding-left: 20px;
    flex-direction: column;
}

#deals-wrapper{
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 140px;
    margin: 20px 0;
}

.deal-item {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 10px;
}

.deal-price{
    font-weight:  600;
    font-size: 32px;
}

.deal-off{
    font-weight:  800;
    font-size: 18px;
}

.deal-area-1 {
    display: flex;
    align-items: center;
    gap: 20px;
}

.deal-area-2 {
    font-weight: 400;
    font-size: 10px;
}

#check-deals {
    padding-right: 30px;
}

#check-deals > button {
    width: 363px;
    height: 42px;
    padding: 10px 20px;
    background-color: #000000;
    color: #fff;
    font-weight: 600;
    font-size: 18px;
}

#excl-wrapper{
    height: 75px;
    width: 100vw;
    background-image: linear-gradient(90deg, rgba(0, 0, 0, 0) 13.54%, #000000 40.1%, #000000 100%);
    display: flex;
    align-items: center;
    gap: 240px;
    padding: 0 20px;
}

#excl-title {
    font-weight: 800;
    font-size: 32px;
    text-transform: uppercase;
    padding: 30px;
}

#excl-subtitle{
    text-transform: uppercase;
    font-weight: 600;
    font-size: 18px;
    color: #fff
}

#excl-button > button {
    padding: 10px 20px; 
    background-color: #fff;
    color: #000000;
    font-weight: 600;
    font-size: 18px;
}

#excl-wrapper >img {
    position: absolute;
    z-index: -9;
}
</style>