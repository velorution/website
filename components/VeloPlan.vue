<template>
    <div>

    <div class="w-screen h-screen flex justify-center">
        <div class="w-7/12 h-7/12">
        <h1 class="text-center">Le plan vélo de Vélorution</h1>
        <h2 class="text-center">Pour une vraie intégration du vélo en ville</h2>
        <br>
        <p >
          L'état des lieux du réseau cycliste sur Cherbourg montre des réalisations faites ces dernières années, sur les 5
          communes de l'agglomération en faveur de la pratique du vélo.</p>
        <br>
          <p>
          Des pistes , des aménagements, des lieux de stationnement, des zones dites « 30 » , existent.
        </p>  
        <br>
        <p>
            Parmi ces réalisations, les pistes Saline - Fort de Querqueville et Gare maritime - Collignon sont plébiscitées par les Cherbourgeois. 
        </p> 
        <p>
            Les double-sens de circulation dans les zones de partage ont été mis en place en ville, même s'ils rencontrent quelquefois des réserves de la part des utilisateurs. Des aires de stationnement ont été créées un peu partout en ville (arceaux , quelques abris).
        </p>
        <br>
        <p>
            On peut donc reconnaître que des avancées ont été faites dans le développement des structures liées au vélo.
        </p> 
        <br>
        <p>
        Cependant les Cherbourgeois pratiquant régulièrement le vélo sur l'agglomération, constatent que le réseau devrait être amélioré, et notamment sur des domaines précis :
        </p>
        <br>
        <ul class="list-disc mx-6">
            <li>La continuité des pistes existantes et l'extension de celles-ci vers l'Est et l'Ouest de Cherbourg-en-Cotentin.</li>
            <li>La sécurité vis-à-vis de la cohabitation avec les voitures et du vol de vélos.</li>
            <li>Le stationnement qui est absent dans certaines zones fréquentées, pas assez aménagé et sous- équipé.</li>
             ex. : abris fermés et sécurisés )
            <li>La promotion de la pratique du vélo, par la communication vers les jeunes publics, par la mise en place d’événements, par des incitations financières à l'acquisition d'un vélo.</li>
        </ul>
        <br>
        <p>
            Nous pensons, à Vélorution, et avec ces cyclistes réguliers, qu' il faut affirmer la place du vélo à Cherbourg, et qu'il devienne un moyen de déplacement à part entière, pas seulement un moyen utilisé pour ses loisirs.
        </p>
        <br>
        <p>
        Beaucoup de personnes sont prêtes à franchir le pas de la pratique du vélo, mais hésitent justement en raison du manque structurel actuel du réseau.
        </p>
        <br>
        <p>
            Vélorution Cherbourg et les cyclistes de l'agglomération, de par leur exercice quotidien du vélo, sont à même de faire des propositions concrètes pour l'amélioration de ce réseau sur tous les thèmes liés. Nous nous faisons le relais des souhaits et des préoccupations des cyclistes Cherbourgeois.
        </p>
        <br>
        <p>
            Notre affiliation à la Fédération des Usagers de la Bicyclette, nous met en relation avec des associations, des villes ayant fait du vélo une priorité et qui aujourd'hui voit les effets positifs de ce choix.
        </p>
        <br>
        <p>
        Vélorution participe aussi aux comités de consultation mis en place par les élus, lors de projets urbains, pour que le vélo soit intégré au mieux dans ces projets.
        </p>
        <br>
        <h2>Plan général des propositions de Vélorution</h2>
        <br>
        <br>
        <p>
            Télécharger le plan vélo de vélorution : <a href="/diaporama1.pdf" download="">Diaporama 1</a> , <a href="/diaporama2.pdf" download="">Diaporama 2</a> , <a href="/diaporama3.pdf" download="">Diaporama 3</a>
        </p>
        <br>
        
         <h2>Les communiqués de presse de Vélorution</h2>
        <br>
        <br>
        <p>
            Télécharger les communiqués de presse : <a href="/Etat des pistes.pdf" download="">Etat des pistes </a> , <a href="/Note sur panneaux stop.pdf" download="">Note sur panneaux stop</a> , <a href="/Occupations irrégulières de pistes et bandes cyclables" download="">Occupations irrégulières de pistes et bandes cyclables</a>
        </p>
        <br>
        <br>
        <br>
        <br>
        <br>
        <br>
     </div>

      


</div> 
    </div>

</template>


<script>
    export default {

    }
</script>

<style scoped>
h1 {
  font-family: 'Lato', sans-serif;
  color:black;
  font-size: 2em;
  font-weight:bold; 
}

h2 {
  font-family: 'Lato', sans-serif;
  color:black;
  font-size: 1.5em;
  font-weight:bold; 
}

.wrapper-passerelle {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}
.one-passerelle {
    grid-area: 1 / 1 / 3 / 3;
    width: 96%;
}
.two-passerelle {
    grid-area: 1 / 3 / 2 / 5;
    margin-left: 5px;
    justify-content: center;
}
.three-passerelle {
    grid-area: 2 / 3 / 3 / 4;
    margin-left: 5px;
}
.four-passerelle {
    grid-area: 2 / 4 / 3 / 5;
    margin-left: 5px;
}
.five-passerelle {
    grid-area: 2 / 5 / 3 / 6; 
    margin-left: 5px;
}

.wrapper-gare {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(5, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}
.one-gare {
    grid-area: 1 / 1 / 3 / 3;
    width: 96%;
}
.two-gare {
    grid-area: 1 / 3 / 2 / 5;
    margin-left: 5px;
}
.three-gare {
    grid-area: 2 / 3 / 3 / 4;
    margin-left: 5px;
}
.four-gare {
    grid-area: 2 / 4 / 3 / 5;
    margin-left: 5px;
}
.five-gare {
    grid-area: 1 / 5 / 3 / 6;
    margin-left: 5px;
}

.wrapper-paris {
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(5, 1fr);
    grid-column-gap: 0px;
    grid-row-gap: 0px;
}
.one-paris {
    grid-area: 1 / 1 / 3 / 3;
    width: 96%;
}
.two-paris {
    grid-area: 1 / 3 / 2 / 5;
    margin-left: 5px;
}
.three-paris {
    grid-area: 2 / 3 / 3 / 4;
    margin-left: 5px;
}
.four-paris {
    grid-area: 2 / 4 / 3 / 5;
    margin-left: 5px;
}
.five-paris {
    grid-area: 1 / 5 / 3 / 6;
    margin-left: 5px;
}


</style>
