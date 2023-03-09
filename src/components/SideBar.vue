<script setup>
    import {defineEmits} from "vue";

    const emits = defineEmits(['selectOption'])
    function selectOption(isColor){
        emits("selectOption", isColor)
     }

</script>


<template>
    <v-navigation-drawer
        expand-on-hover
        rail
    >
    <v-list>
          <v-list-item
            prepend-avatar="https://lh3.googleusercontent.com/IwKcQSNmrWzS3GV1GtBV3V5M3-_pDwxYrUvShpmRxF6mB6v5aG8eMY62vxr6TWUaONdI5ztposgAiKeDia-xAfCfou3QiSKQaTpmw8ON3TOhjyxZ0ePSpPtL-DB8WLmazoTawcDEXQh5qRyv7LZgHKKox1Hx1H5d8LXJdNHaKmqaVzB_40iK9XzodVIvYc3ZCFmnbxoUPxkpB-gMOaVf1w481d3Ui1YcIbzEcpJR2X4diRamf9Ds0s58te5KFGABN49ymTa305xnEWbW5JlRMGuEMS5Fdqg0i5d_JWTUn8oQ_bSUAdwtOo9IJev6dYAkW-XFHqvLToReYTsvvw1CUunUcxRfJhKkzu2HsvDyQF_UVgHIh-nlZz_uWlgYLdmQnFDKg0nnETBLimERvuRz3IqdXRMQRXOOlcXXzpwLcfKrxfQTzZre12BG3LYshPv6tovje-P3XELYs1hjV90P8ve7yf8BbsL0clo53Un1WHGiQY_3yr77IPeXF2iPGCeVnwcvBn1GFxR9fHb_mOF1tzoT6jnumlkbeScijvk9QjvxXkdOIN4fMeg--9i3hvy2pUUNA5DTCSjud1VQCrrtiW9pc4omzW9ZxehlUh2cF_3o-dYnAN_q8ltW7izOvGFbVqr5-tNWkNCvo53NmyhcUZMWNnRyCzv-G8DV0LDuaK93hYCs0yMg1Y9X6FCzwsRn2P9dys_Zk7hNNOLYYu9wOsZIwuasAWFl1OSUwtl6kYhAms2grEey0iDmyeMBkiQZ69JKRx75WmxNWjIli6qelGQQJ2V5801tD2crH36o71N_jvqr8UEKAIKjBSJGw_GSvgdwdFeQlXM1jYxw8VPrnwwTctqHBxC7q_0Tyq8zkFS0pchVcrp0tLKeGeZpV2IVpAr2q3sjODzDTx4iB_PlFB8CLB_yVqG5-ug5rjKCvbwJ=w434-h771-no?authuser=0"
            title="Arnaud Ngari"
            subtitle="jules.ngari@gmail.com"
          ></v-list-item>
    </v-list>

    <v-divider></v-divider>

    <v-list density="compact" nav>
           <v-list-item 
           prepend-icon="mdi-image" 
           title="Color Gallery" 
           value="color"
            @click="selectOption(true)"
          >
          </v-list-item>

           <v-list-item 
           prepend-icon="mdi-dialpad" 
           title="GraySpaceGallery" 
           value="color"
           @click="selectOption(false)"
           >
           </v-list-item>
    </v-list>

    </v-navigation-drawer>
</template>