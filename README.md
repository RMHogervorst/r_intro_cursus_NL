# Leerdoelen voor een R intro cursus in 1 of 2 dagdelen

author: "Roel M. Hogervorst"
date: "February 26, 2018"

# algemeen
Deze leerdoelen zijn bedoeld voor een superkorte intro. Ik wil de kandidaten zo snel mogelijk aan het coden krijgen. 
Je moet snel succes hebben. 

Leren van R en tidyverse bestaat uit 4 delen:

* Begrijpen hoe rstudio in elkaar zit
* begrijpen hoe wat het dataframe is
* ggplot2: begrijpen hoe je een plot uit lagen opbouwt
* dplyr: muteren, selecteren filteren en groeperen van data

## Hoe zitten R en RStudio in elkaar

#### algemeen over de taal
- Je weet dat R de taal is, en RStudio een omgeving om makkelijk met R te werken
- Je weet R hoofdlettergevoelig is, View is niet hetzelfde als view
- een functie heeft een naam en dan haakjes, je stopt data en argumenten in de haakjes `sum()`
- je weet hoe je met vraagteken de help van een functie kunt vinden
- om dingen in het geheugen te zetten wijs je ze toe met een '<-' pijltje
- dingen in R veranderen niet tenzij je ze toewijst aan dezelfde naam


#### Rstudio 
- Je kunt een dataset bekijken met de Viewer
- je weet waar de code wordt uitgevoerd
- je weet waar scripts staan
- je weet waar je kunt vinden welke objecten actief in het geheugen zijn
- je weet waar je de inhoud van de projectmap kunt vinden
- je kunt het laatste plot openen

## Hoe werken we met data in R

- je weet dat een data frame een soort excel in het geheugen is
- je weet dat bij voorkeur data georganiseerd is in rijen en kolommen
- je kunt de eerste en laatste regels van een data frame naar de console printen
- Je hebt een idee van hoe je een extern bestand kunt inladen als een data-frame
- kolommen in een data frame zijn karakters (character) numeriek (numeric) of anders

## werken met ggplot2

- vanwege historische redenen zijn er meerdere manieren om te plotten in R
- een plot bestaat uit een grondlaag en meerdere lagen die met '+' samen worden genomen
- je verteld ggplot2 hoe de kolommen uit de data moeten worden vertaald naar een figuur (op een as, naar een kleur, naar een vorm, etc)
- deze mapping doe je met aes() wat staat voor aesthetics
- plots zijn in te delen naar soort, per soort is er een geom_* 
- je bouwt plots op door laag voor laag te werken (haal een gedeelte weg, als je niet meer uitkomt)
- je werkt iteratief, probeer, verander, probeer opnieuw
- je kunt data opsplitsen en apart plotten met facet_* functies


## werken met dplyr

- alle functies in dplyr doen 1 ding, en 1 ding goed
- je combineert de kleine functies om een groter doel te bereiken
- je kunt verschillende functies combineren met de pipe ` %>% `
- dplyr lijkt veel op sql, maar je hoeft geen ; te gebruiken
- je selecteerd kolommen met select
- je filtered rijen met filter
- je maakt nieuwe kolommen met mutate
- je kunt je dataset opdelen in groepen en bewerkingen per groep uitvoeren met group_by 
- summarize doet een bewerking op de groep en geeft het resultaat per groep
- een veel gebruikt patroon is split-apply-combine: je groepeert ergens op, bewerkt elke groep en combineert het eindresultaat


# Bronnen en verder lezen

* http://third-bit.com/teaching/  "Geweldig goed doordacht boek van Greg Wilson over hoe je iemand het effectiefst leert programmeren"
* https://swcarpentry.github.io/r-novice-gapminder/13-dplyr/ "software carpentry voorbeeldles over dplyr"
