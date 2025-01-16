# Exercicis de tot el tema

Com ja s'ha comentat a la introducció, i per no interferir entre nosaltres, cadascú es connectarà a la seua Base de Dades **f_grup_9999x** (on grup és el vostre grup p.ex. 1cfsg, 1cfsh... , 9999 són
les 4 últimes xifres del vostre DNI, i x la lletra del NIF).


L'esquema Entitat-Relació i l'esquema relacional és el següent:

![](factura.png)

En la Base de Dades anomenada **f_grup_9999x** (on grup és el vostre grup,
9999 són les 4 últimes xifres del vostre DNI, i x la lletra del NIF),
connectant com un usuari amb el mateix nom i contrasenya:

!!!note "Nota"
      Durant tots aquestos exercicis de DML pot ser molt convenient tenir obertes
      les dues connexions: la de **FACTURA** (per anar consultant) i la de
      **f_grup_9999x**, on grup és el vostre grup,
      9999 són les 4 últimes xifres del vostre DNI, i x la lletra del NIF.


**Ex_1** - Inserir en la taula **CATEGORIA** les següents files:

**cod_cat** | **descripcio**  
---|---  
BjcOlimpia | Components Bjc Seria Olimpia  
Legrand | Components marca Legrand  
IntMagn | Interruptor Magnetotérmico  
Niessen | Components Niesen Serie Lisa  
  
**Ex_2** - Inserir els següents articles.

**cod_art** | **descrip** | **preu** | **stock** | **stock_min** | **cod_cat**  
---|---|---|---|---|---  
B10028B | Cruzamiento Bjc Serie Olimpia | 4.38 | 2 | 1 | BjcOlimpia  
B10200B | Cruzamiento Bjc Olimpia Con Visor | 0.88 | 29 |  | BjcOlimpia  
L16550 | Cartucho Fusible Legrand T2 250 A | 5.89 | 1 | 1 | Legrand  
L16555 | Cartucho Fusible Legrand T2 315 A | 5.89 | 3 | 3 | Legrand  
IM2P10L | Interruptor Magnetotermico 2p, 4 | 14.84 | 2 | 1 | IntMagn  
N8008BA | Base Tt Lateral Niessen Trazo Bla | 4.38 | 6 | 6 | Niessen  
  
**Ex_3** - Inserir en la taula **CLIENT** tres files amb les següents dades

**cod_cli** | **nom** | **adreca** | **cp** | **cod_pob**  
---|---|---|---|---  
303 | MIRAVET SALA, MARIA MERCEDES | URBANIZACION EL BALCO, 84-11 |  |   
306 | SAMPEDRO SIMO, MARIA MERCEDES | FINELLO, 161 | 12217 |   
387 | TUR MARTIN, MANUEL FRANCISCO | CALLE PEDRO VIRUELA, 108-8 | 12008 |   
  
**Ex_4** - Inserir la següent factura:

**num_f** | **data** | **cod_cli** | **cod_ven** | **iva** | **dte**  
---|---|---|---|---|---  
6535 | 2015-01-01 | 306 |  | 21 | 10  

**num_f** | **num_l** | **cod_art** | **quant** | **preu** | **dte**  
---|---|---|---|---|---  
6535 | 1 | L16555 | 2 | 5.89 | 25  
  
**Ex_5** - Inserir la següent factura (aquesta té més d'una línia de factura).

**num_f** | **data** | **cod_cli** | **cod_ven** | **iva** | **dte**  
---|---|---|---|---|---  
6559 | 2015-02-16 | 387 |  | 10 | 10  

**num_f** | **num_l** | **cod_art** | **quant** | **preu** | **dte**  
---|---|---|---|---|---  
6559 | 1 | IM2P10L | 3 | 14.84 |   
6559 | 2 | N8008BA | 6 | 4.38 | 20  
  
**Ex_6** - Esborrar la factura **6559**. Comprovar que també s'han esborrat les
seues línies de factura

**Ex_7** - Esborrar els articles dels quals **no** tenim**stock mínim**.

**Ex_8** - Llevar tots els codis postals dels clients.

**Ex_9** - Pujar el preu dels articles de la categoria **BjcOlimpia** un **5%**
(el resultat serà que l'únic article d'aquesta categoria haurà passat d'un
preu de 4.38 a **4.60€**)


Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

