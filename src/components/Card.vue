<template>
 <div class="cardBody">
        <div class="iconBackground">
            <div class="cardContents">
                <div>
                    <img src="../images/patriciaLogo.svg" alt="logo">
                    <button @click="showPass = !showPass" class="passwordEye">
                        <span v-show="!showPass">
                            <img src="../images/MaskClosed.svg" alt="passwordEye">
                        </span>
                        <span v-show="showPass">
                            <img src="../images/Mask.svg" alt="passwordEye">
                        </span>
                    </button>
                </div>

                <div class="passwordText">
                    <input type="password" v-model="password" v-show="!showPass" id
                    readonly/><span v-show="!showPass"
                        class="passwordAppendage">9784</span>
                    <input type="text" v-model="password" v-show="showPass" readonly/><span v-show="showPass"
                        class="openPasswordAppendage">9784</span>
                </div>

                <div class="footerInfo">
                    <p class="cardName">
                        Cardholder's Name
                    </p>
                    <div class="footerRightInfo">
                        <p class="validDate">
                            VALID <br> THRU
                        </p>
                        <p>
                            10/21
                        </p>
                        <p class="ccv">
                            <label for="">CCV</label>
                            <input type="password" id="hiddenPassword" value="123" readonly/>
                        </p>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>

<script>
export default {
  name: 'Card',

    data(){
     return{
            showPass: false,
            password: '9784       9784       9784',
        }
   }
}
</script>

<style >
</style>
