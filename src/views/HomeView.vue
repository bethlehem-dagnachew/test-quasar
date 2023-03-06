<template>
  <div class="q-pa-md">
    <div class="row">
      <div class="col col-md-8">
        <q-card class="my-card">
          <div class="text-h6 q-mb-xs">Check Out</div>
          <q-item-label class="label-text">Strong demand! Complete your order before it's too late!</q-item-label>
          <q-card class="card-cart">
            <div class="cart-text">Your cart is reserved for 10:00 minutes</div>
          </q-card>
          <q-card class="checkout">
            <q-item-label class="express-title">Express Checkout</q-item-label>
            <div class="elements">
              <q-btn class="pay">
              </q-btn>
              <q-btn class="paypal">
              </q-btn>
              <q-btn class="googlepay">
              </q-btn>

            </div>
          </q-card>
          <q-card class="lifetime">
          <q-item-label class="lifetime-label">Lifetime Warrnanty</q-item-label>
          <div class="main-warranty">
          <h5 class="sub-liftime">Add a lifetime warranty & enjoy peace of mind for life with your dream collections order for just $4.99</h5>
          <q-btn class="add-liftime">Add-$4.99</q-btn>
        </div>
          </q-card>
          <q-card-section>
           <q-pa-md>
          <div class="shiping">Contact Information</div>
          <q-form class="q-gutter-md" >
          <q-input
            filled
            type="email"
            label="Email Address"
            class="input-form"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Write Email Address']"
          />
          <q-input
            filled
            type="tel"
            label="Phone Number"
            class="input-form"
            lazy-rules
            :rules="[ val => val && val.length > 0 || 'Please Write Phone Number']"
          />
            <div class="q-gutter-sm">
              <q-checkbox v-model="right" label="Label on Right" />
    
          </div>
        </q-form>
          </q-pa-md>
          <div class="shiping">Shipping Address</div>
        </q-card-section>
        </q-card>
      </div>
      <div class="col-6 col-md-4">
        <q-card class="my-card">
          <div class="text-h6 q-mb-xs">Order Summary</div>
          
    
        </q-card>
      </div>
    </div>

  </div>
</template>

<script>

export default {
  name:'home-page',
  setup () {
  }
}
</script>


<style lang="scss" scoped>
.my-card {
  width: 95%;
  background-color: #fff;
  padding: 30px;
  border-radius: 16px;
}
#q-app{
  margin-top: 0;
}
.label-text{
  font-size: 20px;
  color: #4B4E68;
  padding-top: 20px;
  font-family: 'Poppins';
font-style: normal;
}
.text-h6{
  font-size: 36px;
  font-weight: bold;
  color: #000;
  font-family: 'Poppins';
font-style: normal;
  
}
.card-cart{
  position: relative;
  width: 100%;
  height: 100%;
  margin-top: 2vh;
  background: #EBECF3;
  border-radius: 16px;
  
}
.cart-text{
  font-family: 'Poppins';
font-style: normal;
font-weight: 500;
font-size: 16px;
line-height: 20px;
color: #4B4E68;
padding: 12px;
}
.checkout{
  box-sizing: border-box;
position: relative;
width: 100%;
height: 100%;
padding-bottom: 20px;
background: #FFFFFF;
margin-top:5%;

border: 1px solid #D6D8EE;
border-radius: 16px;
}
.elements{
  display: flex;
width: 100%;
height: 50px;
margin-left: 30px;
margin-top: 10px;
gap: 20px;
}
.pay{
  box-sizing: border-box;
  position: relative;
  width: 147px;
  height: 50px;
background: rgba(90, 49, 244, 0.1);
border: 1px solid rgba(90, 49, 244, 0.6);
border-radius: 16px;
padding: 10px;
}
.express-title{
width: 100%;
height: 30px;
font-family: 'Poppins';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 30px;
color: #000034;
margin-left: 30px;
margin-top: 2vh;
}
.paypal{
  box-sizing: border-box;
position: relative;
width: 147px;
height: 50px;
background: rgba(17, 57, 132, 0.1);
border: 1px solid rgba(17, 57, 132, 0.6);
border-radius: 16px;
}
.googlepay{
  box-sizing: border-box;
position: relative;
width: 146px;
height: 50px;

background: rgba(234, 64, 50, 0.1);
border: 1px solid rgba(234, 64, 50, 0.6);
border-radius: 16px;
}
.lifetime{
  width: 100%;
  height: 100%;
  background: #f2f3f9;
  padding-bottom: 20px;
  border-radius: 16px;
  margin-top: 30px;
}
.lifetime-label{
  position: relative;
width: 100%;
height: 30px;
left: 30px;
top: 20px;

font-family: 'Poppins';
font-style: normal;
font-weight: 500;
font-size: 20px;
line-height: 30px;

color: #000;
}
.main-warranty{
  display: flex;
}
.sub-liftime{
  position: relative;
 width: 70%;
left: 30px;
top: 7px;
font-family: 'Poppins';
font-style: normal;
font-weight: 400;
font-size: 14px;
line-height: 19px;
color: #4B4E68;
}
.add-liftime{
  display: flex;
flex-direction: row;
justify-content: center;
align-items: flex-start;
padding: 11px 30px;
gap: 10px;
position: relative;
width: 15%;
height: 20%;
top: 10px;
margin-left: 60px;
color: #fff;
background: #000034;
border-radius: 10px;
}
.shiping{
  margin-bottom: 30px;
font-family: 'Poppins';
font-style: normal;
font-weight: 500;
font-size: 24px;
line-height: 34px;
color: #000034;
margin-top: 30px;
}
.input-form{
  margin-top: 0;
 
}


</style>
