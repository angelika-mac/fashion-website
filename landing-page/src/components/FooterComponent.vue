<template>
  <div id="footer-component-main">
    <div id="footer-wrapper">
        <div id="footer-text">
            sign up for exclusive deals and updates
        </div>
        <input type="email" id="footer-email" placeholder="Your email address">
    </div>
    <div id="footer-links-wrapper">
        <div id="footer-links">
            <div class="link-section">
                <div class="link-title">
                    COMPANY INFO
                </div>
                <div>About THREADED</div>
                <div>Affiliate</div>
                <div>Blog</div>
                <div>Careers</div>
            </div>
            <div class="link-section">
                <div class="link-title">
                    Help & Support
                </div>
                <div>FAQ</div>
                <div>SHIPPING</div>
                <div>RETURNS</div>
                <div>HOW TO ORDER</div>
                <div>HOW TO TRACK</div>
            </div>
            <div class="link-section">
                <div class="link-title">
                    CUSTOMER CARE
                </div>
                <div>CONTACT US</div>
                <div>PAYMENT METHODS</div>
            </div>

            <div class="link-section">
                <div class="link-title">
                    FOLLOW US
                </div>
                <img src="../assets/socmed/facebook.svg">
                <img src="../assets/socmed/instagram.svg">
                <img src="../assets/socmed/twitter.svg">
                <img src="../assets/socmed/youtube.svg">
                <img src="../assets/socmed/pinterest-alt.svg">
                <img src="../assets/socmed/bx_bxl-tiktok.svg">
                
                <div class="link-title">
                    WE ACCEPT
                </div>
                <img class="payment-icons" src="../assets/payment/visa.png">
                <img class="payment-icons" src="../assets/payment/mastercard.png">
                <img class="payment-icons" src="../assets/payment/maestro.png">
                <img class="payment-icons" src="../assets/payment/amex.png">
                <img class="payment-icons" src="../assets/payment/paypal.png">
            </div>
        </div>
        <div id="footer-rights">
            <div id="footer-copy">
                ©2021 THREADED All Rights Reserved.
            </div>
            <img src="../assets/logo.svg">
        </div>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
#footer-component-main {
    width: 100vw;
}

#footer-wrapper {
    background-color: #000;
    height: 75px;
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px
}

#footer-text {
    font-style: normal;
font-weight: 800;
font-size: 32px;
line-height: 39px;
display: flex;
align-items: center;
text-transform: uppercase;
color: #fff;
}

#footer-email {
    height: 35px;
    width: 300px;
    font-family: 'Montserrat';font-style: normal;
font-weight: 400;

}


#footer-copy {
    font-weight: 400;
    font-size: 12px;
}
#footer-rights{
    display: flex;
    align-items: center;
    text-align: center;
    padding: 20px;    
    justify-content: space-between;
}

#footer-rights >img {
    padding: 20px;
}

.payment-icons{
    width: 37.5px;
    width: 25px;
    margin-right: 10px;
}
.link-section {
    text-transform: capitalize;

color: #000000;
font-weight: 400;
font-size: 12px;
}
.link-title {
    font-weight: 600;
font-size: 12px;
text-transform: uppercase;

color: #000000;

}

#footer-links {
    display: flex;
    justify-content: center;
    gap: 50px;
    margin-top: 50px;
}
.link-section > div{
    margin: 10px 0px;
}

.link-section > .link-title{
    margin-bottom: 20px;
}
</style>