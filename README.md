Some **Ti nspire CX CAS** "programs" that I've created to pass **Solid and Structural Mechanics** *(Scienza delle Costruzioni = SdC)* and **Fluid Mechanics** *(Meccanica dei Fluidi)* at Civil Engineering degree in UniTrento, Italy.
Techinically they are not scripts. They are just a sequence of actions made in "Notes" and with the built-in Spreadsheet. They works ;)

__I switch to italian, sorry__

# Indice file:
## SdC
  - **PLV**: Inserendo SOLO le prime 4 colonne della tabella *(ovvero lunghezza aste e le equazioni dei momenti delle tre strutture degradate)* e cambiando il numero beta nella seconda pagina *(corrispondente a quante aste si hanno)* permette di calcolare i momenti e le Eta di una struttera iperstatica 2 volte. E' poi possibile creare il sistema del PLV per trovare le incognite iperstatiche, ma non è automatizzato del tuttto. Occore inserire eventuali carichi termici, cedimenti e molle.
  
     <br/><img src="/img/s1.jpg" alt="drawing" width="180"/> <img src="/img/s2.jpg" alt="drawing" width="180"/> <img src="/img/s3.jpg" alt="drawing" width="180"/> <img src="/img/s4.jpg" alt="drawing" width="180"/>
## Meccanica dei fluidi 
(If you need the [Moody diagram](/img/Moody.pdf) here it is)
  - **IterMoody1:** Itera le f per trovare la velocità (e portata) in caso di piezometrici dinami e/o statici 
  
      <br/><img src="/img/1a.jpg" alt="drawing" width="180"/> <img src="/img/1b.jpg" alt="drawing" width="180"/> <img src="/img/1c.jpg" alt="drawing" width="180"/> <img src="/img/1d.jpg" alt="drawing" width="180"/>
  
  - **IterMoody2**: Itera le f nel caso reynolds sia fisso perché la portata o la velocità sono già note (oltre a e ed d). Se non sono note in partenza e occore calcolarle dal bilancio energetico: vedi *IterMoody5*
  
      <br/><img src="/img/2a.jpg" alt="drawing" width="180"/> <img src="/img/2b.jpg" alt="drawing" width="180"/> <img src="/img/2c.jpg" alt="drawing" width="180"/> <img src="/img/2d.jpg" alt="drawing" width="180"/>
  
  - **IterMoody3**: Calcola l'altezza di contrazione di vena e l'altezza di petto di un serbatoio con stramazzo
  
      <br/><img src="/img/3a.jpg" alt="drawing" width="180"/> <img src="/img/3b.jpg" alt="drawing" width="180"/> <img src="/img/3c.jpg" alt="drawing" width="180"/> <img src="/img/3d.jpg" alt="drawing" width="180"/>
  
  - **IterMoody4**: Calcola il tirante di moto uniforme e critico e la pendenza del fondo uniforme e critico
  
      <br/><img src="/img/4a.jpg" alt="drawing" width="180"/> <img src="/img/4b.jpg" alt="drawing" width="180"/> <img src="/img/4c.jpg" alt="drawing" width="180"/> <img src="/img/4d.jpg" alt="drawing" width="180"/>
  
  - **IterMoody5**: Itera le f nel caso reynolds sia variabile con la portata che però non è nota a priori. Viene dapprima trovata la portata dal bilancio energetico e poi iterata insieme alle f e reynolds (che variano a loro volta) fino la convergenza. *(Non è perfetto. Creare il sistema iniziale può essere complicato).*
  
      <br/><img src="/img/5a.jpg" alt="drawing" width="180"/> <img src="/img/5b.jpg" alt="drawing" width="180"/> <img src="/img/5c.jpg" alt="drawing" width="180"/> <img src="/img/5d.jpg" alt="drawing" width="180"/>
