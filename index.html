<html>
<head>

    <title>Jeu v01 - Jeu du pendu Wersten (exercice javascript)</title>
		<meta charset="utf-8" />		
		<meta name="description" content="Jeu du pendu version wersten, exercice apprenant en javascript">
		<meta name="keywords" content="Javascript, js, tutoriel">
		<meta name="robots" content="ALL">
		<meta name="distribution" content="Global">
		<meta name="copyright" content="Emmanuel Trépant">
		<meta name="author" content="Emmanuel Trépant">
		<meta name="language" content="Fr">
		<meta name="doc-type" content="Public">
		<meta name="doc-class" content="Complet">
		<meta name="doc-rights" content="Domaine public">
		<meta name="DateCreated" content="30/10/2020">
		<meta property="og:title" content="Jeu du pendu western" />
		<meta property="og:description" content="Jeu de pendu version Western - Exercice apprentisage javascript" />
		<meta property="og:url" content="https://www.trepant.be/cv" />		
		<meta name="viewport" content="width=device-width, initial-scale=1" />		
		<link rel="apple-touch-icon" href="apple-touch-icon-iphone.png" />
		<link rel="apple-touch-icon" sizes="72x72" href="apple-touch-icon-ipad.png" />
		<link rel="apple-touch-icon" sizes="114x114" href="apple-touch-icon-iphone-retina-display.png" />
        <link rel="icon" href="favicon.ico" />
        <link href="https://fonts.googleapis.com/css2?family=Acme&display=swap" rel="stylesheet">
        <link rel="stylesheet" type="text/css" href="reset.css"/>

  <style>

    html {
        font-family: 'Acme', sans-serif;
        }

    body{
        overflow-x: hidden;
        background-image: url("fond.jpg");
        background-position: center;
        background-color: white;
        margin: 0 10px;    
        }

    div {display: inline-block;}

    #message{
                font-size: 40px;
                color: #7c8553;
                text-align: center;
                width: 100%;
                padding: 10px;
                font-family: 'Acme', sans-serif;
      }

h3{
    padding: 4px;
    font-size: 16px;
}

    #lettreDejaTapee{
            
                color:black;
                width: 100%;
                height: 20px;
                text-align: center;
                font-family: 'Acme', sans-serif;
                font-size: 18px;       
            }


    button{
                border : 1px solid grey;
                padding: 10px;
                font-size: 14px;
                background-color: rgb(11, 18, 51);
                color: white;
            }

    #containerMonClavier{
                position: relative;
                z-index: 1;
                top:10px;
                box-shadow: 4px 4px black;
                max-width: 640px;
                display: block;
                margin: auto;
                padding: 10px 0;
                align-items: center;
                justify-content: center;
                text-align: center;
                border-radius: 8px;
                border: 1px solid black;
                background-color: rgba(168, 121, 82, 0.3);      
            }

    button{
                margin: 4px;
                font-family: 'Acme', sans-serif;
        }


    #lettre{
                display: block;
                display: none;
                color: white;
                max-width: 640px;
                margin: auto;
                align-items: center;
                justify-content: center;
                text-align: center;     
        }

    .case{
                padding: 4px;
                margin-right: 4px;
                border: 5px solid black;
                min-height: 20px;
                min-width: 20px;
                background-color: white;
                text-align: center;
    }


    #mesLettres{
                padding: 5px;
    }
        

    #inputB{
                padding: 10px;
                display: block;
                text-align: center;
                position: relative;
                top: 30px;
        }

    #divLettreEcran{
                width: 100%;
                text-align: center;
                position: absolute;
                top:100px;
                z-index: 0;
    }

    #illustration{
                height: 300px;
                width: 100%;
                background-image: url("0.png");
                background-position: center;
                background-repeat: no-repeat;
        }

    .boutonEnvoyer{
                font-family: 'Acme', sans-serif;
                font-size: 16px;
                box-shadow: 4px 4px black;
                border-radius: 5px;
    }



    @media only screen and (max-width:660px) {


        div#message {
            font-size: 30px;
        }

        div#illustration {
            height: 250px;
            background-size: 250px 250px;
            top: -50px;
        }

        #containerMonClavier{
            top : -30px
        }

        input.boutonEnvoyer{
            position: relative;
            top : -30px;
        }

        .case{
            padding: 3px;
            margin-right: 3px;
            border: 2px solid black;
            min-height: 15px;
            min-width: 15px;
        }

    }
 
 
  </style>

</head>
<body>

<!-- info -->
<div id="message">Trouve le nom d'un pays</div>

<div id="divLettreEcran"></div> 

<!-- info écran lettre tapée -->
<div id="lettreDejaTapee">Gringo, trouve le mot avant que je tire !</div>

<!-- Lettre tapée à l'écran -->
<div id="lettre"></div>

<!-- images à l'écran -->
<div id="illustration"></div>

<!-- zone clavier -->
<div id="containerMonClavier"></div>

<!-- Mot entier recherché (admin) -->
<!-- <div id="mot"></div> -->


<script>

// Mémoriser bonnes lettres
        let compteurLettresOk = [];

// Mémoriser les lettres tapées
        const lettreDejaTapee=[];

// Essais (étapes 6 images)
        const essais =  6;

// Difficulté (0) défaut / + (facile) / - (difficile)
        const difficulte = 0;

// Décompte générale (6 essais + nombre de lettres maximum du mot)
        let decompteGameOver = 0;

// Décompte pour affichage illustration
        let decompte=0;

 // Game Over après x tentatives
        let monCompteur = 0;

 // Initialisation paramètre pour effacer complétement le clavier du DOM
        let b = document.body;
        let cibleAeffacer = document.getElementById('containerMonClavier');

 // Selection du div image à modifier en fonction du nombre d'essais
  const imageEssais= document.querySelector("#illustration");

// -----------------------------------------------------------------------------------------------

// Preload Images étapes Cowboy


let images =["0.png","1.png","2.png","3.png","4.png","5.png","6.png","7.png"]

function preload(imageArray, index) {
        index = index || 0; // index = index OU 0
        if (imageArray && imageArray.length > index) {
            let img = new Image ();
            img.onload = function() {
                preload(imageArray, index + 1);
            }
            img.src = images[index];
}}
/* images is an array with image metadata */
preload(images);

// -----------------------------------------------------------------------------------------------



// Liste des mots
        const mots = [

"Afghanistan","Albanie","Algerie","Allemagne","Andorre","Angola","Anguilla","Argentine","Armenie","Aruba","Australie","Autriche","Azerbaidjan","Bahamas",
"Bahrein","Bangladesh","Barbade","Belgique","Belize","Benin",
"Bermudes","Bhoutan","Bielorussie",
"Birmanie","Bolivie",
"Botswana","Bresil","Brunei",
"Bulgarie","Burkina","Faso","Burundi",
"Cambodge","Cameroun","Canada","Chili","Chine",
"Chypre","Colombie","Comores","Croatie","Cuba",
"Danemark","Djibouti","Dominique",
"egypte","emirats","Arabes","Unis","equateur",
"erythree","Espagne","Estonie","ethiopie",
"Fidji","Finlande","France",
"Gabon","Gambie","Georgie",
"Ghana","Gibraltar",
"Grece","Grenade","Groenland",
"Guadeloupe","Guatemala",
"Guinee","Guinee","equatoriale",
"Guyana","Guyane","Française","Haiti",
"Honduras","Hongrie",
"Iran","Iraq","Irlande",
"Islande","Israel","Italie",
"Jamaique","Japon","Jordanie",
"Kenya",
"Koweit","Laos",
"Lesotho","Lettonie",
"Liban","Liberia","Libye",
"Liechtenstein","Lituanie","Luxembourg",
"Macao","Madagascar","Malaisie",
"Malawi","Maldives","Mali",
"Malte","Maroc","Martinique",
"Maurice","Mauritanie","Mayotte",
"Mexique","Moldavie","Monaco",
"Mongolie","Montenegro","Montserrat",
"Mozambique","Namibie","Nauru",
"Nepal","Nicaragua","Niger",
"Nigeria","Norvege",
"Oman",
"Ouganda","Ouzbekistan","Pakistan",
"Panama",
"Paraguay","Hollande","Perou",
"Philippines","Pologne",
"Portugal","Qatar",
"Roumanie","Royaume-Uni",
"Russie","Rwanda",
"Senegal","Serbie",
"Seychelles","Singapour",
"Slovaquie","Slovenie","Somalie",
"Soudan","Suede",
"Suisse","Suriname",
"Swaziland","Syrie","Tadjikistan",
"Taiwan","Tanzanie","Tchad",
"Thailande",
"Tunisie","Turquie","Ukraine","Uruguay",
"Venezuela",
"Yemen","Zambie",
"Zimbabwe"];

// console.log(mots)


// Choix au hasard du mot : random sur x entrées qui est le nombre d'entrées du tableau mot
        const random = Math.floor(Math.random() * mots.length); // 0 à nombre de mots
        // Random est le numero choisit ex: 1 devient mot[1]
        // console.log(random+" num. DataBase / ", mots[random]);


// DOM - mot à trouver en HTML
        // document.getElementById("mot").innerHTML = "Le mot à trouver  : " + mots[random];


// Nombre de caractères du mot à trouver exemple : maison = 6
        const nbreCaractere = `${mots[random].length}`;
        // console.log(nbreCaractere + "= Nombre de lettres");


// Mon mot à jouer mise en variable monMotAJouer
        let monMotAJouer = mots[random];

// Capitaliser les mots car la recherche des lettres se fait sur des lettres capitale
        monMotAJouer=monMotAJouer.toUpperCase()
        // console.log(monMotAJouer);

        // console.log(monMotAJouer + " = le mot à jouer !");
        // creation loop des div - par défaut

        // Pointer div pour coller les lettres du jeu 
        var varPointageCible=document.getElementById("divLettreEcran");
        // let target = document.getElementById("#target");
        // console.log(target)


                  for (let i = 0; i < nbreCaractere; i++) {

                    // console.log(i + " = incrément");
                    // Attention ça ajoute le div dans la DOM au dessus des précédents donc 5,4,3...

                    // creation DIV 
                    let divLettres = document.createElement("div");
                    
                    // ajout id + incrementation (c01,c02 ...)
                    divLettres.setAttribute("id","c0"+i);

                    // ajout de class pour le design css
                    divLettres.setAttribute("class","case");

                    // création du contenu - par défaut
                    let monContenu = document.createTextNode(' - '); 

                    // attacher le noeud monContenu à divLettres
                    divLettres.appendChild(monContenu);
                  
                    // Attacher l'ensemble des div à un conteneur
                    varPointageCible.appendChild(divLettres);
                    document.body.appendChild(varPointageCible);

                }

// -----------------------------------------------------------------------------------------------
// script recupérer info du clic id du bouton

function recupId(monId){

            // monId sert à appeller et y joindre id
            monId=monId.id;
            console.log(monId + " MON ID");

            // Remplir mon div lettre tapée
            document.getElementById("lettre").innerHTML = "Lettre tapée : " + monId;

            // console.log(monMotAJouer) 
            
            // enregistrer les lettres tapées checker 
            const memo = lettreDejaTapee.push(monId);
            // console.log(lettreDejaTapee + "--> Lettre tapée");

            document.getElementById("lettreDejaTapee").innerHTML = "Lettre(s) déjà tapées  : " + lettreDejaTapee;

            // Désactiver les boutons des lettres tapées


// ******************************************************** 
        
                // Loop for désactiver les boutons à l'id déjà tapé
                // <button type="button" disabled>Click Me!</button>

        function desacTBoutonTape(){

                document.getElementById(monId).disabled = true;
                document.getElementById(monId).style.opacity = "0.3";

               }
               desacTBoutonTape()

// ******************************************************** 

        console.log(lettreDejaTapee + "= lettre tapée")


            // monCompteur d'essais
            monCompteur= monCompteur + 1;
            // console.log(monCompteur)
            
// -----------------------------------------------------------------------------------------------

            function verifierLettreMot ()
              {
                      let lettreRecherchee = monId; // id de la lettre cliquée

                      // Recherche lettre tapée, lettre(s) du mots
                      // Recherche doublons

                      function fonctionRechercheLettre(){

                                let lettreRecherchee = monId;

                                    for (var i = 0; i <= monMotAJouer.length; i++) {

                                        // charAt = chercher une lettre

                                        if (monMotAJouer.charAt(i) == lettreRecherchee) {
                                            // console.log(i + " < ---- Lettre ou doublon  /  " + lettreRecherchee + " <--- Lettre"); 
                                            
                                            let winFinal = compteurLettresOk.push(i);
                                            console.log(winFinal + " Lettre(s) valide(s)")

                                        // Sélection et remplir le div avec la lettre trouvée
                                        // console.log("id du Div à chercher ==> "+ i);
                                        document.getElementById("c0"+i).innerHTML = monId;

                                       // Compte les lettres validées (utile pour le message GAGNE)

                                          } // fin de if OK

                                          } // fin de for
                      }

                      // Appel fonction
                      fonctionRechercheLettre()
                    }

                    verifierLettreMot ()


// -----------------------------------------------------------------------------------------------
// GAGNE

              function checkSiGagne(){

                    if(compteurLettresOk.length!=monMotAJouer.length){
                      console.log(monMotAJouer.length + " Length du mot à jouer / "+compteurLettresOk+" Lettres valides ("+compteurLettresOk.length+")");
                    }

                    else { // si nombre de lettres validées est égal à la longueur du mot choisit
                      
                    // console.log("GAGNE");

                    // afficher le message WIN
                    const message = document.querySelector("#message");
                    message.style.color="green";
                    // message.style.fontSize="40px";
                    message.style.textAlign ="center";
                    message.innerHTML=" Gagné Gringo !"
  
                    // Cacher le container contenant le clavier
                    document.getElementById("containerMonClavier").style.display = "none";
                    document.getElementById("lettreDejaTapee").style.display = "none";
                    document.getElementById("divLettreEcran").style.display = "none";
                    

                  // Efface du DOM mon clavier (pas utile car déjà invisible) 
                    let effaceDuDom = b.removeChild(cibleAeffacer); 
                    
                    // Image gagné
                    imageEssais.style.backgroundImage = "url('7.png')";

                    }
              }
                    checkSiGagne()

// -----------------------------------------------------------------------------------------------

            function nombreEssais() // Essais + Game Over
                {
                
                // 6 lettres + 6 essais = 12
                // + difficultés

                        const essaiMax =  parseInt(nbreCaractere) + essais + difficulte; // difficultés augmentée 
                        console.log(essaiMax + " = Nbre essais max");
                        console.log(monCompteur + " = Compteur +");

                        //decompteGameOver = 12 - 6 - (0, -1, -2);
                        decompteGameOver = (essaiMax - essais) - decompte;
                        
// -----------------------------------------------------------------------------------------------

        // Décompte pour affichage du cowboy

                                if(monCompteur > essaiMax - essais){
                                        
                                        decompte = decompte - 1;
                                        decompteGameOver = decompteGameOver-1;
                                        console.log(decompte + "= Decompte");      
                                }

// -----------------------------------------------------------------------------------------------

        // changement image en fonction du nombre d'essais

        // Nom de l'image (x.png)
        let imageVar = (decompte*-1)+".png";
 
// -----------------------------------------------------------------------------------------------  
        

        function image(){

            // Si pas gagné alors affiché image
            if(compteurLettresOk.length!=monMotAJouer.length){
            imageEssais.style.backgroundImage = "url("+imageVar+")";
            }

            // Si gagné
            if(monCompteur == essaiMax){
                imageEssais.style.backgroundImage = "url('7.png')";
            }
        }
                switch(decompte) {

                        case -1 :
                        image();
                        break;

                        case -2:
                        image();
                        break;

                        case -3:
                        image()
                        break;

                        case -4:
                        image()
                        break;

                        case -5:
                        image()
                        break;

                        case -6:
                        image()
                        break;

                        case -7:
                        image()
                        break;

                        default:
                            if(compteurLettresOk.length==monMotAJouer.length){
                                imageEssais.style.backgroundImage = "url('7.png')";
                            }
                        }


    // GAME OVER ---------------------------------------------------------------------------------------------


                        // Quand le nombre essais est atteint
                        if(monCompteur == essaiMax){


                        //  Image perdu
                        // imageEssais.style.backgroundImage = "url('6.png')";
                        image()

                        console.log(" --------- GAME OVER  --------- le mot à trouver était "+ monMotAJouer);

                        // Cacher le container contenant le clavier
                        document.getElementById("containerMonClavier").style.display = "none";

                        // Efface du DOM mon clavier (pas utile car déjà invisible) 
                        let effaceDuDom = b.removeChild(cibleAeffacer);

                        // Désactiver les lettres tapées et lettres affichées du jeu
                        document.getElementById("lettreDejaTapee").style.display = "none";
                        document.getElementById("divLettreEcran").style.display = "none";
                        

                        // afficher le message Game Over
                        const message = document.querySelector("#message");
                        message.style.color="red";
                        // message.style.fontSize="40px";
                        message.style.textAlign ="center";
                        message.innerHTML="Perdu Gringo ! <h3>Le mot à trouver était " + monMotAJouer +"</h3>";
                        imageEssais.style.backgroundImage = "url('6.png')";

                        }

                }
                // Appel nombre essais
                nombreEssais(nbreCaractere)  


// -----------------------------------------------------------------------------------------------


          } // FIN DE FONCTION AU CLIC

                function createButtons(){

                          // Création des boutons Alphabet
                          const alphabet = ["-","A","B","C","D","E","F","G","H","I","J","K","L","M","N","O","P","Q","R","S","T","U","V","W","X","Y","Z"];
                          const longueurTableauAlphabet = alphabet.length; // 26


                            for (let i = 0; i < longueurTableauAlphabet; i++) {
                              // Boucle de 26
                              // console.log(alphabet[i]); 

                              let monBouton = document.createElement("button"); //<button></button>
                                monBouton.id = alphabet[i]; // id="a"

                                // Ajouter à mon bouton un script (attribute)
                                monBouton.setAttribute("onclick", "recupId(this)");
                                monBouton.textContent = `${alphabet[i]}` // <button id="a">a</button>


                                // ajouter dans un tableau les lettres déjà tapées
                                // lettreDejaTapee

                                document.getElementById("containerMonClavier").appendChild(monBouton); // créer dans le Div de id="container" 
                          }
                    }

                  // Appel fonction
                  createButtons()

                  // console.log(document.body)

</script>

<div id="inputB">
    <input class="boutonEnvoyer" type="button" value = "Choisir un nouveau mot" onclick="history.go(0)" />
</div>


</body>
</html>


