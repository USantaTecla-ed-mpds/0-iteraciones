# Solucion de la Prueba en PlantUML

## Pregunta Nº1

- Modela con UML el cuadro de "Las Meninas de Velázquez" de tal forma que se observe qué diferencias existen con otros cuadros en los que el observador no se siente dentro de la escena (Pista: relaciones entre observador, personajes y posiciones)

* **anónimo**


* **lfcv00007**

[plantuml,lfcv00007,svg ]
....

Picture *--> "n" Character : composed by >
Observer --> Picture  : observe >
Character *--> Position
Character --> Observer : look at >
....


* **anggilb**

[enlace-1](https://www.plantuml.com/plantuml/uml/fPR1RkCs48RlV0f2zrqqEHhfOhER1d3hs46zcpsFfR7CXY9TaawGHLycnnReIzGlLbAIIMfi2q5xY4NE_9pvD1eo_6WT6BTh98ELTGPAnt-IsA1oZ9KIhENNIZGWMVVW4oxiJEj7eUfhzsM3YvL5yuI6zQlurH_ltlLh3X4-Ro04zg8uyd4KDDX7xHP5vs7TOlKRbcuOkRSntJvvuOLtg8G2Exa7ePpdAZXOdkodjBVWHBt3vOkgZ6vmCfLIeRNjojdTxP8bAVT9WyaJRur-qe-OHJHQDvEPBdquhThLmSB2Jz1BA97_oAzbkN_z3kPWBuLxyUOxg8oeIAfUWkf96At2UwTiQssmDdgdgXcktUHUMn7p3driEFK1xRPZIOvZpROFw6NIMpfSpqHYd-3vx3dH42BYPTGmJfLKELVPsYXP59zY-rNK6r8iucHaFWuMHJcN2QQ8HQI9gX5L9Szp7RaPjUHikOyAn_cec1AUxJBYZNpZdKPLOxr6fObi1UNZsSeH9oFp32jvY6YqOaHAgSxj0Ufbr30EzgOzGCM9RMk4Aj7QIJnPMwY3cHq6_M7iGnTtO6emmW7_WWOj54b4J_u7WHjd_29dTdYqRJrPJ9IVmDNBL7q3uNoK2y8rTBBXD6ESMbYXv1No1vHWIrqGxTb_Kg4hGTgJj2Jz6URBCUPBDfpcTVtdBtvTxwot0r-2QOJFgyCxBBNJ3RneKz3L__yjBjDRLCzWrhJYdP5rZs4NxFy6_cd_QbPQGX4LPuX84yGDvNcwbOI3Lh4pikwHSSn5gUN-rV9xD2wqezCzovkhSmoJ5qNNa-u6qc7eclc__nPQrzd60n6-1tdBtihwP_QUDm9h7RhPNnD-t-7t8jECLvmUbnubveauvGQsQBH20XJjB8w6JL2YXD2ZNwNKKEIgyGhrNBH6SNr2gtTWAeBLsbZxct2khhwgHwMVrOSFqVNsqaI4BdPUcMQ5He9G12Bpi6oSrUTdRVT_yhb0D_XqH3tE6C_kH9Wj9mtbWqpLuRAxQ3qjwf4pz2Vj2Qg9iNMFb5y1ZD4cpz1PEbfotlIkxX4CnG_ltryKnmbzBUn6FziZQII8YaWIwaQ-Ip2ny9DzYLkKOejy-b0SFEDLJmIztE1Q-eHPPlyfaRP4QsFjxt2R251GHCTRSn_qnybbw8LFExcwcCmEmvOWELWQZbuue-poNAXBbePZDvqdKC9kXAhljL2E3QTZ2qkZhLsi5wP2TODBK4v0hTbfCv_qnrTr0mxzpE_x-I_pnRUvt_VnLFJPpaJzYAhQDV9V)


* **asanera**

[plantuml,asanera,svg]
....
title Cuadro de las Meninas de Velazques

object planeA
object planeB
object planeC

object me
object observer
object king
object queen
object infantaMargarita
object isabelDeVelasco
object mariaAgustina

object mariBarbola
object nicolasitoPertusato
object marcelaDeUlloa
object diegoRuizAzcona
object joseNietoVelazquez
object diegoVelazquez
object dog


observer -->me
observer o--> king
observer o--> queen
planeA o--> infantaMargarita
planeA *-- mariaAgustina
planeA *-- isabelDeVelasco
planeA *-- mariBarbola
planeA *-- nicolasitoPertusato
planeA *-- dog

planeB *-- diegoVelazquez
planeB *-- marcelaDeUlloa
planeB *-- diegoRuizAzcona


planeC o--> king
planeC o--> queen
planeC o-->infantaMargarita
planeC *-- joseNietoVelazquez

object meninas
meninas *-- planeA
meninas *-- planeB
meninas *-- planeC
....

* **borxdev**

[enlace-1](https://github.com/borxdev/master-escuelait/tree/main/4_meninas)

[enlace-2](https://www.plantuml.com/plantuml/svg/TL91QiCm4Bph5JeNv1S4aq2XbmGAXTwtzk9kQw_TrTg5_2PloSUgHBOgDyt9sfdPOMVmrYk8ZbrhM_07P6Bmhd_xm4gzgmaQWSuO9MtHxi7RMLBOLspFf-FNY4TZejvEs494Pa3VyHc8bRZP9_UCVAcGCMqJVgCiqsVOIT91Y2lq_W3IW932GdYKwMfU4oPrHtM3kkFwiM-Ia5HH0lOqWeHOl13XN6I_6uO-t8dfcD09ULsc2dY2p5-a5sDIt8rpipv1rhdoJdmJWsvS6JF6iIZAE_9_uOVWdmeqo-k2pfVaq6rzERlkC6TMHQvMRjfShrtxoQ6_BUVSNAw9tmiIUub1VWNHDblO8jVXn_q1)



* **mabernabe**

[enlace-1](https://www.planttext.com/api/plantuml/svg/ZPLBQnin4CVl-XJ3djB26kBZKamWz122dPn2qjlO6Zjgrj9MaXESjD-zsjLhimzQWn7C_Fxpq8pOAsDHszEnPcnDKaWqzoYa5V80NqkktcIvWk9oMS3rCshSMTBiRcj8lvA6HKrxkrZ1GCWI2jz--nXmEsF_BlSeBRjNHbYXP7RSdQmHd6BC230OeJTo4ap98bSiYr3eH26TtFKMpj1vwYYs7EnpnRLTccjrQchw1vagY9cY8v9bkUf5cv_DMcYjDFC735ICxMeq9a3mmI1Vtu5i3utcYo_i3yEjiMrruDL9yi6SwD4XxdZgI0_CDDdbW_Rl-1yTpvZQ_YGNkMWqSXMwgWRT5G1ee4yasH7r0RMmMFdDyMYoZhbOJ3Mz9WDz6aECSrPLd7tHacULN2hOKuQPQ_0fXdGAiwTQD7Jpi7O5eCIgDvGkuy2VTAzKu_kl4xrNOMTzdcGUW_zr5ICwJopm3vyJvtd5nn85RrZNVlCgVtWkcndhppYkT1xcb7Tu7LDCleCfRoz_0jsxIUKt-GKEasNfXFEi5elLfwKzAuUD1Z_GJI7f2ihUTIHll-hnkAIo1CM6Y4CO11Tuq7W4gq18BdRe0FjCyD9k6g3aQJa1DRaH6RKJ3kAjeWKD7WcQ-Afzr6utDqksMRgkHmsqlokIlFsk_0K0)

* **diego-novoa**


* **anónimo**

[plantuml, segundoAnonimo, svg]
....
object meninas
object ":Observer" as Observer
object ":Foreground" as Foreground
object ":Background" as Background
object ":ThirdPlane" as ThirdPlane
object margarita
object ":Menina" as Menina1
object ":Menina" as Menina2
object ":Canvas" as Canvas
object velazquez
object ":Servant" as Servant1
object ":Servant" as Servant2
object mirror
object felipeIV
object marianaDeAustria
object ":Personage" as Personage

meninas *--> Foreground
meninas *--> Background
meninas *--> ThirdPlane

Foreground *--> margarita
Foreground *--> Menina1
Foreground *--> Menina2
Foreground *--> Canvas

Background *--> velazquez
Background *--> Servant1
Background *--> Servant2

ThirdPlane *--> mirror
ThirdPlane *--> Personage

mirror *--> felipeIV
mirror *--> marianaDeAustria
mirror --> Observer

Observer ..> meninas
velazquez --> Canvas
Canvas o--> meninas
Canvas o--> mirror

....

* *lab-lovalace*

[Meninas:](link:https://github.com/USantaTecla-ed-mpds/lab-lovalace/blob/master/20220217_Meninas.pdf) .. El archivo es el que se llama 20220217_Meninas.pdf



## Pregunta Nº2

- Dada la tabla de verdad (combinaciones de cierto y falso) de la "puerta" XOR (especificación en tabla verde de https://es.wikipedia.org/wiki/Puerta_XOR), escribe la expresión lógica de la salida (tercera columna) correspondiente a la entrada (primeras 2 columnas)

* **anónimo**

A <> B = 1


* **lfcv00007**


* **anggilb**

s = a.!b + !a.b



* *asanera*

Q = (A ⊕ B) = A.B + A.B


* **borxdev**

~A && B || A && ~B


* **mabernabe**

SALIDA = (A && !B) || (!A && B



* **diego-novoa**


* **anónimo**

A == B = O
A != B = 1
....

* **lab-lovalace**

a XOR b = (a AND NOT b) OR (NOT a AND b)



## Pregunta Nº3


## Pregunta Nº4


## Pregunta Nº5