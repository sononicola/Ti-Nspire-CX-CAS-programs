Some **Ti nspire CX CAS** "programs" that I've created to pass **Solid and Structural Mechanics** *(Scienza delle Costruzioni = SdC)* and **Fluid Mechanics** *(Meccanica dei Fluidi)* at Civil Engineering degree in UniTrento, Italy.
Techinically they are not scripts. They are just a sequence of actions made in "Notes" and with the built-in Spreadsheet. They works ;)

__I switch to italian, sorry__

# Indice file:
## SdC
  - **PLV**: Inserendo SOLO le prime 4 colonne della tabella *(ovvero lunghezza aste e le equazioni dei momenti delle tre strutture degradate)* e cambiando il numero beta nella seconda pagina *(corrispondente a quante aste si hanno)* permette di calcolare i momenti e le Eta di una struttera iperstatica 2 volte. E' poi possibile creare il sistema del PLV per trovare le incognite iperstatiche, ma non è automatizzato del tuttto. Occore inserire eventuali carichi termici, cedimenti e molle.
  
     <br/><img src="/img/s1.jpg" alt="drawing" width="180"/> <img src="/img/s2.jpg" alt="drawing" width="180"/> <img src="/img/s3.jpg" alt="drawing" width="180"/> <img src="/img/s4.jpg" alt="drawing" width="180"/>
## Meccanica dei fluidi 
(If you need the [Moody diagram](/img/Moody.pdf) here it is)
  - **MF:** This is a library. You have to put into "MyLib" folder and then refresh libraries. It helps you to find f0, area, exc. using for example: mf\a(diam). It isn't necessary to have it with programs below.
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
    
   - **Spinte dinamiche**: Calcola le spinte dinamiche in un'intersezione di tubi. [PDF](/img/Versori%20entranti%20e%20uscenti.pdf) d'aiuto con versori entranti e uscenti.
  
      <br/><img src="/img/SD1.jpg" alt="drawing" width="180"/> <img src="/img/SD2.jpg" alt="drawing" width="180"/> <img src="/img/SD3.jpg" alt="drawing" width="180"/> <img src="/img/SD4.jpg" alt="drawing" width="180"/>
## Computational structural mechanics (FEM)
  - **SlaveMaster**: Calculates the displacements and deformations starting from the coordinates of the Master and Slave element. At the moment there are two version of this file. The one (page 2.1 - 2.4) that uses the program slavemaster_1() is the one more optimized to not block the calculator. I'm working to transform the other formulas.
  
     <br/><img src="/img/MecCompu1.jpg" alt="drawing" width="180"/> <img src="/img/MecCompu2.jpg" alt="drawing" width="180"/> <img src="/img/MecCompu3.jpg" alt="drawing" width="180"/> <img src="/img/MecCompu4.jpg" alt="drawing" width="180"/>   
 ## Structural Safety
  - **LoadCombination**: init version: compute Ultimate State Limit ULS (Stati Limiti Ultimi SLU) accordingly to Eurocode (EU) and NTC2018 (italian normative). Only gamma A1 coefficients
  
  Future versions TODO: add SLS combinations, add gamma A2 and gamma EQU


  <br/><img src="/img/LoadComb1.jpg" alt="drawing" width="180"/> <img src="/img/LoadComb2.jpg" alt="drawing" width="180"/> <img src="/img/LoadComb3.jpg" alt="drawing" width="180"/> <img src="/img/LoadComb4.jpg" alt="drawing" width="180"/>          
