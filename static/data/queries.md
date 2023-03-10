# The semantics

## The semiotics of suits in numeral cards

The first four queries present significant results for the study of the semiotics of tarot suits. With regard to the suit of Wands, the largest percentage shows that the reference is to the forest and, in general, to the forest setting of *Il Castello*. In those cases where the semantics deviates from the setting, it emerges that it is the number that defines the meaning of the card: the *Due di Bastoni* is, in fact, used to express a duality or a choice between two situations (fourth story of *Tutte le altre storie*) regardless of the suit; the *Asso di Bastoni*, on the other hand, may refer not only to the tree, but also to power and its material symbol (third story of *Tutte le altre storie*). Unlike numerals with the suit of Wands, those of Coins refer, instead, to two clearly opposite semantic fields: the first is that of earthly power, wealth and materiality (e.g. richness, inheritance, money); the second, on the other hand, has to do with heaven, the divine and the immaterial (e.g. light, moon, state of beatitude). Between the two semantic fields, however, the former stands out over the latter. The largest percentage of the results obtained for the semantics of numerals with the seed of Swords pertain to themes of warfare (e.g. war, duel, dispute); sometimes, it specifically refers to defence (e.g. barrier, guards). Finally, the semantic meaning associated with the suit of Cups is less clearly defined than the three aforementioned suits. From the results, it is possible to note a large percentage that refers to banqueting and refreshment (e.g. banquet, wedding banquet, tavern); there are, however, other references such as those related to wealth (e.g. the source of life, world peace) or to love (e.g. love encounter).

### Wands

What are the meanings associated with cards that have suit Wands?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit bacodi:bastoni.
    ?cardDeck odi:hasTypology bacodi:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |         cardDeck        |            meaning            |
|----|-------------------------|-------------------------------|
|  1 | bacodi:due-di-bastoni    | bacodi:necessit??-di-una-scelta |
|  2 | bacodi:due-di-bastoni    | bacodi:vittoria-altro-su-uno   |
|  3 | bacodi:due-di-bastoni    | bacodi:necessit??-di-una-scelta |
|  4 | bacodi:due-di-bastoni    | bacodi:due-bastoni             |
|  5 | bacodi:asso-di-bastoni   | bacodi:scettro                 |
|  6 | bacodi:asso-di-bastoni   | bacodi:tronco                  |
|  7 | bacodi:cinque-di-bastoni | bacodi:vista-del-massacro      |
|  8 | bacodi:cinque-di-bastoni | bacodi:schianto-dei-tronchi    |
|  9 | bacodi:cinque-di-bastoni | bacodi:bosco                   |
| 10 | bacodi:dieci-di-bastoni  | bacodi:bosco                   |

### Coins

What are the meanings associated with cards that have suit Coins?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit bacodi:denari.
    ?cardDeck odi:hasTypology bacodi:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |         cardDeck        |               meaning              |
|----|-------------------------|------------------------------------|
|  1 | bacodi:asso-di-denari   | bacodi:elemosina                   |
|  2 | bacodi:asso-di-denari   | bacodi:luna                        |
|  3 | bacodi:cinque-di-denari | bacodi:luce-del-mattino            |
|  4 | bacodi:cinque-di-denari | bacodi:spreco                      |
|  5 | bacodi:dieci-di-denari  | bacodi:et??-dello-oro               |
|  6 | bacodi:dieci-di-denari  | bacodi:pagamento-per-uno-scherano  |
|  7 | bacodi:dieci-di-denari  | bacodi:ricchezza                   |
|  8 | bacodi:dieci-di-denari  | bacodi:eredit??                     |
|  9 | bacodi:due-di-denari    | bacodi:due-denari                  |
| 10 | bacodi:due-di-denari    | bacodi:dualit??-del-bene-e-del-male |

### Swords

What are the meanings associated with cards that have suit Swords?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit bacodi:spade.
    ?cardDeck odi:hasTypology bacodi:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |        cardDeck       |                    meaning                    |
|----|-----------------------|-----------------------------------------------|
|  1 | bacodi:asso-di-spade  | bacodi:volont??-divina                         |
|  2 | bacodi:asso-di-spade  |  bacodi:assenza-di-orlando                    |
|  3 | bacodi:dieci-di-spade | bacodi:guerra                                 |
|  4 | bacodi:dieci-di-spade | bacodi:cadaveri-squartati                     |
|  5 | bacodi:dieci-di-spade | bacodi:storia-bellicosa-di-orlando            |
|  6 | bacodi:dieci-di-spade | bacodi:barriera-degli-arcangeli               |
|  7 | bacodi:due-di-spade   |  bacodi:duello-tra-protagonista-e-condottiero |
|  8 | bacodi:due-di-spade   |  bacodi:guardie                               |
|  9 | bacodi:due-di-spade   |  bacodi:duello                                |
| 10 | bacodi:nove-di-spade  |  bacodi:esito-della-guerra                    |

### Cups

What are the meanings associated with cards that have suit Cups?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit bacodi:coppe.
    ?cardDeck odi:hasTypology bacodi:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |        cardDeck        |             meaning            |
|----|------------------------|--------------------------------|
|  1 | bacodi:asso-di-coppe   | bacodi:coppa-sacra             |
|  2 | bacodi:asso-di-coppe   | bacodi:vino                    |
|  3 | bacodi:asso-di-coppe   | bacodi:fonte-della-vita        |
|  4 | bacodi:asso-di-coppe   | bacodi:bevuta-del-protagonista |
|  5 | bacodi:cinque-di-coppe | bacodi:coppe                   |
|  6 | bacodi:cinque-di-coppe | bacodi:brindisi                |
|  7 | bacodi:cinque-di-coppe | bacodi:discorso                |
|  8 | bacodi:cinque-di-coppe | bacodi:rintocchi               |
|  9 | bacodi:cinque-di-coppe | bacodi:segreto                 |
| 10 | bacodi:dieci-di-coppe  | bacodi:osteria                 |

## The narrative function of court cards and triumphs

Court cards are used by Calvino to represent each protagonist in the story (e.g. the *Cavaliere di Coppe* in *Storia dell'ingrato punito*). For this reason, interrogating the ontology to find out the semantic content of all the representations of the court cards was useful for two reasons: the first because the existence of cases in which the court cards do not have the 'protagonist' representation emerged, noting the non-exclusivity of this type of card with the role of protagonist cards (e.g. the *Fante di Bastoni* in *Storia dell'Orlando pazzo per amore* which represents Medoro); the second because it turns out that the court cards almost always represent a character (odi:Character, 12 occurrences), but with the presence of one occurrence in which the court card refers to an inanimate object (Trojan horse) and two occurrences, instead, concerning an event (removal of a leader, unforeseen). In this way, it was verified how Calvino prefers the court card typology to represent characters in stories.
Triumphs present more complex miniatures and this complexity stimulates the author's imagination, enriching the multiple possibilities of interpretation for the narrative plots. In fact, the results of the seventh query are very diversified: some triumphs represent characters (e.g. brigand, maiden), others inanimate objects (e.g. prediction, soul), still others events (e.g. violence, transformation of everything into gold) or finctional places (e.g. grave, moon); finally, some refer to symbols (e.g. inner harmony, justice).

### Court cards

Are there cases in which the court cards don't have a reference to the protagonist?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasTypology bacodi:carta-di-corte.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |           cardDeck          |                meaning                |
|----|-----------------------------|---------------------------------------|
|  1 | bacodi:regina-di-coppe      | bacodi:protagonista                   |
|  2 | bacodi:cavaliere-di-bastoni | bacodi:cavallo-di-troia               |
|  3 | bacodi:cavaliere-di-bastoni | bacodi:protagonista                   |
|  4 | bacodi:cavaliere-di-coppe   | bacodi:allontanamento-del-condottiero |
|  5 | bacodi:cavaliere-di-coppe   | bacodi:protagonista                   |
|  6 | bacodi:cavaliere-di-denari  | bacodi:protagonista                   |
|  7 | bacodi:cavaliere-di-spade   | bacodi:guerriero                      |
|  8 | bacodi:cavaliere-di-spade   | bacodi:condottiero                    |
|  9 | bacodi:cavaliere-di-spade   | bacodi:arcangelo                      |
| 10 | bacodi:cavaliere-di-spade   | bacodi:imprevisto                     |

### Court cards

If yes, to which class do the other representations belong?

```
select ?cardDeck ?meaning ?class
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasTypology bacodi:carta-di-corte.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
    ?representation a ?class
  FILTER NOT EXISTS {?representation odi:hasMeaningOf bacodi:protagonista}
}
```

|    |           cardDeck          |                meaning                |        class        |
|----|-----------------------------|---------------------------------------|---------------------|
|  1 | bacodi:cavaliere-di-bastoni | bacodi:cavallo-di-troia               | odi:InanimateObject |
|  2 | bacodi:cavaliere-di-coppe   | bacodi:allontanamento-del-condottiero | odi:Event           |
|  3 | bacodi:cavaliere-di-spade   | bacodi:guerriero                      | odi:Character       |
|  4 | bacodi:cavaliere-di-spade   | bacodi:condottiero                    | odi:Character       |
|  5 | bacodi:cavaliere-di-spade   | bacodi:arcangelo                      | odi:Character       |
|  6 | bacodi:cavaliere-di-spade   | bacodi:imprevisto                     | odi:Event           |
|  7 | bacodi:fante-di-bastoni     | bacodi:brigante                       | odi:Character       |
|  8 | bacodi:fante-di-bastoni     | bacodi:medoro                         | odi:Character       |
|  9 | bacodi:fante-di-spade       | bacodi:guerriero                      | odi:Character       |
| 10 | bacodi:re-di-denari         | bacodi:padre-del-condottiero          | odi:Character       |

### Triumphs

Which class do the triumphs most represent?

```
select ?cardDeck ?class
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasTypology bacodi:trionfo.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation a ?class.
}
```

|    |      cardDeck      |        class        |
|----|--------------------|---------------------|
|  1 | bacodi:il-bagatto  | odi:Character       |
|  2 | bacodi:il-bagatto  | odi:Character       |
|  3 | bacodi:il-bagatto  | odi:Character       |
|  4 | bacodi:il-bagatto  | odi:Character       |
|  5 | bacodi:il-carro    | odi:InanimateObject |
|  6 | bacodi:il-carro    | odi:InanimateObject |
|  7 | bacodi:il-carro    | odi:Event           |
|  8 | bacodi:il-carro    | odi:Event           |
|  9 | bacodi:il-sole     | odi:InanimateObject |
| 10 | bacodi:il-sole     | odi:Event           |
| 11 | bacodi:il-sole     | odi:Character       |
| 12 | bacodi:il-sole     | odi:Character       |
| 13 | bacodi:il-diavolo  | odi:Character       |
| 14 | bacodi:il-diavolo  | odi:Character       |
| 15 | bacodi:il-diavolo  | odi:Character       |
| 16 | bacodi:il-diavolo  | odi:Character       |
| 17 | bacodi:il-giudizio | odi:Symbol          |
| 18 | bacodi:il-giudizio | odi:InanimateObject |
| 19 | bacodi:il-giudizio | odi:Symbol          |
| 20 | bacodi:il-giudizio | odi:InanimateObject |
| 21 | bacodi:il-matto    | odi:Character       |
| 22 | bacodi:il-matto    | odi:Character       |
| 23 | bacodi:il-matto    | odi:Character       |
| 24 | bacodi:il-matto    | odi:Character       |
| 25 | bacodi:il-mondo    | odi:FinctionalPlace |

## Use the same cards with the same meaning in different stories

The meaning of the triumph *La Luna* in *Storia dell'Orlando pazzo per amore* and in *Storia di Astolfo sulla Luna* can only be the moon, both because the card can only refer to the moon due to its specific iconography, and because it is used in two stories that share a reference to the story of Orlando. Significant, however, are the other results of the query, as they show how other cards share the same representation in different occurrences in the text, despite having miniatures that cannot be univocally interpreted: for example, the *Nove di Coppe* that in both the first and last stories of the chapter *Tutte le altre storie* is used to represent the banquet; the *Otto di Coppe* that in *Storia dell'ingrato punito* and in the last story of the final chapter signifies the wedding banquet.

### Same meaning in different stories

Which cards have the same representation in the different stories?

```
select ?cardDeck ?meaning (group_concat(distinct ?story) as ?stories) (count(distinct ?story) as ?n_stories)
where {
   ?cardDeck a odi:DeckCard.
   ?cardStory odi:specifies ?cardDeck.
   ?story odi:hasCard ?cardStory.
   ?cardStory odi:carriesRepresentation ?representation.
   ?representation odi:hasMeaningOf ?meaning.  
}
GROUP BY ?cardDeck ?meaning
HAVING (?n_stories XXX 1)
ORDER BY DESC (?n_stories)
```

|    |          cardDeck      |         meaning           |      stories    |       n_stories      |
|----|------------------------|---------------------------|-----------------|----------------------|
|  1 | bacodi:il-diavolo      | bacodi:diavolo            | "https://purl.org/ebr/odi/data/TuttelealtrestorieCinque https://purl.org/ebr/odi/data/TuttelealtrestorieQuattro https://purl.org/ebr/odi/data/storiaTre"                |  "3"^^xsd:integer    |
|  2 | bacodi:nove-di-bastoni | bacodi:bosco              | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieSei https://purl.org/ebr/odi/data/storiaUno"                |  "3"^^xsd:integer    |
|  3 | bacodi:il-papa         | bacodi:papa               | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/storiaTre"                |  "2"^^xsd:integer    |
|  4 | bacodi:la-forza        | bacodi:brigante           | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/storiaUno"                |  "2"^^xsd:integer    |
|  5 | bacodi:nove-di-denari  | bacodi:ricchezza          | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/storiaQuattro"                |  "2"^^xsd:integer    |
|  6 | bacodi:sei-di-spade    | bacodi:battaglie          | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieQuattro"                |  "2"^^xsd:integer    |
|  7 | bacodi:otto-di-coppe   | bacodi:banchetto-di-nozze | "https://purl.org/ebr/odi/data/TuttelealtrestorieSei https://purl.org/ebr/odi/data/storiaUno"                |  "2"^^xsd:integer    |
|  8 | bacodi:lo-eremita      | bacodi:indovino           | "https://purl.org/ebr/odi/data/TuttelealtrestorieUno https://purl.org/ebr/odi/data/storiaSei"                |  "2"^^xsd:integer    |
|  9 | bacodi:nove-di-coppe   | bacodi:banchetto          | "https://purl.org/ebr/odi/data/TuttelealtrestorieUno https://purl.org/ebr/odi/data/storiaSei"                |  "2"^^xsd:integer    |
| 10 | bacodi:il-sole         | bacodi:bambino            | "https://purl.org/ebr/odi/data/storiaCinque https://purl.org/ebr/odi/data/storiaUno"                |  "2"^^xsd:integer    |   

## Use different cards for the same representation in the same story

Two cards may have a semantic link to express an identity (odi:sameAs) or an evolution of the same representation (odi:changesIn).  
The results of the two queries reveal six occurrences where two cards are used to represent the same entity within a story and ten occurrences where two cards are used to represent an evolution of the same entity within a story.
In the first case, the entity of the two cards is almost always a character (5 occurrences vs. 6 total occurrences), with the exception of one occurrence where it is a symbol (richness). Thus, one notes an almost exclusive propensity to delineate a character's identity through the use of two different cards in the same story.
In the second case, the evolution expressed between the two cards always occurs for a character, without exception (thus excluding inanimate objects, events, places and symbols). Thus, evolution turns out to be an exclusive property of characters. Most of the time (6 vs. 10), both the starting card and the finishing card is a triumph, but there are occurrences of court cards: three as a starting card (e.g. from the *Cavaliere di Coppe* to *Il Penduto* and only one as a finishing card (from *La Stella* to the *Regina di Spade*). This means that triumphs are more effective for the writer to represent an evolution of a character in the story and that the court card competes with the triumph to represent a condition - physical or intellectual - at the beginning, but not to express evolution.

### Identity

Which different cards have the same representation?

```
select distinct ?cardDeck1 ?story1 ?cardDeck2 ?story2 ?meaning
where {
    ?cardStory1 odi:specifies ?cardDeck1.
    ?cardStory1 odi:carriesRepresentation ?representation1.
    ?story1 odi:hasCard ?cardStory1.
    ?representation1 odi:hasMeaningOf ?meaning.
    ?cardStory2 odi:specifies ?cardDeck2.
    ?cardStory2 odi:carriesRepresentation ?representation2.
    ?story2 odi:hasCard ?cardStory2.
    ?representation2 odi:hasMeaningOf ?meaning.
    ?representation1 odi:sameAs ?representation2
    FILTER (?cardDeck1 != ?cardDeck2)
}
```
|   | cardDeck1 | story1 | cardDeck2 | story2 | meaning |
|---|-----------|--------|-----------|--------|---------|
| 1 | bacodi:il-bagatto | bacodi:storiaDue | bacodi:il-diavolo | bacodi:storiaDue | bacodi:visitatore |
| 2 | bacodi:fante-di-coppe | bacodi:TuttelealtrestorieCinque | bacodi:il-bagatto | bacodi:TuttelealtrestorieCinque | bacodi:protagonista |
| 3 | bacodi:la-forza | bacodi:TuttelealtrestorieDue | bacodi:fante-di-bastoni | bacodi:TuttelealtrestorieDue | bacodi:brigante |
| 4 | bacodi:la-stella | bacodi:storiaTre | bacodi:la-morte | bacodi:storiaTre | bacodi:fanciulla |
| 5 | bacodi:nove-di-denari | bacodi:storiaQuattro | bacodi:dieci-di-denari | bacodi:storiaQuattro | bacodi:ricchezza |
| 6 | bacodi:regina-di-bastoni | bacodi:TuttelealtrestorieSei | bacodi:la-giustizia | bacodi:TuttelealtrestorieSei | bacodi:protagonista |

### Evolution

Which different cards express an evolution of the same representation?

```
select distinct ?cardDeck1 ?story1 ?cardDeck2 ?story2 ?meaning
where {
    ?cardStory1 odi:specifies ?cardDeck1.
    ?cardStory1 odi:carriesRepresentation ?representation1.
    ?story1 odi:hasCard ?cardStory1.
    ?representation1 odi:hasMeaningOf ?meaning.
    ?cardStory2 odi:specifies ?cardDeck2.
    ?cardStory2 odi:carriesRepresentation ?representation2.
    ?story2 odi:hasCard ?cardStory2.
    ?representation2 odi:hasMeaningOf ?meaning.
    ?representation1 odi:changesIn ?representation2
    FILTER (?cardDeck1 != ?cardDeck2)
}
```

|   | cardDeck1 | story1 | textualreference1 | textualreference2 | cardDeck2 | story2 |
|---|-----------|--------|-------------------|-------------------|-----------|--------|
| 1 | bacodi:la-temperanza | bacodi:storiaUno | "??forse figlia d'un boscaiolo o d'un capraio, che avanzava [...] reggendo due brocche d'acqua, certo di ritorno dalla fonte.??" | "??la sua salvatrice del bosco, fatta pi?? piena e risoluta e calma, con un melanconico sorriso [...].??" | bacodi:la-giustizia | bacodi:storiaUno |
| 2 | bacodi:la-temperanza | bacodi:storiaUno | "??forse figlia d'un boscaiolo o d'un capraio, che avanzava [...] reggendo due brocche d'acqua, certo di ritorno dalla fonte.??" | "??spadaccina agguerita??" | bacodi:la-giustizia | bacodi:storiaUno |
| 3 | bacodi:la-temperanza | bacodi:storiaUno | "??semplice figlia dei boschi??" | "??la sua salvatrice del bosco, fatta pi?? piena e risoluta e calma, con un melanconico sorriso [...].??" | bacodi:la-giustizia | bacodi:storiaUno |
| 4 | bacodi:la-temperanza | bacodi:storiaUno | "??semplice figlia dei boschi??" | "??spadaccina agguerita??" | bacodi:la-giustizia | bacodi:storiaUno |
| 5 | bacodi:cavaliere-di-coppe | bacodi:storiaUno | "??un giovane roseo e biondo che sfoggiava un mantello raggiante di ricami a forma di sole, [...] mosso [...] pi?? dal desiderio d'apparire che da una vera vocazione cavalleresca.??" | "??il nostro giovane biondo spogliato d'ogni avere, e lasciato a penzolare da un ramo, a testa in gi??.??" | bacodi:il-penduto | bacodi:storiaUno |
| 6 | bacodi:re-di-spade | bacodi:storiaCinque | "??Orlando paladino che mulinava la sua Durlindana.??" | "??Sfogato ormai il pi?? grosso groppo di furore, [...] con la testa piene di penne [...] ecco che Orlando ersa disceso gi?? nel cuore caotico delle cose, [...] al punto d'intersezione di tutti gli ordini possibili.??" | bacodi:il-matto | bacodi:storiaCinque |
| 7 | bacodi:la-forza | bacodi:TuttelealtrestorieDue | "??feroce brigante??" | "??un feroce brigante [...] appeso a uno strumento di tortura??" | bacodi:il-penduto | bacodi:TuttelealtrestorieDue |
| 8 | bacodi:la-forza | bacodi:TuttelealtrestorieSei | "??l'energumeno??" | "??lo scherano [...] legato a testa in gi????" | bacodi:il-penduto | bacodi:TuttelealtrestorieSei |
| 9 | bacodi:la-stella | bacodi:storiaTre | "??una giovinetta di sidereo pallore che s'aggirava nella notte in camicia e coi capelli sciolti, levando alto un cero acceso.??" | "??ecco la meschinella trasformarsi in regina da torneo, pavoneggiarsi, far la gatta.??" | bacodi:regina-di-spade | bacodi:storiaTre |
| 10 | bacodi:regina-di-bastoni | bacodi:TuttelealtrestorieSei | "??nostra narratrice, allora tenera educanda??" | "??l'eroina s'era celata sotto i panni d'una ostessa o ancella di castello??" | bacodi:la-temperanza | bacodi:TuttelealtrestorieSei |

# The text structure

## *Pattern* of cards

Each protagonist can have a "simple relationship", i.e. a direct relationship, or a "complex relationship", i.e. an indirect relationship, with the other cards in its history: in particular, cards that have a direct relationship can either be specified (odi:isSpecifiedBy) or have a general relationship (odi:isRelatedWith) with the card that has an indirect relationship with that protagonist.
In the first case, only the triumphs *Il Mondo* and *La Torre* are, in fact, used twice to express the same narrative situation: the meaning of *Il Mondo*is specified by *La Torre* (*Storia dell'ingrato punito* and the first story of *Tutte le altre storie*).
In the second case, the numerals *Due di Denari* and *Quattro di Spade* have a general relation with the triumph *Il Diavolo* in three occurrences: *Storia della sposa dannata*, and the fourth and fifth story of the chapter *Tutte le altre storie*. Therefore, a significant *pattern* of cards was discovered: *Il Diavolo*, the *Due di Denari* and the *Quattro di Spade*.

### Specification

Which pairs of cards are used, more than once, close together where one is specified by the other?

```
select distinct ?cardDeck1 ?story1 ?cardDeck2 ?story2
where {
    ?cardStory1 odi:specifies ?cardDeck1.
    ?cardStory1 odi:carriesRepresentation ?representation1.
    ?story1 odi:hasCard ?cardStory1.
    ?representation1 odi:hasMeaningOf ?meaning1.
    ?cardStory2 odi:specifies ?cardDeck2.
    ?cardStory2 odi:carriesRepresentation ?representation2.
    ?story2 odi:hasCard ?cardStory2.
    ?representation2 odi:hasMeaningOf ?meaning2.
    ?representation1 odi:isSpecifiedWith ?representation2.
    FILTER (?cardDeck1 != ?cardDeck2)
}
```

|    |         cardDeck1         |            story1            |       cardDeck2       |            story2            |
|----|---------------------------|------------------------------|-----------------------|------------------------------|
|  1 | bacodi:cavaliere-di-spade | bacodi:TuttelealtrestorieDue | bacodi:nove-di-denari | bacodi:TuttelealtrestorieDue |
|  2 | bacodi:dieci-di-denari    | bacodi:TuttelealtrestorieDue | bacodi:il-giudizio    | bacodi:TuttelealtrestorieDue |
|  3 | bacodi:dieci-di-denari    | bacodi:TuttelealtrestorieDue | bacodi:la-torre       | bacodi:TuttelealtrestorieDue |
|  4 | bacodi:dieci-di-denari    | bacodi:TuttelealtrestorieDue | bacodi:otto-di-coppe  | bacodi:TuttelealtrestorieDue |
|  5 | bacodi:dieci-di-denari    | bacodi:TuttelealtrestorieDue | bacodi:sei-di-spade   | bacodi:TuttelealtrestorieDue |
|  6 | bacodi:il-giudizio        | bacodi:storiaSei             | bacodi:dieci-di-coppe | bacodi:storiaSei             |
|  7 | bacodi:il-mondo           | bacodi:storiaQuattro         | bacodi:la-torre       | bacodi:storiaQuattro         |
|  8 | bacodi:il-mondo           | bacodi:TuttelealtrestorieUno | bacodi:la-torre       | bacodi:TuttelealtrestorieUno |
|  9 | bacodi:il-penduto         | bacodi:TuttelealtrestorieDue | bacodi:il-sole        | bacodi:TuttelealtrestorieDue |
| 10 | bacodi:il-penduto         | bacodi:TuttelealtrestorieDue | bacodi:la-giustizia   | bacodi:TuttelealtrestorieDue |

### General relation

Which pairs of cards are used, more than once, close together where one has a general relationship with the other?

```
select distinct ?cardDeck1 ?story1 ?cardDeck2 ?story2
where {
    ?cardStory1 odi:specifies ?cardDeck1.
    ?cardStory1 odi:carriesRepresentation ?representation1.
    ?story1 odi:hasCard ?cardStory1.
    ?representation1 odi:hasMeaningOf ?meaning1.
    ?cardStory2 odi:specifies ?cardDeck2.
    ?cardStory2 odi:carriesRepresentation ?representation2.
    ?story2 odi:hasCard ?cardStory2.
    ?representation2 odi:hasMeaningOf ?meaning2.
    ?representation1 odi:isRelatedWith ?representation2.
    FILTER (?cardDeck1 != ?cardDeck2)
}
```

|   | cardDeck1 | story1 | cardDeck2 | story2 |
|---|-----------|--------|-----------|--------|
| 1 | bacodi:cavaliere-di-denari | bacodi:TuttelealtrestorieQuattro | bacodi:due-di-bastoni | bacodi:TuttelealtrestorieQuattro |
| 2 | bacodi:cavaliere-di-spade | bacodi:storiaQuattro | bacodi:nove-di-denari | bacodi:storiaQuattro |
| 3 | bacodi:cavaliere-di-spade | bacodi:storiaQuattro | bacodi:otto-di-coppe | bacodi:storiaQuattro |
| 4 | bacodi:cavaliere-di-spade | bacodi:storiaQuattro | bacodi:sei-di-spade | bacodi:storiaQuattro |
| 5 | bacodi:dieci-di-coppe | bacodi:TuttelealtrestorieDue | bacodi:asso-di-bastoni | bacodi:TuttelealtrestorieDue |
| 6 | bacodi:dieci-di-denari | bacodi:TuttelealtrestorieSei | bacodi:nove-di-bastoni | bacodi:TuttelealtrestorieSei |
| 7 | bacodi:fante-di-spade | bacodi:TuttelealtrestorieQuattro | bacodi:sei-di-coppe | bacodi:TuttelealtrestorieQuattro |
| 8 | bacodi:due-di-spade | bacodi:TuttelealtrestorieSei | bacodi:otto-di-spade | bacodi:TuttelealtrestorieSei |
| 9 | bacodi:il-diavolo | bacodi:TuttelealtrestorieCinque | bacodi:due-di-denari | bacodi:TuttelealtrestorieCinque |
| 10 | bacodi:la-papessa | bacodi:TuttelealtrestorieCinque | bacodi:asso-di-coppe | bacodi:TuttelealtrestorieCinque |

## The iconographic dimension

There are a total of 118 iconographic depictions running along the edition's margins, comprising 61 large and 57 small images. However, the iconographic dimensions are different.
The three queries made for the iconographic dimension of the cards show that, as far as numerals and triumphs are concerned, the discrepancy between the number of big dimensions and small dimensions is little.
Differently, the iconographic dimension of the court cards, and in particular those representing the protagonist, is almost always big with the exception of three occurrences in the sixth chapter Tutte le altre storie in which it is drawn on the page with a small size (*Il Bagatto* in the fifth story; *La Temperanza* and *La Giustizia* in the last story). In all three occurrences, however, the three cards express something else than the presentation at the beginning of the story. In other words, the big size serves, initially, the reader of the story to identify the protagonist's card; the other times the protagonist appears with a different card, it can be either big or small in size. For example, in *Storia dell???alchimista che vendette l???anima* the protagonist is, initially, represented with the *Fante di Coppe* and it has got a big dimension. After, the protagonist is represented with *Il Bagatto*, which serves to express the protagonist's desire to become emperor, and it has got a small dimension. In this way, the author???s artistic choice to give importance to the dimension of each card in the text is proven. In the case of the protagonist card, the big dimension indicates the importance of the protagonist as the main driving force of the narrative.

### Protagonist's dimension

What is the iconographic dimension of the protagonist?

```
select distinct ?cardDeck ?story ?iconography
where {
    ?cardDeck a odi:DeckCard.     
    ?cardStory odi:specifies ?cardDeck.
    ?story odi:hasCard ?cardStory.
    ?cardStory odi:hasIconography ?iconography.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf bacodi:protagonista.
}
```

|    |           cardDeck          |              story              |   iconography  |
|----|-----------------------------|---------------------------------|----------------|
|  1 | bacodi:re-di-coppe          | bacodi:storiaDue                | bacodi:grande  |  
|  2 | bacodi:il-penduto           | bacodi:storiaUno                | bacodi:grande  |   
|  3 | bacodi:cavaliere-di-bastoni | bacodi:storiaSei                | bacodi:grande  |   
|  4 | bacodi:cavaliere-di-coppe   | bacodi:storiaUno                | bacodi:grande  |   
|  5 | bacodi:re-di-bastoni        | bacodi:TuttelealtrestorieTre    | bacodi:grande  |   
|  6 | bacodi:fante-di-spade       | bacodi:storiaTre                | bacodi:grande  |   
|  7 | bacodi:la-temperanza        | bacodi:TuttelealtrestorieSei    | bacodi:piccola |   
|  8 | bacodi:la-giustizia         | bacodi:TuttelealtrestorieSei    | bacodi:piccola |   
|  9 | bacodi:fante-di-coppe       | bacodi:TuttelealtrestorieCinque | bacodi:grande  |   
| 10 | bacodi:il-bagatto           | bacodi:TuttelealtrestorieCinque | bacodi:piccola |   

### Big dimension

How many cards have a big iconographic dimension?

```
select distinct ?typology (COUNT(DISTINCT ?cardDeck) AS ?n)
where {
    ?cardDeck a odi:DeckCard.     
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:hasIconography bacodi:grande.
    ?cardDeck odi:hasTypology ?typology.
}
GROUP BY ?typology ORDER BY DESC (?n)
```

|   |        typology       |         n         |
|---|-----------------------|-------------------|
| 1 | bacodi:trionfo        | "21"^^xsd:integer |
| 2 | bacodi:numerale       | "16"^^xsd:integer |
| 3 | bacodi:carta-di-corte | "14"^^xsd:integer |

### Small dimension

How many cards have a small iconographic dimension?

```
select distinct ?typology (COUNT(DISTINCT ?cardDeck) AS ?n)
where {
    ?cardDeck a odi:DeckCard.     
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:hasIconography bacodi:piccola.
    ?cardDeck odi:hasTypology ?typology.
}
GROUP BY ?typology ORDER BY DESC (?n)
```

|   |        typology       |         n         |
|---|-----------------------|-------------------|
| 1 | bacodi:trionfo        | "19"^^xsd:integer |
| 2 | bacodi:numerale       | "15"^^xsd:integer |
| 3 | bacodi:carta-di-corte | "5"^^xsd:integer  |

## Position of the cards

The position of the cards concerns the order in which they appear in the stories.
The results of query 16 show that some cards appear in two different stories at the same time. In other words, two cards are mentioned in two different stories at the same point in the order of their appearance. This is possible due to the strict architecture of the square that interweaves the cards in such a way that some of them are used more than once, but without being able to move them from their previously established position.

### Same position

Are there cards that have the same position in more than one story?

```
select ?cardDeck ?position (group_concat(distinct ?story) as ?stories) (count(distinct ?story) as ?n_stories)
where {
    ?cardDeck a odi:DeckCard.
    ?cardStory odi:specifies ?cardDeck.
    ?story odi:hasCard ?cardStory.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
    ?cardStory odi:hasPositionInTheText ?position.    
}
GROUP BY ?cardDeck ?position
HAVING (?n_stories XXX 1)
ORDER BY DESC (?n_stories)
```

|  | cardDeck | position | stories | n_stories |
|--|----------|----------|---------|-----------|
| 1 | bacodi:la-stella | "4"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieCinque https://purl.org/ebr/odi/data/storiaTre" | "2"^^xsd:integer |
| 2 | bacodi:fante-di-bastoni | "7"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/storiaCinque" | "2"^^xsd:integer |
| 3 | bacodi:il-matto | "11"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieUno" | "2"^^xsd:integer |
| 4 | bacodi:la-giustizia | "5"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieSei" | "2"^^xsd:integer |
| 5 | bacodi:la-luna | "10"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieUno" | "2"^^xsd:integer |
| 6 | bacodi:lo-amore | "9"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieDue https://purl.org/ebr/odi/data/TuttelealtrestorieUno" | "2"^^xsd:integer |
| 7 | bacodi:la-papessa | "3"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieSei https://purl.org/ebr/odi/data/storiaDue" | "2"^^xsd:integer |
| 8 | bacodi:la-temperanza | "16"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieSei https://purl.org/ebr/odi/data/storiaDue" | "2"^^xsd:integer |
| 9 | bacodi:dieci-di-coppe | "7"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieUno https://purl.org/ebr/odi/data/storiaQuattro" | "2"^^xsd:integer |
| 10 | bacodi:nove-di-coppe | "13"^^xsd:integer | "https://purl.org/ebr/odi/data/TuttelealtrestorieUno https://purl.org/ebr/odi/data/storiaDue" | "2"^^xsd:integer |
| 11 | bacodi:lo-amore | "6"^^xsd:integer | "https://purl.org/ebr/odi/data/storiaCinque https://purl.org/ebr/odi/data/storiaSei" | "2"^^xsd:integer |

# Relationships between cards

## "simple relations" and "complex relations"

The direct relationships that each protagonist has with the other cards within each story have a minimal gap compared to the indirect ones: the former, in fact, number 83 compared to the total number of 71 for the latter.
The last query provides one of the most interesting results at the narratological level: some properties, relating to narrative relationships, are used more frequently than others. By following the decreasing order of incidence of the various relations, it is possible to delineate a constant narrative sequence: a character (protagonist) comes across (odi:bumpsInto) another character at a certain place in the story - which is almost always the forest or the forest - (odi:movingThrough) and, once he receives something (odi:receives), he sets off to reach another place (odi:arrivesAt), in which the story will develop further. This narrative sequence is interesting to note an order in the way Calvino tells stories using tarot cards as signs.

### Simple relations

How many cards have a simple relationship with the protagonist?

```
select ?representation1 ?relation ?representation2
where {
    ?representation1 odi:hasMeaningOf bacodi:protagonista.
    ?representation2 a ?class2.
    ?class2 rdfs:subClassOf odi:Representation.
    ?representation1 ?relation ?representation2.
    FILTER NOT EXISTS {?representation1 odi:hasComplexRelationWith ?representation2.}
}
```

|   | representation1 | relation | representation2 |
|---|-----------------|----------|-----------------|
| 1 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | odi:bumpsInto | bacodi:la-forza-tuttelealtrestorieDue-brigante |
| 2 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | odi:bumpsInto | bacodi:regina-di-spade-tuttelealtrestorieDue-guerriera |
| 3 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | odi:movingThrough | bacodi:dieci-di-bastoni-tuttelealtrestorieDue-bosco |
| 4 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | odi:discovers | bacodi:fante-di-bastoni-tuttelealtrestorieDue-brigante |
| 5 | bacodi:re-di-coppe-storiaDue-protagonista | odi:bumpsInto | bacodi:il-bagatto-storiaDue-visitatore |
| 6 | bacodi:re-di-coppe-storiaDue-protagonista | odi:receives | bacodi:cinque-di-coppe-storiaDue-discorso_anima_corpo |
| 7 | bacodi:re-di-coppe-storiaDue-protagonista | odi:receives | bacodi:cinque-di-coppe-storiaDue-segreto_alchimistico |
| 8 | bacodi:re-di-coppe-storiaDue-protagonista | odi:receives | bacodi:lo-imperatore-storiaDue-profezia |
| 9 | bacodi:re-di-coppe-storiaDue-protagonista | odi:longsFor | bacodi:asso-di-coppe-storiaDue-fonte_della_vita |
| 10 | bacodi:re-di-coppe-storiaDue-protagonista | odi:movingThrough | bacodi:otto-di-bastoni-storiaDue-bosco |
| 11 | bacodi:re-di-coppe-storiaDue-protagonista | odi:sees | bacodi:sette-di-denari-storiaDue-denaro |
| 12 | bacodi:re-di-coppe-storiaDue-protagonista | odi:discovers | bacodi:il-diavolo-storiaDue-visitatore |
| 13 | bacodi:re-di-coppe-storiaDue-protagonista | odi:trades | bacodi:la-stella-storiaDue-anima |
| 14 | bacodi:re-di-coppe-storiaDue-protagonista | odi:isHelpedBy | bacodi:la-papessa-storiaDue-strega |
| 15 | bacodi:cavaliere-di-bastoni-storiaSei-protagonista | odi:bumpsInto | bacodi:il-bagatto-storiaSei-poeta |

### Complex relations

How many cards have a complex relationship with the protagonist?

```
select ?representation1 ?representation2
where {
    ?representation1 odi:hasMeaningOf bacodi:protagonista.
    ?representation2 a ?class2.
    ?class2 rdfs:subClassOf odi:Representation.
    ?representation1 odi:hasComplexRelationWith ?representation2.


```
|   | representation1 | representation2 |  
|---|-----------------|-----------------|
| 1 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:il-carro-tuttelealtrestorieDue-carro |  |
| 2 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:cinque-di-denari-tuttelealtrestorieDue-luce_del_mattino |  |
| 3 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:dieci-di-spade-tuttelealtrestorieDue-guerra |  |
| 4 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:il-matto-tuttelealtrestorieDue-vagabondo |  |
| 5 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:il-penduto-tuttelealtrestorieDue-brigante |  |
| 6 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:il-sole-tuttelealtrestorieDue-sole |  |
| 7 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:la-giustizia-tuttelealtrestorieDue-giustizia |  |
| 8 | bacodi:regina-di-coppe-tuttelealtrestorieDue-protagonista | bacodi:tre-di-coppe-tuttelealtrestorieDue-bevuta_del_brigante |  |
| 9 | bacodi:re-di-coppe-storiaDue-protagonista | bacodi:due-di-spade-storiaDue-guardie |  |
| 10 | bacodi:re-di-coppe-storiaDue-protagonista | bacodi:nove-di-coppe-storiaDue-ricchezza |  |
| 11 | bacodi:re-di-coppe-storiaDue-protagonista | bacodi:sei-di-denari-storiaDue-citt??_di_oro |  |
| 12 | bacodi:re-di-coppe-storiaDue-protagonista | bacodi:la-temperanza-storiaDue-fanciulla |  |
| 13 | bacodi:cavaliere-di-bastoni-storiaSei-protagonista | bacodi:asso-di-denari-storiaSei-luna |  |
| 14 | bacodi:cavaliere-di-bastoni-storiaSei-protagonista | bacodi:dieci-di-coppe-storiaSei-deposito |  |
| 15 | bacodi:cavaliere-di-bastoni-storiaSei-protagonista | bacodi:il-matto-storiaSei-orlando |  |


### ++ Simple relations

What are the simple relationships that appear most frequently in the collection?

```
select ?relation (COUNT(?relation) as ?n)
where {
    ?representation1 odi:hasMeaningOf bacodi:protagonista.
    ?representation2 a ?class2.
    ?class2 rdfs:subClassOf odi:Representation.
    ?representation1 ?relation ?representation2.
    FILTER (?representation1 != ?representation2)
    FILTER NOT EXISTS {?representation1 odi:hasComplexRelationWith ?representation2.}   
}
GROUP BY ?relation ORDER BY DESC (?n)
```

|    |            relation           |         n         |
|----|-------------------------------|-------------------|
|  1 | odi:bumpsInto                 | "21"^^xsd:integer |
|  2 | odi:movingThrough             | "9"^^xsd:integer  |
|  3 | odi:receives                  | "9"^^xsd:integer  |
|  4 | odi:arrivesAt                 | "6"^^xsd:integer  |
|  5 | odi:hasAParticularConditionOf | "6"^^xsd:integer  |
|  6 | odi:discovers                 | "4"^^xsd:integer  |
|  7 | odi:longsFor                  | "4"^^xsd:integer  |
|  8 | odi:sees                      | "4"^^xsd:integer  |
|  9 | odi:isHelpedBy                | "4"^^xsd:integer  |
| 10 | odi:changesIn                 | "3"^^xsd:integer  |
| 11 | odi:isDefeatedBy              | "3"^^xsd:integer  |
| 12 | odi:trades                    | "2"^^xsd:integer  |
| 13 | odi:marries                   | "2"^^xsd:integer  |
| 14 | odi:sameAs                    | "2"^^xsd:integer  |
| 15 | odi:hasFamilyRelationWith     | "1"^^xsd:integer  |
| 16 | odi:loses                     | "1"^^xsd:integer  |
| 17 | odi:climbs                    | "1"^^xsd:integer  |
| 18 | odi:speaksTo                  | "1"^^xsd:integer  |
