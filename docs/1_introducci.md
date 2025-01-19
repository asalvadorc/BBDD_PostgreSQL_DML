# 1. Introducció

La sentència **SELECT** (Data Query Language) ens permetia consultar la informació ja introduïda. Les
sentències de **DDL** (Data Definition Language) ens permeten crear (o modificar o esborrar) les estructures:
taules, índex, o altres objectes.

Les sentències de **DML** (Data Manipulation Language) són aquelles que ens han de permetre alterar les dades, és a dir, l'estructura de les taules quedarà intancta, i només es modificarà
el seu contingut: 


  * **INSERT** , per a introduir files noves a la taula.
  

  * **DELETE** , per a esborrar files senceres de la taula.
  

  * **UPDATE** , per a modificar el contigut d'una o més files ja existents.


Durant tota aquesta part de SQL farem consultes per a modificar les dades de les taules.

No ens convé en absolut treballar sobre la Base de Dades **geo** ni sobre
**factura** , ja que el que faríem seria "boicotejar-nos" entre nosaltres.
Treballarem amb dues Bases de Dades noves:

  * **proves** (connectant-nos com l'usuari **proves**): servirà per a fer proves, com el seu propi nom indica. Tots els exemples els farem en aquesta BD.
  * **f_grup_9999x** , on grup és el codi del vostre grup (p.ex 1cfsg, 1cfsj, 1cfsl...), 9999 seran les 4 últimes xifres del vostre DNI, i x és la lletra del vostre NIF. És a dir, tindreu una Base de Dades per a cadascú de vosaltres, i un usuari amb el mateix nom. És on haureu de treballar els exercicis.

Us recomane vivament que us creeu una altra connexió per a cadascuna de les
Bases de Dades anteriors. D'aquesta manera, segurament en tindreu quatre
connexions: la de **geo** , la de **factura** , la de **proves** i la de
**f_grup_9999x** (substituint per les dades del vostre grup i NIF)



Llicenciat sota la  [Llicència Creative Commons Reconeixement NoComercial
CompartirIgual 3.0](http://creativecommons.org/licenses/by-nc-sa/3.0/)

