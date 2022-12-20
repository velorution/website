<template>
<section class="clip-path px-4 bg-bermuda text-center wave-container">
      <div class="pb-12 mt-36">
             <div class="hero_title ">
                <span class="fadeInUp" style="animation-delay:0.1s;">Pour </span>  
                <span class="fadeInUp" style="animation-delay:0.2s;">une</span> 
                <span class="fadeInUp" style="animation-delay:0.3s;">vraie</span>
              </div>
              <div class="hero_title">
                <span class="fadeInUp" style="animation-delay:0.4s;">intégration</span>
                <span class="fadeInUp" style="animation-delay:0.5s;">du </span>
                <span class="fadeInUp" style="animation-delay:0.6s;">vélo  </span>
                <span class="fadeInUp" style="animation-delay:0.7s;">à  </span>
                <span class="fadeInUp" style="animation-delay:0.8s;">Cherbourg-en-cotentin  </span>
              </div> 
          <div class="md:max-w-2xl mx-auto">
          <p class="fadeInUp text-white" style="animation-delay:1s;">
            Pour le développement du vélo
          </p>
          </div>

          <div class="mb-36 mt-12 fadeInUp" style="animation-delay:1.1s;">
            <a href="https://www.helloasso.com/associations/velorution-cherbourg" class="py-2 px-4 md:py-4 md:px-6 mr-2 border select-none hover:bg-gray-100 bg-white rounded shadow-lg text-black">Bulletin d'adhésion</a>
            <NuxtLink to="/ContactPage" class="py-2 px-4 md:py-4 md:px-6 border select-none hover:bg-gray-100 bg-white rounded shadow-lg text-black">  Contact <span>&rarr;</span></NuxtLink>
          </div>
        </div>
</section>
</template>
    
<script>
    export default {
    }
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Lato&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@800&display=swap');

.wave-container {
  position: relative;
  background-image: url('@/assets/closeup-of-casual-man-legs-riding-classic-bike-on-city-road.jpg');
  background-size: cover;
  color: black;
  text-align: center;
  overflow: hidden;
}

h1 {
  font-family: 'Lato', sans-serif;
  color:black;
  font-size: 3em;
  font-weight:bold; 
}
p {
  font-size: 1.5rem;
  margin: 0 1.25rem 5rem 1.25rem;
}

span {
  display: inline-block;
}

.box{
    width:200px; 
    height:50px; 
    background: #ccc; 
    margin: 0 auto; 
    text-align:center; 
    line-height:50px;
}

.clip-path {
  width: 100%;
  min-height: 600px;
  clip-path: polygon(0 0, 100% 0, 100% 92%, 0 100%);
}

.hero_title {
    font-family: 'Raleway', sans-serif;
    font-size: 40px;
    color: white;
}
.fadeInUp{
    animation:fadeInUp 0.5s ease backwards;
    margin-left: 8px;
}

@keyframes fadeInUp{
  0%{transform:translate(0px, 30px); opacity: 0;}
  100%{transform:translate(0px, 0); opacity: 1;}
}

@media screen { 
  
}

    
</style>

