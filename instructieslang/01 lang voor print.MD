# HTML workshop


## wat we gaan maken:

![einddoel.PNG](img/einddoel.PNG)

## Press START!

open de volgende link in je browser:

https://codepen.io/pen/

## Html

Op de pagina zie je het volgende:

![htmlwindow.PNG](img/htmlwindow.PNG)

Dat is waar we onze `HTML` code gaan typen

## Basis html

type de volgende code in het `HTML` window


![htmltag.PNG](img/htmltag.PNG)

## Resultaat

Je ziet nog niets.
Dat klopt!

We hebben nog geen tekst, kleur en plaatjes toegevoegd



# Poke blok

We gaan verder, we gaan nu blokjes maken voor de pokemon


## Opzetten van het blok

type de volgende code in het `HTML` window


![pokeblok.PNG](img/pokeblok.PNG)

## Resultaat

nu zien we tekst:

![pokeblokresult1.PNG](img/pokeblokresult1.PNG)

## plaatje voorbereiden

Nu het plaatje, in de `figure` tag gaan we typen:


![pokeblok2.PNG](img/pokeblok2.PNG)

## het plaatje laden

in `src=""` gaan we nu een link plaatsen:

`https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/387.png`

die zet je tussen de `src="HIER KOMT DE LINK"`

## Resultaat


![pokeblokresult2.PNG](img/pokeblokresult2.PNG)

# Pokestyle

Het is nog vrij stijlloos, laten we dat aanpakken!

## Opzetten van het blok

we gaan nu stijl aangeven, dat doen we in het `CSS` window


![css.PNG](img/css.PNG)

## Background maken

We willen een poke-ball achtige achtergrond, dus rood-wit

in het `CSS` window type je:



![css1.PNG](img/css1.PNG)

## Resultaat

nu krijg je ongeveer dit te zien:

![cssresult1.PNG](img/cssresult1.PNG)

## het blokje

nu nog het blokje, we geven deze:
- een achtergrond kleur
- een hoogte & breedte
- een shaduw


in het `CSS` window type je:

![css2.PNG](img/css2.PNG)

- Zie jij welke wat doet?

## Resultaat

![cssresult2.PNG](img/cssresult2.PNG)

## Grass

De grass tekst staat nog niet mooi, we beginnen met een hoogte 


in het `CSS` window type je:

![css3.PNG](img/css3.PNG)

### Result

![cssresult3.PNG](img/cssresult3.PNG)

## Center

in het `CSS` window type je:

![css4.PNG](img/css4.PNG)

De tekst komt in het midden te staan door:
- `justify-content: center;`
- `align-items: center;`

### Result

![cssresult4.PNG](img/cssresult4.PNG)

## nu het plaatje nog

maak nu in het `CSS` window een nieuw blok aan voor `figure`
vergeet je `{` en `}` niet

binnen de `{` en `}` zetten we onze stijl.
Hier gaan we dezelfde properties gebruiken :
- height: 70%;
- display: flex;
- justify-content: center;
- align-items: center;

Die 70% is dus de rest van de 100% van het `article`

probeer dit zelf!
- kijk naar de andere code

lukt het niet? kijk hieronder

<details>
<summary>Code oplossing</summary>

![plaatjeoplossing.PNG](img/plaatjeoplossing.PNG)

</details>

## Result

nu hebben we 1 blok af

![cssresult5.PNG](img/cssresult5.PNG)
# 3 starters

Nu hebben we maar 1 starter
Laten we er meer maken

## Opzetten van het blok

kopieer het `article` en plak deze `2` keer zodat je dit krijgt:

![starters1.PNG](img/starters1.PNG)


## Onder elkaar?

Ze komen onder elkaar...
we willen ze naast elkaar!

Hoe doen we dat?
- `display: flex;`

Deze zetten we op de `body` in het `CSS` window


![naast.PNG](img/naast.PNG)

probeer het zelf, lukt het niet? kijk hieronder

<details>
<summary>Code oplossing</summary>

![naastcode.PNG](img/naastcode.PNG)

</details>

## Ruimte!

Nu staan ze op elkaar, even wat ruimte
Dit doen we weer op de `body` in het `CSS` window 

gebruik
- `gap: 20px;`

<details>
<summary>Code oplossing</summary>

![gap.PNG](img/gap.PNG)

</details>

## Resultaat

dan zien we dit:

![gapped.PNG](img/gapped.PNG)

## Andere pokemon

Verander het tweede en derde blok zodat je andere pokemon hebt

- Water: `https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/393.png`
- Fire `https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/390.png`

## Resultaat
![gapped.PNG](img/gapped.PNG)

# interactie

Laten we nu wat interactie maken

## Interactie met CSS

Deze zetten we op de `article` in het `CSS` window
- `transition: 0.2s;`

Dit is de `animatie` snelheid in secondes. Pas die maar aan!

![transition2.PNG](img/transition2.PNG)

En we voegen dit toe in het `CSS` window

![transition.PNG](img/transition.PNG)


## javascript

nu gaan we het `spel` beginnen ^.^
plak deze code in het `JS` window
```
    function chooseYou(article)
    {
        console.log(article);
        window.open( 'https://www.youtube.com/watch?v=af_SqTbt3yc','_blank');
    }


    var articles=document.getElementsByTagName('article')
    for(let i =0; i< articles.length; i++)
    {
        console.log(articles[i]);
        articles[i].addEventListener('click',chooseYou);
    }
```
