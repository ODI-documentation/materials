# La semantica

## La semiotica dei semi

Le prime quattro query presentano dei risultati significativi per lo studio della semiotica dei semi dei tarocchi (query da Q1 a Q7). Per quanto riguarda il seme di Bastoni, la percentuale maggiore mostra che il rimando è al bosco e, in generale, all’ambientazione boschiva del Castello. Nei casi in cui la semantica si discosti dall’ambientazione, emerge come a definire il significato della carta sia il numero: il Due di Bastoni viene, infatti, utilizzato per esprimere una dualità o una scelta tra due situazioni (cfr. tabella 1, risultati 1; 2; 3); l’Asso di Bastoni, invece, può rimandare, oltre all’albero, al potere ed al suo simbolo materiale (cfr. ivi, risultati 5; 6). A differenza dei numerali con seme di Bastoni, quelli di Denari rimandano, invece, a due campi semantici nettamente opposti: il primo è quello del potere terreno, della ricchezza e della materialità (cfr. tabella 2, risultati 5; 7; 8); il secondo, invece, ha a che fare con il cielo, con il divino e con l’immateriale (cfr. ivi, risultati 2; 3; 10). Tra i due campi semantici spicca, tuttavia, il primo rispetto al secondo. La percentuale maggiore dei risultati ottenuti per la semantica dei numerali con seme di Spade rimanda all’ambito bellico (cfr. tabella 3, risultati 3; 5; 7; 9; 10); a volte, può far riferimento, più specificatamente, alla difesa (cfr. ivi, risultati 6; 8). L’utilizzo narrativo dei numerali di Coppe risulta, invece, meno definito rispetto agli altri tre fino ad ora delineati. Dai risultati è possibile notare una grande percentuale che rimanda al banchetto e al ristoro (cfr. tabella 4, risultati 2; 4; 6; 11); sono presenti, tuttavia, altri rimandi come quello legato al benessere (cfr. ivi, risultati 3; 18) o all’amore (cfr. ivi, risultato 15; Appendice D, risultati 21; 23).

### Bastoni

Quali sono i significati associati alle carte che hanno seme Bastoni?

`select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:bastoni.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`

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
| 11 | odikb:nove-di-bastoni   | odikb:bosco                   |

### Denari

Quali sono i significati associati alle carte che hanno seme Denari?

`select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:denari.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`

### Spade 

Quali sono i significati associati alle carte che hanno seme Spade?

`select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:spade.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`

|    |       cardDeck       |                   meaning                   |
|----|----------------------|---------------------------------------------|
|  1 | odikb:asso-di-spade  | odikb:volontà-divina                        |
|  9 | odikb:due-di-spade   | odikb:duello                                |
| 10 | odikb:nove-di-spade  | odikb:esito-della-guerra                    |

### Coppe

Quali sono i significati associati alle carte che hanno seme Coppe?

`select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:coppe.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`

|   |        cardDeck       |            meaning            |
|---|-----------------------|-------------------------------|
| 1 | odikb:asso-di-coppe   | odikb:coppa-sacra             |
| 2 | odikb:asso-di-coppe   | odikb:vino                    |
| 3 | odikb:asso-di-coppe   | odikb:fonte-della-vita        |
| 4 | odikb:asso-di-coppe   | odikb:bevuta-del-protagonista |
| 5 | odikb:cinque-di-coppe | odikb:coppe                   |
| 6 | odikb:cinque-di-coppe | odikb:brindisi                |
| 7 | odikb:cinque-di-coppe | odikb:discorso                |
| 8 | odikb:cinque-di-coppe | odikb:rintocchi               |

## La semiotica dei semi2

Le prime quattro query presentano dei risultati significativi per lo studio della semiotica dei semi dei tarocchi (query da Q1 a Q7). Per quanto riguarda il seme di Bastoni, la percentuale maggiore mostra che il rimando è al bosco e, in generale, all’ambientazione boschiva del Castello. Nei casi in cui la semantica si discosti dall’ambientazione, emerge come a definire il significato della carta sia il numero: il Due di Bastoni viene, infatti, utilizzato per esprimere una dualità o una scelta tra due situazioni (cfr. tabella 1, risultati 1; 2; 3); l’Asso di Bastoni, invece, può rimandare, oltre all’albero, al potere ed al suo simbolo materiale (cfr. ivi, risultati 5; 6). A differenza dei numerali con seme di Bastoni, quelli di Denari rimandano, invece, a due campi semantici nettamente opposti: il primo è quello del potere terreno, della ricchezza e della materialità (cfr. tabella 2, risultati 5; 7; 8); il secondo, invece, ha a che fare con il cielo, con il divino e con l’immateriale (cfr. ivi, risultati 2; 3; 10). Tra i due campi semantici spicca, tuttavia, il primo rispetto al secondo. La percentuale maggiore dei risultati ottenuti per la semantica dei numerali con seme di Spade rimanda all’ambito bellico (cfr. tabella 3, risultati 3; 5; 7; 9; 10); a volte, può far riferimento, più specificatamente, alla difesa (cfr. ivi, risultati 6; 8). L’utilizzo narrativo dei numerali di Coppe risulta, invece, meno definito rispetto agli altri tre fino ad ora delineati. Dai risultati è possibile notare una grande percentuale che rimanda al banchetto e al ristoro (cfr. tabella 4, risultati 2; 4; 6; 11); sono presenti, tuttavia, altri rimandi come quello legato al benessere (cfr. ivi, risultati 3; 18) o all’amore (cfr. ivi, risultato 15; Appendice D, risultati 21; 23).

### Bastoni2

Quali sono i significati associati alle carte che hanno seme Bastoni?

`select ?cardDeck ?meaning
select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:bastoni.
    ?cardDeck odi:hasSuit odikb:coppe.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`

|    |         cardDeck        |            meaning            |
|----|---------------------------|-------------------------------|
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
| 11 | odikb:nove-di-bastoni   | odikb:bosco                   |



### Denari2

Quali sono i significati associati alle carte che hanno seme Denari?

`select ?cardDeck ?meaning
where {
    ?cardDeck a odi:DeckCard.
    ?cardDeck odi:hasSuit odikb:denari.
    ?cardDeck odi:hasTypology odikb:numerale.
    ?cardStory odi:specifies ?cardDeck.
    ?cardStory odi:carriesRepresentation ?representation.
    ?representation odi:hasMeaningOf ?meaning.
}`


|   |        cardDeck        |              meaning             |
|---|------------------------|----------------------------------|
| 1 | odikb:asso-di-denari   | odikb:elemosina                  |
| 2 | odikb:asso-di-denari   | odikb:luna                       |
| 3 | odikb:cinque-di-denari | odikb:luce-del-mattino           |
| 4 | odikb:cinque-di-denari | odikb:spreco                     |
| 5 | odikb:dieci-di-denari  | odikb:età-dello-oro              |
| 6 | odikb:dieci-di-denari  | odikb:pagamento-per-uno-scherano |
| 7 | odikb:dieci-di-denari  | odikb:ricchezza                  |
| 8 | odikb:dieci-di-denari  | odikb:eredità                    |




# MACROCATEGORIA

## CARD (= set di query)

Descrizione del set di query

### Competency question id or brief title

Competency question in Natural Language

`SPARQL Query`

| Syntax      | Description |
| ----------- | ----------- |
| Header      | Title       |
| Paragraph   | Text        |
