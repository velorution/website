<template>
<div>
 <section class="section_projects mt-36">
        <h2 class=" content_title  text-center my-10">Pourquoi Vélorution-Cherbourg ? </h2>
        <br>
        <p class="my-10 mt-10 mx-10 text-center">
        L'association Vélorution - Cherbourg a pour but de populariser le vélo comme mode de déplacement doux et écologique. Nous échangeons avec les communes déléguées dans le cadre des projets d'aménagements urbains afin de penser la place des vélos et ainsi les intégrer le mieux possible dans notre ville. 
        Vélorution Cherbourg est membre du réseau national FUB, la Fédération Française des Usagers de la Bicyclette, qui agit pour le vélo auprès des pouvoirs publics, réalise des campagnes de communication ainsi que des campagnes nationales comme par exemple : "cyclistes, brillez !"
        </p>
        <div class="projects__grid grid gap-8 max-w-screen-lg ">
          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg "> 
            <h3>Place du vélo sur le territoire</h3>
            <p class="project__description">
              L'association Vélorution est un des interlocuteurs de terrain pour les collectivités territoriales afin de construire les projets cyclistes du territoire d'aujourd'hui et de demain.
            </p>
            <ul class="project__stack flex">
              <a href="https://www.cherbourg.fr/"><li class="project__stack-item">Cherbourg-en-cotentin</li></a>
            </ul>
          </div>

          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg">
            <h3>Marquage Bicycode</h3>
            <p class="project__description">
              Le marquage bicycode consiste à graver sur le cadre des vélos un numéro unique et standardisé, référencé dans un fichier national accessible en ligne.
              L'objectif du dispositif est de permettre la restitution des vélos volés à leurs propriétaires par les services de police /gendarmerie et de lutter contre le recel et la revente illicite.
            </p>
            <ul class="project__stack flex">
              <a href="https://www.bicycode.org/"><li class="project__stack-item">Bycicode</li></a>
              <a href="https://moncompte.bicycode.eu/s-inscrire"><li class="project__stack-item">Inscrire son vélo</li></a>
      
            </ul>
          </div>
          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg "> 
            <h3>Bourse aux vélos</h3>
            <p class="project__description">
              L'association Vélorution organise chaque année une bourse aux vélos, au printemps. Déposez vos vélos le matin, venez trouver la bicyclette de vos rêves l'après-midi... L'association fait l'intermédiaire entre les vendeurs et les acheteurs.  
            </p>
            <ul class="project__stack flex">
              <li class="project__stack-item">lorem</li>
              <li class="project__stack-item">lorem</li>
              <li class="project__stack-item">lorem</li>
            </ul>
          </div>

          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg">
            <h3>Prévention</h3>
            <p class="project__description">
              L'association Vélorution est un des interlocuteurs de terrain pour les collectivités territoriales afin de construire les projets cyclistes du territoire d'aujourd'hui et de demain.

            </p>
            <ul class="project__stack flex">
              <li class="project__stack-item">lorem</li>
              <li class="project__stack-item">lorem</li>
              <li class="project__stack-item">lorem</li>
            </ul>
          </div>

          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg">
            <h3>Vélo-visite du patrimoine</h3>
            <p class="project__description">
              Vélorution, c'est une association citoyenne qui participe à la vie du territoire. Signaler, faire remonter des problèmes de revêtements, de signalisation, de points accidentogènes.
             
            </p>
          </div>
          <div class="px-8 py-6 mt-4 text-center bg-white shadow-lg rounded-lg">
            <h3>Moments festifs</h3>
            <p class="project__description">
              Mai à vélo, la fête du bio, rando pique-nique, rejoignez-nous ! Le vélo, c'est festif !
            </p>
          </div>

          
        </div>
      </section>

</div>

</template>

<script>

export default {

}

</script>
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@800&display=swap');

h2 {
 font-size: 2rem;
    
}

h3 {
 font-size: 2rem;
    
}

ul {
  list-style-type: none;
}

a {
  text-decoration: none;
}

/*========
  layout
========*/

.projects__grid {
  margin: 0 auto;
  grid-template-columns: repeat(auto-fit, minmax(18em, 1fr));
}

.project {
  padding: 2em;
  margin: 0 auto;
  text-align: center;
  box-shadow: var(--shadow);
  transition: transform 0.2s linear;
}

.project:hover {
  transform: translateY(-7px);
}

.project__description {
  margin-top: 1em;
  text-align: center;
}

.project__stack {
  flex-wrap: wrap;
  justify-content: center;
  margin: 1.2em 0;
}

.project__stack-item {
  margin: 0.5em;
  font-weight: 500;
  font-size: 0.8rem;
}



.project .link--icon {
  margin-left: 0.5em;
}



.content_title {
    font-family: 'Raleway', sans-serif;
    font-size: 40px;
}


</style>


