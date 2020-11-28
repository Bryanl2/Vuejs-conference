<template>
    <div class="presentation">
        <img  class="img" src="@/assets/Images/LogoConference.png" alt="">
    <hr>
    
    <hr>

       <div  class="d-flex ">
         <FirstConference  :One="false"  :@FirstSWitch="n=$event"/>

           <SecondConference :Two="false" />

           <ThirdConference :Three="false" />
        </div>    
       
{{n}}
    <hr>
    <div class="ShowIdeas">
                <div id="juk" v-if="n===true" >
                    <h2>Software's Architecture : From the bussiness's logic to development</h2>
                        <hr>
                        <b-card no-body class="overflow-hidden" id="confe" >
                            <b-row no-gutters>
                            <b-col md="6">
                                <b-carousel
                                        id="carousel-fade"
                                        style="text-shadow: 0px 0px 2px #000"
                                        fade
                                        indicators
                                        class="Slide"
                                    
                                    >
                                        <b-carousel-slide
                                        caption="First slide"
                                        :img-src="require('@/assets/Images/First/1_1 .png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Second Slide"
                                        :img-src="require('@/assets/Images/First/2_1.png')"
                                        class="Slide"
                                        >jhghjgjg</b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Third Slide"
                                        :img-src="require('@/assets/Images/First/3_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                    </b-carousel>
                            </b-col>
                            <b-col md="6">
                                <b-card-body >
                                <b-card-text>
                                    Software's Architecture : From the bussiness's logic to development
                                </b-card-text>
                                
                                </b-card-body>
                                <b-button variant="danger" id="bottoms" @click="onClick()">Display</b-button>
                            </b-col>
                            </b-row>
                        </b-card>
                
                </div>
                
                <div id="juk" v-if="SwitchTwo===true" >
                    <h2>The road to become a Operations Engineer, experiences and learnings</h2>
                        <hr>
                        <b-card no-body class="overflow-hidden" id="confe" >
                            <b-row no-gutters>
                            <b-col md="6">
                                <b-carousel
                                        id="carousel-fade"
                                        style="text-shadow: 0px 0px 2px #000"
                                        fade
                                        indicators
                                        class="Slide"
                                    
                                    >
                                        <b-carousel-slide
                                        caption="First slide"
                                        :img-src="require('@/assets/Images/Second/1_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Second Slide"
                                        :img-src="require('@/assets/Images/Second/2_1.png')"
                                        class="Slide"
                                        >jhghjgjg</b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Third Slide"
                                        :img-src="require('@/assets/Images/Second/3_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                    </b-carousel>
                            </b-col>
                            <b-col md="6">
                                <b-card-body >
                                <b-card-text>
                                    The road to become a Operations Engineer, experiences and learnings
                                </b-card-text>
                                
                                </b-card-body>
                                <b-button variant="danger" id="bottoms" @click="onClick()">Display</b-button>
                            </b-col>
                            </b-row>
                        </b-card>
                </div>

                <div id="juk" v-if="SwitchThree===true" >
                        <h2>Trainbox the idea, product and the union with Playvox</h2>
                        <hr>
                        <b-card no-body class="overflow-hidden" id="confe" >
                            <b-row no-gutters>
                            <b-col md="6">
                                <b-carousel
                                        id="carousel-fade"
                                        style="text-shadow: 0px 0px 2px #000"
                                        fade
                                        indicators
                                        class="Slide"
                                    
                                    >
                                        <b-carousel-slide
                                        caption="First slide"
                                        :img-src="require('@/assets/Images/Third/1_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Second Slide"
                                        :img-src="require('@/assets/Images/Third/2_1.png')"
                                        class="Slide"
                                        >jhghjgjg</b-carousel-slide>
                                        <b-carousel-slide
                                        caption="Third Slide"
                                        :img-src="require('@/assets/Images/Third/3_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                    </b-carousel>
                            </b-col>
                            <b-col md="6">
                                <b-card-body >
                                <b-card-text>
                                    Trainbox the idea, product and the union with Playvox
                                </b-card-text>
                                
                                </b-card-body>
                                <b-button variant="danger" id="bottoms" @click="onClick()">Display</b-button>
                            </b-col>
                            </b-row>
                        </b-card>
                </div>
            
    </div>
               
    </div>

    
</template>

<script>
import FirstConference from './FirstConference'
import SecondConference from './SecondConference'
import ThirdConference from './ThirdConference'

export default {
    name:'MainSector',
    Data(){
        return{
            switchOne:false,
            switchTwo:false,
            switchThree:false,
            n:false,
        }
    },
    components:{
        FirstConference,
        SecondConference,
        ThirdConference

    },
    methods:{
        onClick(){
            return this.$emit('click');
        },

        ShowOne(){
            alert("hola");
            return this.$set(this.switchOne=!this.switchOne);
        },
        showTwo(){
            return this.switchTwo=true;
        },
        showThree(){
            return this.switchThree=true;
        },
    }
}
</script>

<style scoped>
    .img{
        display: inline-block;
        margin-top: 0px;
        padding: 0px;
        top: 0px;
        width: 100%;
       
    }
    .presentation{
        position: absolute;
        top: 0px;
        width: 100%;
        height: 40px;
    }
   
   #conferences{
       height: 50px;
   }

    .ShowIdeas{
        margin-top: 5%;
    }

    #juk{
        margin-top: 5%;
        margin-left:2%;
        margin-right:2%;
    }
   
</style>