<template>
  <div class="Container">
   <div>
       <div  >
            <h2>First Wednesday's Conference</h2>
            <hr>
            <b-card no-body class="overflow-hidden" id="conferences" >
                <b-row no-gutters>
                <b-col md="6">
                    <b-card-img :src="require('@/assets/Images/1.png')"></b-card-img>
                </b-col>
                <b-col md="6">
                    <b-card-body >
                    <b-card-text>
                        Software's Architecture : From the bussiness's logic to development
                         {{on}}
                    </b-card-text>
                    
                    </b-card-body>
                    <b-button variant="danger" id="bottoms" @click="Change()" >Display</b-button>
                   
                </b-col>
                </b-row>
            </b-card>
         </div>
        </div>
  </div>
</template>

<script>
export default {
    props:["One"]
     ,
     data(){
         return{
            on:true,
         }
     },
     methods:{
         Change(){
             return this.on=!this.on;
         }
     },
     mounted(){
         this.$emit('FirstSWitch',this.on);
     }
    }

</script>

<style >

    #conferences{
        height: 300px;
        max-width: 600px;
        margin-left: 78px;
    }

       #bottoms{
        position:absolute;
        bottom: 0px;
        width: 95%;
        left: 8px;
        font-size: 20px;
        
    }
</style>

