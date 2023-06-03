<template>
  <div id="newprod-component-main">
    <div id="arrival-wrapper">
            <div id="arrival-content">
                <div id="arrival-title">
                    NEW<br>ARRIVALS
                </div>
                <div id="arrival-text">
                    Get ready for the holidays with us!
                </div>
                <div id="arrival-btn">
                    <button>SHOP NOW</button>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>


#arrival-wrapper {
    margin-top: 50px;
    width: 103vw;
    height: 400px;
    background-image: url('../assets/arrival-banner.png');
  background-size: 2000px 500px;
  display: flex;
    align-items: center;
    justify-content: flex-end;
}

#arrival-title {
    font-style: normal;
font-weight: 800;
font-size: 86px;
color:#FFFFFF
}

#arrival-text {
    font-style: normal;
font-weight: 600;
font-size: 28px;
color:#FFFFFF
}

#arrival-btn > button {
    text-transform: uppercase;

    background-color: #FFFFFF ;
    color: #000000;
    font-weight: 600;
    font-size: 18px;
    width: 149px;
height: 42px;
border: none;

}

#arrival-content {
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding-right: 50px;
    
}
</style>