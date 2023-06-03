<template>
    <div id="hero-component-main">
        <div id="hero-wrapper">
            <div id="bg-wrap">
                <img src="../assets/hero-1.png" id="hero-img-1"/>
                <img src="../assets/hero-2.svg" id="hero-img-2"/>
            </div>
            <div id="hero-nav">
                <img src="../assets/arrow-left.svg" id="hero-arrow-left"/>
                <img src="../assets/arrow-right.svg" id="hero-arrow-right"/>
            </div>
            
            <div id="hero-misc">
                <div id="hero-shop">
                    <img src="../assets/hero-text.svg" id="hero-text"/>
                    <button id="shop-now">SHOP NOW</button>
                </div>
                <img src="../assets/hero-slider.svg" id="hero-slider"/>
            </div>
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>
#hero-wrapper {
    width: 100vw;
    height: 650px;
    background-color: #EDE9DD;
}

#hero-nav {
    width: 100vw;
    height: 650px;
    position: absolute;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

#hero-nav > img {
    width: 50px;
    height: 50px;
}

#bg-wrap {
    position: relative;
}

#hero-img-1, #hero-img-2 {
    height: 650px;
}

#hero-img-1 {
    position: absolute
}


#hero-img-2 {
    opacity: 0.2;
    top: 0;
    right: 0;
    position: relative;
    float: right
}

#hero-arrow-left {
    text-align: center;
}

#hero-misc {
    width: 103vw;
    height: 650px;
    position: absolute;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
}

#hero-slider{
    width: 50px;
    height: 15px;
    padding: 20px;
}

#shop-now {
    background-color: #fff;
    width: 278px;
    height: 74px;
    box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
    cursor: pointer;
    border: none;
    font-weight: 600;
    font-size: 36px;
    align-items: center;
text-align: center;
}

#hero-text {
    width: 644px;
    height: 446px;
}

#hero-shop {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: absolute;
    right: 0;
    gap: 20px;
}

</style>