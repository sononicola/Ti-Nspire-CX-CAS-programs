Some **Ti nspire CX CAS** "programs" that I've created to pass "scienza delle costruzioni" and "Meccanica dei Fluidi" at UniTrento
Techinically they are not scripts. They are just a sequence of actions made in "Notes" and the built-in Spreadsheet. They works ;)

__I switch to italian, sorry__

# Indice file:
* SDC
  - PLV: Inserendo SOLO le prime 4 colonne della tabella *(ovvero lunghezza aste e le equazioni dei momenti delle tre strutture degradate)* e cambiando il numero beta nella seconda pagina *(corrispondente a quante aste si hanno)* permette di calcolare i momenti e le Eta di una struttera iperstatica 2 volte. E' poi possibile creare il sistema del PLV per trovare le incognite iperstatiche, ma non è automatizzato del tuttto. Occore inserire eventuali carichi termici, cedimenti e molle.
* Meccanica dei fluidi
  - IterMoody1: Itera le f per trovare la velocità (e portata) in caso di piezometrici dinami e/o statici
  
  *In 1.2 inserire e,diametro,delta, lunghezza tubo e la formula della velocità ricavata eguagliando le energie dei due piezometri e contando le perdite. In 1.3 vengono iterate le f partendo dall'ipotesi di tubo scabro, calcolando U0 e Reynolds 0. Leggere i valori di U(i) corrispondenti a quando le f sono uguali alla terza o quarta cifra decimale. Viene poi calcolata la portata.  Non modificare nulla in 1.3* e 1.4.*
