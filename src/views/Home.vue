


<template>
    <div class="home d-flex flex-column flex-md-row justify-content-around">
        <div class="text-container col-12 col-md-6">
            <div class="home__img">
            <img src="/img/icons/profile.jpg" alt="about__img">
        </div>
            <span class="title">I am Christoph Barton</span>
            <span class="sub-title">Web / App Developer</span>
            <a download= "Lebenslauf-ChristophBarton.pdf" href="/img/icons/Lebenslauf-ChristophBarton.pdf" button class="btn"><i class="fa fa-download"></i> Download Resume</a>
            <p></p>
            <a download= "Zertifikat-Backend-Web-Developer.png" href="/img/icons/Zertifikat-Backend-Web-Developer.png" button class="btn"><i class="fa fa-download"></i> Backend Developer Certification</a>
        
        </div>
        
            
           
    </div>
  
</template>

<script>








import loader from '@/mixins/loader';

export default {
    name: 'Home',
    mixins: [loader],
    mounted() {
        // fallback for old browsers
        const minHeight = window.innerHeight - 200;
        document.querySelector('.home').style.minHeight = `${minHeight}px`;
    }
};



</script>

<style lang="scss">
@import '~rfs/scss';

.home {
    height: var(--desktop-full-height);
    .mobile-view > & {
        height: var(--mobile-full-height);
    }
}



.text-container {
    color: white;
    align-items: center;
    

    .title {
        @include font-size(54px);
        margin-bottom: 0px;
    }

    .sub-title {
        @include font-size(16px);
        color: #969696;
        margin-bottom: 100px;
    }
}

.text-container,
.image-container {
    flex-shrink: 1;
    display: flex;
    flex-direction: column;
    margin-top: 2px;
    
}


.btn {
  background-color: DodgerBlue;
  border: none;
  color: white;
  padding: 12px 30px;
  cursor: pointer;
  font-size: 20px;
  margin-top: 5px;
}

/* Darker background on mouse-over */
.btn:hover {
  background-color: RoyalBlue;
}

.home__img {
  padding-top: 0.0rem;
  padding-left: 0.0rem;
  width: 160px;
  height: 180px;
  
  background-color: var(--first-color);
  border-radius: 50%;
  overflow: hidden;
  margin-bottom: 80px;
  margin-top: 200px;
  
  

  
  
    
}
img {
    max-width: 100%;
    height: auto;
    display: block;
    
  }

  title {
      
  }
</style>
