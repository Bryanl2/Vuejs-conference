<template>

    <div>
            <h2>Second Wednesday's Conference</h2>
            <hr>
            <b-card no-body class="overflow-hidden" id="conferences"  >
                <b-row no-gutters>
                <b-col md="6">
                    <b-card-img :src="require('@/assets/Images/2.png')"></b-card-img>
                </b-col>
                <b-col md="6">
                    <b-card-body >
                    <b-card-text>
                        The road to become a Operations Engineer, experiences and learnings
                    </b-card-text>
                    </b-card-body>
                    <b-button variant="danger" id="bottoms" @click="Change()" >Display</b-button>
                    {{Two}}
                </b-col>
                </b-row>
            </b-card>
            </div>
</template>

<script>
  export default {
     props:["Two"],
     
      methods:{
         Change(){
             return this.Two=!this.Two;
         }
     }
    }
  
</script>
