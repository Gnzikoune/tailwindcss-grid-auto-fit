# Grid auto fit (grilles responsives automatique) avec Tailwind CSS

Voici un plugin qui vous aidera à créer des grilles responsives de manière automatique, sans utiliser les médias queries.
Il est constituer de propriétés css telles que 'auto-fit' et 'grid-template-columns' afin de vous aider au mieux dans la conceptions 
de grilles responsives.

## Installation

Vous pouvez l'installer dans un nouveau projet, ou un autre déjà existant:

----------------------------------------------------------------

npm install -D @gnzikoune/tailwindcss-grid-auto-fit

----------------------------------------------------------------

Ensuite, ajoutez le plugin à votre fichier de configuration 'tailwind.config.js'

----------------------------------------------------------------
module.exports = {
    theme: {

    },
    plugins: [
        require('@gnzikoune/tailwindcss-grid-auto-fit'),
    ],
}

-----------------------------------------------------------------


### Usage 

Utilisez les classes 'grid-auto-fit' avec au préalable la classe 'grid'
afin de créer des grilles responsives.


-------------------------------------------------------------------

<section class="grid grid-auto-fit gap-2 ">
   <div class="p-6 bg-blue-400 rounded-md">
      Grille 1
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 2
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 3
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 4
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 5
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 6
   </div>
   <div class="p-6 bg-yellow-400 rounded-md">
      Grille 7
   </div>
</section>

-------------------------------------------------------------------



#### Classes utilitaires pour rendre vos grilles responsives

Utilisez les utilitaires tels que '.grid-auto-fit-xs', '.grid-auto-fit-xl' afin de changer la taille responsive minimum et maximum des grilles. Ce plugin inclut 6 tailles par défault en fonction des différentes tailles d'écran. La taille minimum par défaut est de 16rem.


| Classes                               | Tailles            |
| ------------------------------------- | ------------------ |
| 'grid-auto-fit-xs'                    | '12rem'            |
| 'grid-auto-fit-sm'                    | '14rem'            |
| 'grid-auto-fit' ou 'grid-auto-fit-md' | '16rem'            |
| 'grid-auto-fit-lg'                    | '18rem'            |
| 'grid-auto-fit-xl'                    | '20rem'            |
| 'grid-auto-fit-2xl'                   | '22rem'            |


##### Valeurs arbitraires

Ce plugin supporte également l'utilisation de valeurs arbitraires si vous voulez bien évidemment personnaliser la taille de vos différents éléments.

-------------------------------------------------------------------
<section class="grid grid-auto-fit-[13rem]">
   ...
</section>
-------------------------------------------------------------------



NB: Vous pouvez bien évidemment télécharger le code source du plugin et bien sur l'upgrader en fonction de l'évolution du framework Tailwind CSS.




<!-- Merci à Cyberschool Entrepreunariat  -->

<!-- Gildas Nzikouné  -->
<!-- Dev Front-End -->
