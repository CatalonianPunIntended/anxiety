# act1

```
SceneSetup.act1();
```

(...300)

n: I AQUESTA ÉS L'ANSIETAT DE L'ÉSSER HUMÀ

n: _TU_ ETS L'ANSIETAT

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: Oh, ei! Hem tornat aquí?

`hong({eyes:"0_neutral"})`

n: HAS DE PROTEGIR AL TEU ÉSSER HUMÀ DEL *PERILL*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FET, JUGAR AQUEST JOC DE NOU EL POSA EN *PERILL* ARA MATEIX

n: RÀPID, AVISEU-LO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humà! Escolta, estem en perill! Qui està jugant ara mateix...

[...ens torturarà als dos de nou!](#act1_replay_torture)

[...no trobarà un final alternatiu!](#act1_replay_alternate)

[...experimentarà dissonància ludonarrativa!](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: Ens farà cargolar-nos en una pilota i plorarem!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: Ens farà destruir el teu telèfon per donar-te un atac de pànic!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: Ens farà *NO* donar un cop de puny al hoste de la festa!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: Ens farà donar un cop de puny al Simpàtic Hoste Antivilà!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: D'acord, al menys potser no saltem del sostre aques--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: ENS FARÀ SALTAR DEL SOSTRE.
{{/if}}

`bb({body:"fear"});`

b: TOTES AQUESTES NOVES I TERRIBLES COSES ENS PASARAN, I DESPRÉS--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Sí, la història en si és la mateixa, però cada capítol té dos possibles finals, a més de totes les opcions de diàleg ramifica--

`bb({body:"fear"});`

b: Qui sigui qui jugui estarà decebut, tancarà aquesta finestra, eliminarà el programari i després--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: Què dius de distribucions?

`bb({eyes:"normal"});`

b: L'arc de la història parlava de com pots *DECIDIR* per construir una colaboració sana amb les teves pors,

`bb({eyes:"normal_right"});`

b: Però rejugar el joc et donarà la mateixa història, implicant que les teves *DECISIONS* no importen,

`bb({eyes:"narrow_eyebrow"});`

b: Doncs mostrarà una contradicció entre el missatges del joc i les seves mecàniques,

`bb({eyes:"fear"});`

b: I terminarà desfent els fils d'aquest univers narratiu,

`bb({body:"fear"});`

b: I finalment nosaltres--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: MORIREEEEEEEEEEEEM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: Vinga tornem als nostres papers.

```
Game.clearText();
```

n4: (DEIXA QUE LA _TEVA_ ANSIETAT BLA BLA BLA ESCULL EL QUE S'APROXIMI MÉS A LES _TEVES_ PORS BLA BLA BLA JA SAPS COM VA)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: Oh, bé, ha tornat el meu llop. Fantàààààstic.

`hong({eyes:"0_neutral"})`

n: HAS DE PROTEGIR AL TEU HUMÀ DEL *PERILL*

`bb({eyes:"look", mouth:"small_lock"})`

n: DE FET, AQUELL SÀNDVITX DE NOUS EL POSA EN *PERILL* ARA MATEIX

n: RÀPID, AVISEU-LO!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: Humà! Escolta, estem en perill! El perill és...

`bb({body:"squeeze"})`

n4: (DEIXA QUE LA _TEVA_ ANSIETAT VINGUI A JUGAR! ESCULL EL QUE S'APROXIMI MÉS A LES _TEVES_ PORS)

(#act1_normal_choice)

# act1_normal_choice

[Estem menjant sols! Un altre cop!](#act1a_alone) `bb({body:"squeeze_talk"})`

[Menjant no sóm productius!](#act1a_productive) `bb({body:"squeeze_talk"})`

[Aquest pa blanc és nociu per nosaltres!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: No saps que la solitud és associada a la mort prematura tant com prendre's 15 cigarretes al dia?-

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: Ehm, gràcies per citar les teves fonts però--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: Que vol dir que si no parlem amb algú *ara mateix* nosaltres-

`bb({body:"panic"})`

b: MORIREEEEEEEEEEEEM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: HAS FET SERVIR *LA POR A L'ABANDONAMENT*

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: Treu el portàtil i fes alguna cosa ara mateix!

`hong({eyes:"0_annoyed"})`

h: Ehm, no m'agradaria tenir molles al tecla--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Si no contribuïm al cos de la societat serem uns paràsits de la societat!

b: El cos de la societat anirà al doctor per a societats, es medicarà per matar als paràsits de la societat i després--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: MORIREEEEEEEEEEEEM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: HAS FET SERVIR LA *POR A SER UNA MALA PERSONA*

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: Han pogut replicar els es--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: El blat processat augmentarà el sucre en sang i hauran d'amputar-nos totes les extremitats i després--

`bb({body:"panic"})`

b: MORIREEEEEEEEEEEEM

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: HAS FET SERVIR LA *POR AL DANY FÍSIC*

(#act1b)

# act1b

n: ÉS MOLT EFECTIU

`bb({mouth:"smile", eyes:"smile"});`

b: Veus, humà? Soc el teu lleial llop guardià!

`bb({body:"pride_talk"});`

b: Creu el que et digui el cor! Els teus sentiments sempre són vàlids!

`bb({body:"pride"});`

n: FES QUE LA SEVA BARRA D'ENERGIA ARRIBI A ZERO

n: PER PROTEGIR LES SEVES INTEGRITATS FÍSIQUES + SOCIALS + MORALS, POTS FER SERVIR:

n: LA POR AL *DANY FÍSIC* #harm#

n: LA POR A LA *MARGINACIÓ* #alone#

n: I LA POR A *SER UNA MALA PERSONA* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (CONSELL: ESCULL LES OPCIONS QUE PERSONALMENT COINCIDEIXIN AMB LES TEVES PORS MÉS PROFUNDES I FOSQUES!~)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: saps què? potser estaria bé mirar el telèfon.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: PROTEGEIX AL TEU ÉSSER HUMÀ

n: DEL MÓN. D'ALTRA GENT. DE SI MATEIX.

n: BONA SORT

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: RONDA U: *LLUITA!*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: Huh. Les recomanacions de Facebook diuen que hi ha una festa aquest cap de setmana.

`bb({eyes:"uncertain"});`

b: Però aquest paio no fa una festa *cada* cap de setmana?

`bb({eyes:"uncertain_right"});`

b: Quina mena de buit interior intenten emplenar? Han de tenir un problema ben gros!

`hong({eyes:"surprise"});`

h: Espera, a més m'ha enviat l'invitació?

`bb({eyes:"fear", mouth:"normal"});`

b: Ara...!

[Accepta-la, o ens morirem sols!](#act1c_loner)

[Rebutja-la, estarà tot ple de drogues!](#act1c_drugs)

[Ignora-la, només fem que les festes siguin tristes.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: Quinze cigarretes al dia, humà! Quinze!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: I ningú anirà al nostre funeral, tiraran les nostres restes al oceà, ens menjarà una balena,
{{/if}}

{{if !_.fifteencigs}}
b: i ens tornarem en CACA DE BALENA!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: Així que hauriem d'anar a la festa!
{{/if}}

{{if _.parasite}}
b: Només obre el portàtil perquè poguem treballar, i no ser uns paràsits de la societat.
{{/if}}

{{if _.whitebread}}
b: Sempre que no ens donin PA BLANC
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: MARE MEVA. Si et callaràs, vinga.

h: Dirè que sí.

{{if _.whalepoop}}
b: Caca de balena, humà! Caca de balena!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: o pitjor encara... PA BLANC
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: Ens donarà una sobredosi de metanfetamina i pa blanc que no seran capaços de ficar el nostre cos gras al crematori!
{{/if}}

{{if !_.whitebread}}
b: Ens donarà una sobredosi de tantes drogues que la mort es preguntarà com el nostre cos *ja estava* embalsamat!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: A més, no podem anar de festa, hem de treballar o serem un terrible paràsit de la societat!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: MARE MEVA. Si et callaràs, vinga.

h: Dirè que no.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: Tot el que fem és plorar a una cantonada sobre com la solitud és tan mortal com 15 cigarretes al dia.
{{/if}}

{{if _.parasite}}
b: Tot el que fem a les festes és preocupar-nos sobre com hauriem de ser productius.
{{/if}}

{{if _.whitebread}}
b: Tot el que fem es preocupar-nos sobre com les opcions de menjar no salutable ens poden matar.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: ja em pregunto el per què.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: Així que si anem se sentiran malament, però si no, també se sentiran malament!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: TOT EL QUE FEM ÉS FER QUE LA GENT SE SENTI MALAMENT, AIXÍ QUE HAURÍEM DE SENTIR-NOS MALAMENT

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: Agh. Si et callaràs, vinga.

h: Ignorarè la invitació.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: Ara. Facebook és massa. Necessito alguna cosa més calmant, que produeixi menys ansietat.

`hong({eyes:"neutral"});`

h: Què hi ha de nou al Twitter?

`bb({eyes:"look"});`

[Oh no, fixa't en aquella noticia terrible!](#act1d_news)

[Oh no, una indirecta cap a *nosaltres*?](#act1d_subtweet)

[Ei, un GIF d'un gatet bevent llet](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: Déu meu, realment sembla que el món estigui en flames, no?

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: Sembla que tot està acabant, que tot està morint i que tots estem comdenats i que no podem fer res en contra.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: Fem un retwit d'aquesta història!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: D'acord, faré una repiulada, només no parlis tant!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: A prendre per cul, mirem l'Snapchat.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: És un subtwit! Un subtwit molt, molt difícil de veure!

`hong({eyes:"annoyed"});`

h: Potser no ho és?

`bb({eyes:"narrow", mouth:"small"});`

b: però i si tothom parla darrere nostre

h: No ho esta--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: EN FRONT DELS NOSTRES NASSOS

`hong({eyes:"sad", mouth:"sad"});`

h: Jo n--

`bb({eyes:"narrow", mouth:"small"});`

b: i si *fos així*

h: C--

`bb({eyes:"narrow_eyebrow"});`

b: i si *fos així*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: d'a-CORD, provaré l'Snapchat.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: Ei, és molt maco, l'acabo de repiular, penso q--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: ELS GATS NO PODEN DIGERIR LLET I SOM GENT TERRIBLE PER DISFRUTAR L'ABÚS ANIMAL

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: d'a-CORD, provaré l'Snapchat.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: Ah, fotos d'ahir a la nit. *Així* són les festes setmanals.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: Buf, sembla massa ocupat per a la meva ansietat.

h: Potser no hauria haver acceptat la invitació?

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[Canviar la nostra resposta? Com uns idiotes?!](#act1e_yes_dontchange)

[Canviem la nostra resposta! Està massa ple!](#act1e_yes_changetono)

{{if _.subtweet}}
[Sí, ens estaven subtwitejant definitivament.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, hem retwitejat sense verificar.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Saps que tens una postura molt dolenta?](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Comptaven amb que nosaltres anèssim i ara els decebem? Vols morir sola?!

{{if _.fifteencigs}}
b: QUINZE. CIGARRETES.
{{/if}}

{{if _.whalepoop}}
b: CACA. DE BALENA.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Calla calla, ho deixo igual!

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: No coneixes les estampides humanes?

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: En 2003 un club nocturn a Rhode Island va tenir un incendi i el pànic va fer que la gent taponés les sortides, així que 100 persones van estar cremades a la mort-

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: VOLS QUE AIXÒ ENS PASSI-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: QUE NO QUE NO QUE NO QUE NO QUE NO QUE NO QUE NO QUE NO QUE N-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Calla calla, ja canviaré la resposta a no! Déu meu!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembla molt divertit.

h: Potser era millor acceptar la invitació?

`bb({mouth:"normal", eyes:"normal"});`

[Canviar la nostra resposta? Com uns idiotes?!](#act1e_no_dontchange)

[Canviem la nostra resposta! No volem morir sols!](#act1e_no_changetoyes)

{{if _.subtweet}}
[Sí, definitivament ens subpiulen.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[Espera, hem repiulat sense verificar.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[Saps que tens una postura molt dolenta?](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: Tothom ens estava esperant!

b: ...només perquè nosaltres els deixèssim sols amb una festa divertida sense cretins {{if _.whitebread}}menjadors de pa blanc{{/if}} com nosaltre--


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Calla calla, ho deixaré tal qual!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: La solitud crònica augmenta els nostres nivells de cortisol, a més del risc a sofrir una malaltia o atac cardiovascular!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: QUINZE. CIGARRETES.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Calla calla, canviaré la meva resposta a sí! Déu meu!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Totes les piulades problemàtiques han tornat a turmentar-nos!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: Ens assenyalaran i cancel·laran i ens arrossegaran amb una corda lligada a un cavall a través de l'autovia de la informació!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Per què ets així?!

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Estem transmetent desinformació! Estem destruïnt la nostra credibilitat amb només un clic!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Som la raó per la qual el fascisme s'alçarà des de les runes de la democràcia!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: Per què ets així?!

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Vols una esquena que sembli un pretzel?! Canvia la teva postura!

```
bb({body:"meta"});
```

b: Això també va per tu.

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: Per què ets així?!

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: Hm... sembla molt divertit.

h: Potser hauria de mirar la invitació?

`bb({mouth:"normal", eyes:"normal"});`

[Ignora-ho, no cambiarà el fet que som uns aixafaguitarres](#act1e_ignore_continue)

[Espera, accepta-la.](#act1e_ignore_changetoyes)

[Espera, rebutja-la.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: No és una mica de mala educació ignorar-los?

`bb({eyes:"normal_right"});`

b: Els altres sempre estan *ignorant-nos*, així que

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: diguem que ja està solucionat.

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: M'estàs... deixant que em diverteixi?

b: Sigui, vull dir, la solitud ens *pot* matar.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: Està massa ple. Les multituds són perilloses.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: El que sigui. Una nova notificació de Tinder.

`bb({eyes:"uncertain"})`

b: Espera, aquella aplicació per lligar?

`hong({eyes:"annoyed"})`

h: No és una aplicació per lligar, només és una forma de conèixer a gent no--

`bb({eyes:"narrow"})`

b: És una aplicació per lligar.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: Oh, tinc un «match»! Sembla agradable!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: Si us plau no ho arruïnis to--

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: PERILL PERILL PERILL PERILL PERILL PERILL

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[Estem sent *utilitzats* per altra gent.](#act1f_used_by_others)

[Estem *utilitzant* a altra gent.](#act1f_using_others)

[EL TEU «MATCH» ÉS UN ASSASSÍ EN SÉRIE](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: Parelles escollides a l'atzar poden emplenar el forat que tens allà abaix,

b: però mai podran emplenar el forat que tens...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *aqui*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: El que vull transmetre és que MORIREM SOLS

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: Creus que els genitals de la resta són com Pokémons per obtenir?

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: ♫ (tema d'obertura de pokémon)-

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ Arribarè a ser un ^maso^-

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ El millor que hi pugui haver-

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ Cuixes i ^cul^, tot voluptuós-

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ i l'altre amb els ^collons^!-

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ MÒN-PERVERTIT! FES'TE-LS TOTS TE-

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: El que vull dir és que som uns manipuladors.

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: Et tiraran a un pou i et forçaran a menjar pa blanc fins que siguis tan grossa perquè puguin fer servir la teva pell com un vestit!
{{/if}}

{{if _.parasite}}
b: Et forçaran a fer servir un temporitzador pomodoro i et diran «HAURIES DE SER MÉS PRODUCTIVA MALEÏT PARÀSIT»
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Et destrossarà els músculs per fer confetti, farà de les teves entranyes serpentines, i de la teva sang una ponxera!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: Què et sembla AIXÒ en comparació amb una festa?!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: n'estic fart d'aquest joc.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}«la solitud ens matarà»... {{/if}}
{{if _.parasite}}«som paràssits de la societat»... {{/if}}
{{if _.whitebread}}«no mengis això, ens matarà»... {{/if}}
{{if _.subtweet}}«parlen darrere nostre»... {{/if}}
{{if _.badnews}}«el món està en flames»... {{/if}}
{{if _.hookuphole}}«morirem sols»... {{/if}}
{{if _.serialkiller}}«ell és un assassí en sèrie»... {{/if}}
{{if _.catmilk}}«els gats no poden digerir llet»... {{/if}}
{{if _.pokemon}}una cançó paròdia ^molt fotuda^... {{/if}}

h: només vull viure la meva vida.

h: només vull parar de... sofrir d'aquesta forma.

`bb({eyes:"look_sad"});`

b: Ei... humà...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: Tot anirà bé.

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: Com el lleial llop guardià que soc, sempre faig una ullada al perill, i faig el que puc per mantenir-te segur.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: Ho prometo.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Última app. Instagram. Què diràs?

`hong({eyes:"sad"});`

h: Són... més fotos de la festa.

`hong({mouth:"sad"});`

h: Tothom sembla estar content. Sense preocupacions. Sense ansietat.

`hong({mouth:"anger"});`

h: Déu meu, per què no puc ser com ells? Perquè no puc ser *normal*?

`bb({eyes:"normal_right"});`

b: Si parles de festes, voldria mencionar la invitació del cap de setmana. La meva decisió FINAL és:

`bb({eyes:"normal"});`

[Hauriem d'anar.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[No hauriem d'anar.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: Hauriem de--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: VES-TE'N.

`hong({body:"2_you"});`

h: A TORRAR *^COLLONS^*.

(...500)

b: q

(...1500)

`bb({eyes:"wat_2"});`

b: què?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: ANIRÈ a la festa.

{{if _.act1g=="go"}}
h: NO perquè vulguis, sinò perquè *JO* vull.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisament PERQUÈ tu no ho vols.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: NO tens cap mena de control sobre mi.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Ara disculpa'm mentre menjo aquest sabrós sandvitx en pau.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH ENS MORIREM](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH TOTHOM ENS ODIA](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH SOM GENT TERRIBLE](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH ENS MORIREM AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH TOTHOM ENS ODIA AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH SOM GENT TERRIBLE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: FELICITACIONS

(...500)

n: HEU ACONSEGUIT PROTEGIR LES NECESSITATS FÍSIQUES + SOCIALS + MORALS DEL TEU HUMÀ

n: NOMÉS FIXA'T COM D'AGRAÏT ESTÀ AMB TU!

(...500)

n: ARA QUE LA SEVA ENERGIA ÉS ZERO, POTS CONTROLAR LES SEVES ACCIONS.

`bb({mouth:"smile", eyes:"normal"});`

n: ESCULL EL TEU MOVIMENT FINAL

`bb({mouth:"small_lock", eyes:"fear"});`

n: *ACABA'LS*

[{LLUITA: Castiga el teu estressant telèfon!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGIDA: Cargola't com una pilota i plora!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: El teu telèfon t'estava donant un atac de pànic!

`bb({eyes:"anger"})`

b: Zuckerberg i els seus estan manipulant la teva salut mental pels inversors capitalistes!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Castiga el telèfon! Destrueix-lo! Mata'l!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA'L MATA--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: El món sencer està plè de perills!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Fes com els armadillos! Fes-te bola per autodefensar-te!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: FES-TE BOLA I PLORA FES-TE BOLA I PLORA FES-TE BOLA I PLORA FES-TE BOLA I PLORA FES-TE BOLA I PLORA FES-TE BOLA I PLO--

(#act1j)

# act1j

`SceneSetup.act1_outro()`