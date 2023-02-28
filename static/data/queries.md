# The semantics

## The semiotics of suits in numeral cards

The first four queries present significant results for the study of the semiotics of tarot suits. With regard to the suit of Wands, the largest percentage shows that the reference is to the forest and, in general, to the forest setting of *Il Castello*. In those cases where the semantics deviates from the setting, it emerges that it is the number that defines the meaning of the card: the *Due di Bastoni* is, in fact, used to express a duality or a choice between two situations (fourth story of *Tutte le altre storie*) regardless of the suit; the *Asso di Bastoni*, on the other hand, may refer not only to the tree, but also to power and its material symbol (third story of *Tutte le altre storie*). Unlike numerals with the suit of Wands, those of Coins refer, instead, to two clearly opposite semantic fields: the first is that of earthly power, wealth and materiality (e.g. richness, inheritance, money); the second, on the other hand, has to do with heaven, the divine and the immaterial (e.g. light, moon, state of beatitude). Between the two semantic fields, however, the former stands out over the latter. The largest percentage of the results obtained for the semantics of numerals with the seed of Swords pertain to themes of warfare (e.g. war, duel, dispute); sometimes, it specifically refers to defence (e.g. barrier, guards). Finally, the semantic meaning associated with the suit of Cups is less clearly defined than the three aforementioned suits. From the results, it is possible to note a large percentage that refers to banqueting and refreshment (e.g. banquet, wedding banquet, tavern); there are, however, other references such as those related to wealth (e.g. the source of life, world peace) or to love (e.g. love encounter).

### Wands

What are the meanings associated with cards that have suit Wands?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:bastoni.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |         cardDeck        |            meaning            |
|----|-------------------------|-------------------------------|
|  1 | odikb:due-di-bastoni    | odikb:necessità-di-una-scelta |
|  2 | odikb:due-di-bastoni    | odikb:vittoria-altro-su-uno   |
|  3 | odikb:due-di-bastoni    | odikb:necessità-di-una-scelta |
|  4 | odikb:due-di-bastoni    | odikb:due-bastoni             |
|  5 | odikb:asso-di-bastoni   | odikb:scettro                 |
|  6 | odikb:asso-di-bastoni   | odikb:tronco                  |
|  7 | odikb:cinque-di-bastoni | odikb:vista-del-massacro      |
|  8 | odikb:cinque-di-bastoni | odikb:schianto-dei-tronchi    |
|  9 | odikb:cinque-di-bastoni | odikb:bosco                   |
| 10 | odikb:dieci-di-bastoni  | odikb:bosco                   |

### Coins

What are the meanings associated with cards that have suit Coins?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:denari.
    ?cardDeck odi:hasTypology odikb:numerale.
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
|  5 | bacodi:dieci-di-denari  | bacodi:età-dello-oro               |
|  6 | bacodi:dieci-di-denari  | bacodi:pagamento-per-uno-scherano  |
|  7 | bacodi:dieci-di-denari  | bacodi:ricchezza                   |
|  8 | bacodi:dieci-di-denari  | bacodi:eredità                     |
|  9 | bacodi:due-di-denari    | bacodi:due-denari                  |
| 10 | bacodi:due-di-denari    | bacodi:dualità-del-bene-e-del-male |

### Swords 

What are the meanings associated with cards that have suit Swords?

```
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:spade.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}
```

|    |        cardDeck       |                    meaning                    |
|----|-----------------------|-----------------------------------------------|
|  1 | bacodi:asso-di-spade  | bacodi:volontà-divina                         |
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
    ?cardDeck odi:hasSuit odikb:coppe.
    ?cardDeck odi:hasTypology odikb:numerale.
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

## The narrative function of court cards and triumph

Court cards are used by Calvino to represent each protagonist in the story (e.g. the *Cavaliere di Coppe* in *Storia dell'ingrato punito*). For this reason, interrogating the ontology to find out the semantic content of all the representations of the court cards was useful for two reasons: the first because the existence of cases in which the court cards do not have the 'protagonist' representation emerged, noting the non-exclusivity of this type of card with the role of protagonist cards (e.g. the *Fante di Bastoni* in *Storia dell'Orlando pazzo per amore* which represents Medoro); the second because it turns out that the court cards almost always represent a character (odi:Character, 12 occurrences), but with the presence of one occurrence in which the court card refers to an inanimate object (Trojan horse) and two occurrences, instead, concerning an event (removal of a leader, unforeseen). In this way, it was verified how Calvino prefers the court card typology to represent characters in stories.
Triumphs present more complex miniatures and this complexity stimulates the author's imagination, enriching the multiple possibilities of interpretation for the narrative events. In fact, the results of the seventh query are very diverse: some triumphs represent characters, others inanimate objects, still others events or places in history; finally, some refer to symbolic images.



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

# MACROCATEGORIA

## CARD (= set di query)

Descrizione del set di query

### Competency question id or brief title

Competency question in Natural Language

```SPARQL Query```

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
