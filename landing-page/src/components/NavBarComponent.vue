<template>
  <div id="nav-bar-wrapper">
    <div id="nav-bar-header">
        <div id="header-left">
            <div>WOMEN</div>
            <div>PLUS</div>
            <div>MEN</div>
            <div>ACCESORIES</div>
        </div>
        <div id="header-center">
            <img src="../assets/logo.svg">
        </div>
        <div id="header-right">
            <div id="right-icons">
                <div v-for="(icon, index) in aIcons" :key="index" class="nav-icons">
                    <img :src="icon">
                </div>
            </div>
            <div id="right-currency">
                <div id="currency-wrapper">
                    <img src="../assets/us flag.svg" id="currency-flag">
                    <div>USD$</div>
                    <img src="../assets/arrow-down.svg" id="currency-arrow">
                </div>
            </div>
        </div>
    </div>
    <div id="nav-bar-subheader">
        <div class="perks-icon" v-for="(perk, index) in aBenefits" :key="index">
            <div class="icon">
                <img :src="perk.icon">
            </div>
            <div class="desc">{{perk.description}}</div>
        </div>
    </div>
  </div>
</template>

<script>
export default {
    data() {

        return {
            aIcons: [
                '../src/assets/account.svg',
                '../src/assets/cart.svg',
                '../src/assets/wish.svg',
                '../src/assets/support.svg',
                '../src/assets/search.svg',
            ],
            aBenefits: [
                {
                    icon: '../src/assets/vip.svg',
                    description: 'Exclusive Deals for VIP 2 and up!'
                },
                
                {
                    icon: '../src/assets/star.svg',
                    description: 'Weekly New Arrivals'
                },
                
                {
                    icon: '../src/assets/shipping.svg',
                    description: 'Free Shipping On Orders Over $100'
                },
                
                {
                    icon: '../src/assets/pin.png',
                    description: 'Track Your Order'
                },
                
                {
                    icon: '../src/assets/tag.svg',
                    description: '10% Off On Your First Order!'
                }
            ]
        };
    }
}
</script>

<style>
#nav-bar-wrapper {
    display: flex;
    flex-direction: column;
}
#header-left > div {
    
  font-weight: 400;
  font-size: 14px;
  cursor: pointer;
  align-items: center;
}

#header-left > div:hover{
  font-weight: 600;
  font-size: 16px;
}
#nav-bar-header {
    height: 70px;
    display: flex;
    justify-content: space-between;
    text-align: center;    
    padding: 0 20px;
    align-items: center;
}

#header-center {
    text-align: center;
}

#currency-wrapper {
    width: 100px;
    height: 35px;

    background: #FFFFFF;
    border: 1px solid #F2F2F2;
    border-radius: 35px;
    box-sizing: border-box;
    text-align: center;

    justify-content: center;
    gap: 4px;

    align-items:center ;

}

#currency-flag {
    width: 25px;
    height: 25px;
}

#currency-arrow {
    width: 10px;
    height: 10px;
}

#right-icons {
    display: flex;
    gap: 20px;
    text-align: center;
    align-items: center;
    margin-right: 10px;
}
#header-left, #header-right, #currency-wrapper{
    display: flex;
}

#header-left {
    gap: 20px;
}

#nav-bar-subheader{
    background-color: #F2F2F2;
    width: 100vw;
    height: 50px;
    text-align: center;

    display: flex;
    justify-content: space-around; /* Optional: Adjust this value to change the space between icons */
    align-items: center;
}

.perks-icon {
    font-style: normal;
    font-weight: 400;
    font-size: 12px;
    line-height: 15px;

    display:flex;
    justify-content: space-between;
    text-align: center;
    align-items: center;

    gap: 10px;
}

</style>