# kata_pizza

## Mission

Vous allez diner dans une pizzeria avec des amis. Au moment de l’addition, vous vous rendez compte que les 4 pizzaïolos ont chacun leur façon de déterminer le prix d’une pizza ! LE but du kata est ici de déterminer le prix de l'addition.
<br>

## Règles 

Voici les données brutes dont vous aurez besoin, sachant que pous pouvez modifier le format de ces données comme vous voulez.

+ **Variable ingrédients** : comprend tous les  ingrédients disponibles avec leur prix en €, sous le format : « ingredient:prix ».

``$ingredients = ['tomates:1', 'champignons:3', 'mozzarella:3', 'jambon:2', 'serrano:4', 'chevre:2', 'oeuf:2', 'chorizo:5', 'saumon:5', 'basilic:2', 'oignons:2', 'poivron:1', 'salade:1', 'anchois:2', 'olive:3', 'ananas:5'];``

<br>

+ **Variable $pizzas** : contient toutes les pizzas préparées. Une pizza est représentée par une liste d’ingrédients, chacun séparé par une virgule (,).

``$pizzas = ['poivron,ananas,poivron,tomates', 'salade,mozzarella,salade,champignons,chevre', 'serrano,basilic,tomates,jambon,basilic', 'champignons,serrano,jambon', 'tomates,oeuf,serrano,champignons', 'olive,oeuf,tomates,poivron', 'olive,salade,ananas', 'chevre,ananas,salade,chevre', 'chevre,anchois,tomates,ananas,oeuf,olive', 'salade,mozzarella,basilic,salade,oignons', 'poivron,serrano,jambon', 'ananas,tomates,champignons,ananas,olive', 'chevre,chevre,tomates,saumon,poivron'];``

<br>

+ **Variable $pizzaiolo** : donne l’ordre dans lequel les pizzaiolos réalisent et chiffrent donc les pizzas.

``$pizzaiolos = ['donatello', 'raphael', 'michelangelo', 'leonardo', 'michelangelo', 'leonardo', 'donatello', 'raphael', 'donatello', 'raphael', 'raphael', 'raphael', 'donatello'];``

<br>

La première pizza de la variable pizza est réalisé par le premier nom de la variable pizzaiolos, et ainsi du suite.

**Voici comment chacun d'entre eux chiffre les pizzas :**
+ *Léonardo* : il ajoute simplement le prix de chaque ingrédient
+ *Donatello* : il prend l’ingrédient le plus cher et multiplie par 5
+ *Michelangelo* : il prend la somme des 2 ingrédients les plus chers, et multiplie par 3
+ *Raphaël* : il commence à 10€, ajoute le prix de l’ingrédient le moins cher et le prix de l’ingrédient le plus cher

## But
+ Determiner le montant total de l’addition, c’est à dire la somme des prix de chaque pizza.
+ Respect des principes SOLID (https://alexsoyes.com/solid/) et KISS

## Temps 
Vous avez 30 minutes, bon courage ! :)
