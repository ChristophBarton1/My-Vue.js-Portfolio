<template>
    <div class="curvy-bg">
        <div class="works col-12 col-sm-10 col-lg-8 pt-5 mx-auto">
            <h1>Works</h1>
            <div class="d-flex flex-column">
                <work
                    image="/img/projects/lagomba.jpg"
                    title="La Gomba - Full Stack Web Project"
                    :tech="[ 'HTML5', 'CSS3','Javascript', 'PHP', 'MySQL']"
                    source="https://github.com/ChristophBarton1"
                    website="http://lagomba.com/"
                >
                <p></p>
                    <template #description>
                        La Gomba is a Website that i have made for a little Company in Vienna. I made the Front End and the Backend Part of the Website.
                        It has a wonderful Frond and a good working Payment System with a My Sql Database.
                    </template>
                    
                </work>
                <work
                    image="/img/projects/weather.jpg"
                    title="Weather App - My own Weather App"
                    :tech="['Vue.js', 'HTML5', 'CSS', 'Javascript', 'Weather-Api']"
                    source="https://github.com/ChristophBarton1"
                   
                >
                    <template #description>
                        I created my own Weather App with the Power of Vue.js and an nice working Weather Api to track the Weather at your Location.
                    </template>
                </work>
            </div>
        </div>
    </div>
</template>

<script>
import loader from '@/mixins/loader';
import Work from '@/components/Work';

export default {
    mixins: [loader],
    components: {
        Work
    }
};
</script>

<style lang="scss">
.works {
    h1 {
        
        font-size: 30px;
    }
    h6 {
        font-size: 30px;
    }

    h1 {
        font-size: 50px;
    }

    p {
        font-size: 20px;
    }
}
.tech span{
margin-bottom: 250px;
font-size: 20px;
}
.image {
    width: 450px;
    height: 550px;
    
    
}
</style>
