<template>
 
   <div>

           <div>
           <h2>Third Wednesday's Conference</h2>
            <hr>
            <b-card no-body class="overflow-hidden" id="conferences"  >
                <b-row no-gutters>
                <b-col md="6">
                    <b-card-img :src="require('@/assets/Images/3.png')" @click="onClick()"></b-card-img>
                </b-col>
                <b-col md="6">
                    <b-card-body >
                    <b-card-text>
                       Trainbox the idea, product and the union with Playvox
                    </b-card-text>
                    </b-card-body>
                    <b-button variant="danger" id="bottoms" @click="Change()">Display </b-button>
                    {{Three}}
                </b-col>
                </b-row>
            </b-card>
            </div>
 
</div>
</template>

<script>
  export default {
      props:["Three"],
      
    
     methods:{
         Change(){
             return this.Three=!this.Three;
         }
     }
  }
</script>
