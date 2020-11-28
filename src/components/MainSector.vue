<template>
    <div class="presentation">
        <img  class="img" src="@/assets/Images/LogoConference.png" alt="">
    <hr>
    
    <hr>

       <div  class="d-flex ">
         <FirstConference  :One="false"  :@FirstSWitch="switchOne=$event"/>

           <SecondConference :Two="false" />

           <ThirdConference :Three="false" />
        </div>    
       
{{n}}
    <hr>
    <div class="ShowIdeas">
                <div id="juk" >
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
                                        caption=""
                                        :img-src="require('@/assets/Images/First/1_1 .png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
                                        :img-src="require('@/assets/Images/First/2_1.png')"
                                        class="Slide"
                                        >j</b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
                                        :img-src="require('@/assets/Images/First/3_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                    </b-carousel>
                            </b-col>
                            <b-col md="6">
                                <b-card-body >
                                <b-card-text>
                                    Here he took the main concepts about the Software Architecture like:
                                    -What is Software Architecture?
                                    -How it works?
                                    -What are the main challenges in a near future?

                                    Some of the concepts that answers those questions are:

                                    -It shows the system's structure, but hide details about implementationbundleRenderer.
                                    -Lead the delivered requirements from different stakeholdersbundleRenderer.renderToStream
                                    -Consider the functional and QA requirements.

                                </b-card-text>
                                
                                </b-card-body>
                                
                            </b-col>
                            </b-row>
                        </b-card>
                
                </div>
                
                <div id="juk" >
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
                                        caption=""
                                        :img-src="require('@/assets/Images/Second/1_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
                                        :img-src="require('@/assets/Images/Second/2_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
                                        :img-src="require('@/assets/Images/Second/3_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                    </b-carousel>
                            </b-col>
                            <b-col md="6">
                                <b-card-body >
                                <b-card-text>
                                    Different concepts about operating were taken.
                                    For example:
                                    -Security : Normally operating's people are seen like the ones in charge
                                    to protect and hold the security inner the organization where they work. Among
                                    the many roles and occupations that they have , it is needed to make or include different
                                    strategies that allows better performance in this field.
                                    -Performance Databases
                                    -Study computer's networking.
                                    -Recomendations.
                                </b-card-text>
                                
                                </b-card-body>
                                
                            </b-col>
                            </b-row>
                        </b-card>
                </div>

                <div id="juk"  >
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
                                        caption=""
                                        :img-src="require('@/assets/Images/Third/1_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
                                        :img-src="require('@/assets/Images/Third/2_1.png')"
                                        class="Slide"
                                        ></b-carousel-slide>
                                        <b-carousel-slide
                                        caption=""
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
                                    Here were taken a lot of different topics related to entrepreneurship , and how was the beginning of 
                                    a bussiness idea.
                                    Principally showed how a game's idea was becoming or branching on differents ways and aspects of the bussiness
                                    . Showed how the opportunities are there waiting for to be taken by people that can reach them and aboard them
                                    with the enough enthusiasm.

                                    Among all the different game's ideas related to gaming we can find out :

                                    -MaxTurbo
                                    -SinAbuso
                                    -VitimaLz

                                    And how the union between playvox and trainbox was done.

                                    Here the main advice and message from the expositor was to engage the people toward the enthusiasm and 
                                    the hard work with a strong discipline to take challenges, and to make them know that there are a big variety
                                    of rewards in this field .
                                </b-card-body>
                                
                            </b-col>
                            </b-row>
                        </b-card>
                </div>
                <br>
                <hr>
            
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
            switchOne:true,
            switchTwo:false,
            switchThree:false,
            n:true,
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
        margin-left:9%;
        margin-right:5%;
        font-size: 25px;
        margin-bottom: 2%;
       
    }
   
</style>