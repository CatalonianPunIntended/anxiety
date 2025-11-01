# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[JUGA!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: Abans de començar, com voldries llegir *tu*?

`publish("show_options_bottom")`

# intro-start-2

n3: Ara, començem amb la història...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: AIXÒ ÉS UN ÉSSER HUMÀ

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: I AQUESTA ÉS L'ANSIETAT DE L'ÉSSER HUMÀ

n: _TU_ ETS L'ANSIETAT

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Nop. No, no, no t'escoltaré. Miraré el mòbil.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: HAS DE PROTEGIR AL TEU ÉSSER HUMÀ DEL *PERILL*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: Espant! Estàs malgastant la teva vida al Twitter! Un altre cop!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: Sí, em pregunto perquè no escolto als meus pensaments més sovint.

`hong({eyes:"neutral"});`

n: RÀPID, AVISA'LS D'UN *PERILL!*

```
bb({eyes:"look"});
```

[Oh no, fixa't en aquella noticia terrible!](#act1d_news)

[Oh no, una indirecta cap a *nosaltres*?](#act1d_subtweet)

[Ei, un GIF d'un gatet bevent llet](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: Ei, és molt maco, l'acabo de repiular, penso q--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: ELS GATS NO PODEN DIGERIR LLET I SOM GENT TERRIBLE PER GAUDIR L'ABÚS ANIMAL

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```


