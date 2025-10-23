# act2

`SceneSetup.act2();`

{{if _.badnews && !_.factcheck}}
(#act2-preamble-news1)
{{/if}}

{{if _.badnews && _.factcheck}}
(#act2-preamble-news2)
{{/if}}

{{if _.catmilk}}
(#act2-preamble-cat)
{{/if}}

(#act2-preamble-tinder)


# act2-preamble-news1

```
publish("act2",["dee",3]);
```

s: Però has *vist* aquella història sobre el tràgic esdeveniment que està passant a algun lloc?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hola...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Carai, odio les noticies. Només és sensacionalisme i «Clicbait».

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: bo... bonica festa...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Veritat, però només segueixen incentius. El problema *real* són els que fan clic.

```
publish("act2",["dee",3]);
```

s: Qui faria repiolada d'una terrible història, i fer que tots els seus amics se sentin malament?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Agh, quin fàstic, veritat?

(#act2-preamble-end)


# act2-preamble-news2

```
publish("act2",["dee",3]);
```

s: Però has *vist* aquella notícia viral?

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hola...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",3]);
```

a: Ja, molt falsa. Qui podria caure a tal cosa i repiolar-ho?

```
publish("act2",["dum",2]);
publish("act2",["party_hong","next"]);
```

h2: q... quina festa més maca...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: T'ho juro paio. Sigui, ei, que pots obrir el Google i comprovar la informació?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Agh, quin fàstic, veritat?

(#act2-preamble-end)


# act2-preamble-cat

```
publish("act2",["dee",3]);
```

s: Com anava dient, el Complexe Industrial dels Mems explota als gats.

```
publish("act2",["dee",2]);
publish("act2",["party_hong","next"]);
```

h2: h-hola...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Elabora la teva tesi.

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: q... quina festa més maca...

```
publish("act2",["party_hong","next"]);
publish("act2",["party_hunter",0]);
publish("act2",["dee",1]);
```

s: Bé, ahir vaig veure algú repiolant un GIF d'un gat bevent llet.

```
publish("act2",["dee",3]);
```

s: No poden digerir aquella ^merda^! Qui repiolaria *abús animal* com si res?

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Agh, quin fàstic, veritat?

(#act2-preamble-end)


# act2-preamble-tinder

```
publish("act2",["dee",1]);
```

s: Així que sí, no em va tornar a contestar!

```
publish("act2",["dee",0]);
publish("act2",["party_hong","next"]);
```

h2: h-hola...

```
publish("act2",["party_hunter",1]);
publish("act2",["party_hong","next"]);
publish("act2",["dum",1]);
```

a: Encara que els dos vau fer match al Tinder?

```
publish("act2",["dum",0]);
publish("act2",["party_hong","next"]);
```

h2: q... quina festa més maca...

```
publish("act2",["party_hong","next"]);
```

{{if _.serialkiller}}
(#act2-preamble-serialkiller)
{{/if}}

{{if _.hookuphole}}
(#act2-preamble-hookuphole)
{{/if}}

{{if _.pokemon}}
(#act2-preamble-pokemon)
{{/if}}

# act2-preamble-serialkiller

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ni idea! Què, van pensar que era un *assassí en serie*? Quina paranoia.

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Agh, quin fàstic, veritat?

(#act2-preamble-end)


# act2-preamble-hookuphole

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ni idea! Potser pensen que tenir un match no pot emplenar el forat al seu cor?

s: No siguis tan purità! Primer obres el cap, després obres les cames!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Agh, quin fàstic, veritat?

(#act2-preamble-end)


# act2-preamble-pokemon

```
publish("act2",["party_hunter",0]);
publish("act2",["dee",3]);
```

s: Ni idea! No estava tan bona, però podria haver estat una bona pesca!

```
publish("act2",["party_hunter",1]);
publish("act2",["dee",2]);
publish("act2",["dum",3]);
```

a: Fes-les tots teves!™

(#act2-preamble-end)


# act2-preamble-end

```
Game.clearText();
publish("act2-out-1");
music(null, {fade:1});
```

(...3000)

```
music('battle', {volume:0.5});
publish("hp_show");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

n: RONDA DOS: *LLUITA!*

[Oh no ens odien!](#act2a_social)

[Estaves *mirant* al pel-roig?](#act2a_perv)

[Ei, parlem del significat de la vida.](#act2a_meaning)

# act2a_social

`bb({eyes:"sad"})`

b: Estem entristint aquesta festa per ser uns aixafaguitarres tristos!

`bb({eyes:"shock", body:"two_up"})`

b: Estem matant les bones sensacions! Estem cometint un assassinat de sensacions de primer grau!

`bb({eyes:"normal", body:"normal"})`

b: Humana, hem de sortir *ja* abans no--

```
_.a2_first_danger = 'social';
_.a2_attack_1 = "alone";
```

(#act2b)

# act2a_perv

`bb({eyes:"suspect"})`

b: Són més atractius que nosaltres, el que vol dir que si fem l'intent de *mirar-los* doncs--

`bb({eyes:"shock", body:"two_up"})`

b: SÓM UNS PERVERITS.

`bb({body:"normal"})`

b: Sóm uns pervertits temibles, malèfics, molt i molt do--

```
_.a2_first_danger = 'perv';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2a_meaning

`bb({body:"one_up", eyes:"normal_r"})`

b: Realment, què podem fer que importi de veritat?

`bb({body:"normal", eyes:"sad"})`

b: Contribuir a l'humanitat? Tots els bons treballs cauen com en Osimàndias. L'amor? La mort sempre el separa.

`bb({eyes:"sad_r"})`

b: Oi, i quanta mort! *Nosaltres* morirem. *Els nostres estimats* moriran.

`bb({eyes:"shock", body:"two_up"})`

b: Caram, la Segona Llei de la Termodinàmica diu que fins i tot el nostre *univers* morirà!

`bb({eyes:"suspect", body:"normal"})`

b: Que «la mort ens permet apreciar la vida»? És com dir que la esclavitud és bona perquè ens permet apreciar la llibertat!

`bb({body:"one_up"})`

b: Que «has de donar sentit al món? Això és el que fan els sectaris i els conspiranoics!

`bb({eyes:"shock", body:"two_up"})`

b: La vida no té cap significat, ni la mort, fins i tot *significat* no té significat! Què se supossa que ha de fer un ànima mort--

```
_.a2_first_danger = 'meaning';
_.a2_attack_1 = "bad";
```

(#act2b)

# act2b

`bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"suspect"})`

b: Ehm... em pots escoltar, humà?

`bb({eyes:"normal", MOUTH_LOCK:true})`

b: ...

`bb({eyes:"shock", mouth:"small_talk", body:"chest", MOUTH_LOCK:true})`

b: *ESPANT*

`bb({mouth:"small_talk"})`

b: HE D'ADVERTIR-VOS DE...

[*Més* perills similars!](#act2b_louder)

{{if _.a2_first_danger=="social"}}
[Un *altre* perill social!](#act2b_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[Un *altre* perill moral!](#act2b_different_moral)
{{/if}}

[Ignoreu el perill! Això és perillós!](#act2b_ignore)

# act2b_louder

`_.a2_first_choice = "louder"`

{{if _.a2_first_danger=="social"}}
(#act2b_louder_social)
{{/if}}

{{if _.a2_first_danger=="perv"}}
(#act2b_louder_perv)
{{/if}}

{{if _.a2_first_danger=="meaning"}}
(#act2b_louder_meaning)
{{/if}}

# act2b_louder_social

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: LES EMOCIONS SÓN CONTAGIOSES! SI NO SURTS INFECTARÀS A TOTHOM AMB ELS TEUS PROBLEMES MENTALS!

b: Crearàs un brot del SINDROME DE L'AIXAFAGUITARRES TRIST

`bb({eyes:"suspect", body:"normal", mouth:"normal"})`

b: Hem de sortir d'aquí i fer quarentena permanent a una habitació petitona amb Netflix i menjar a domicili!

```
_.a2_second_danger = 'netflix';
_.a2_attack_2 = "alone";
```


(#act2c)

# act2b_louder_perv

`bb({eyes:"suspect", body:"two_up", mouth:"normal"})`

b: NO SIGUIS PERVERTIT. ESTÀ CONTRA LA LLEI!

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: Llei de Pervertits, Secció 74.5: (1) Tota persona que comprovi (a) aquelles espatlles musculoses (b) aquell cul rodonet (2) serà reconegut com a

`bb({eyes:"shock", body:"two_up", mouth:"normal"})`

b: «UN PERVERTIT GRAN I FASTIGÓS»

```
_.a2_second_danger = 'law';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "la llei";
```

(#act2c)

# act2b_louder_meaning

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: Realment, fins i tot si trobes un propòsit digne a la vida, *encara pots* fúmer tot!

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Alfred Nobel cercava la pau mundial i l'interculturalitat. Això el va impolsar a simplificar el procès de viatjar.

`bb({eyes:"normal_r"})`

b: Necessitava trobar una forma per formar túnels de ferrocarrils. Doncs va crear un nou material anomenat «dinamita»...

`bb({body:"one_up", eyes:"normal"})`

b: que va ser utilitzada a la Primera Guerra Mundial per ASSASSINAR MILIONS DE PERSONES

`bb({body:"two_up", eyes:"shock"})`

b: AIXÒ ÉS L'EFECTE PAPALLONA, HUMÀ! QUANTES PERSONES ESTÀS MATANT ACCIDENTALMENT ARA MATEIX

```
_.a2_second_danger = 'butterfly';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "la Primera Guerra Mundial";
```

(#act2c)

# act2b_different_social

`_.a2_first_choice = "different"`

`bb({eyes:"normal_r", body:"point", mouth:"normal"})`

b: Ara que ho penso, saps què és pitjor que ningú t'estimi? Que *tothom* t'estimi.

`bb({body:"one_up", eyes:"suspect", mouth:"normal"})`

b: Un exemple seria convertir-te en un *d'aquests* fiesters busca-plaers.

`bb({body:"normal", mouth:"small"})`

b: Una vida buida amb amics buits que només coneixen la teva versió buida!

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Humà, hem de escapar d'aquests zombis del plaer abans de que ens converteixin!

```
_.a2_second_danger = 'zombies';
_.a2_attack_2 = "alone";
_.a2_hoodie_callback = "zombis";
```

(#act2c)

# act2b_different_moral

`_.a2_first_choice = "different"`

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: Gent està morint a crisis de fam i genocidis *ara mateix* i nosaltres estem en festes com si res!

`bb({body:"point", eyes:"closed", mouth:"small"})`

b: Una persona sàvia va dir una vegada, «l'únic necessari perquè triomfi el mal és que la gent bona no faci res».

`bb({body:"two_up", eyes:"shock", mouth:"normal"})`

b: NO ESTEM FENT RES

`bb({mouth:"small"})`

b: PER ANAR DE FESTA, AJUDEM A *HITLER*.

```
_.a2_second_danger = 'hitler';
_.a2_attack_2 = "bad";
_.a2_hoodie_callback = "en Hitler";
```

(#act2c)

# act2b_ignore

`_.a2_first_choice = "ignore"`

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Penses que estas segur perquè l'has tret les piles al detector de monòxid de carboni?

`bb({eyes:"suspect_r"})`

b: No sentiras pas el verí! T'adormiras i després---

`bb({body:"scream_c_1"})`

b: MORIRÀÀÀÀÀÀÀÀÀÀÀÀÀÀÀÀÀÀS

```
_.a2_second_danger = 'ignore';
_.a2_attack_2 = "harm";
_.a2_hoodie_callback = "el monòxid de carboni";
```

(#act2c)

# act2c

```
hong({body:"ignore_sweat"});
bb({eyes:"normal", mouth:"normal", body:"normal", MOUTH_LOCK:true});
```

b: ...

`bb({eyes:"happy", mouth:"smile", body:"chest"})`

b: Gràcies a tot el que és bo, humà, crec que pots sentir-me de nou!

`bb({eyes:"closed", body:"point"})`

b: T'HE D'ADVERTIR...

{{if _.a2_first_choice=="louder"}}
[*Encara més* del mateix perill!](#act2c_louder)
{{/if}}

{{if _.a2_first_choice!="louder"}}
[*Més* sobre el mateix parill!](#act2c_louder)
{{/if}}

{{if _.a2_first_danger=="social"}}
[D'un *altre* perill social!](#act2c_different_social)
{{/if}}

{{if _.a2_first_danger=="perv" || _.a2_first_danger=="meaning"}}
[D'un *altre* perill moral!](#act2c_different_moral)
{{/if}}

[Has revisat el ponx abans de beure?](#act2c_punch)

#act2c_louder

{{if _.a2_second_danger=="netflix"}}
(#act2c_louder_netflix)
{{/if}}

{{if _.a2_second_danger=="law"}}
(#act2c_louder_law)
{{/if}}

{{if _.a2_second_danger=="butterfly"}}
(#act2c_louder_butterfly)
{{/if}}

{{if _.a2_second_danger=="zombies"}}
(#act2c_louder_zombies)
{{/if}}

{{if _.a2_second_danger=="hitler"}}
(#act2c_louder_hitler)
{{/if}}

{{if _.a2_second_danger=="ignore"}}
(#act2c_louder_ignore)
{{/if}}

# act2c_louder_netflix

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: Oblida't del Netflix i del menjar a domicili, ni això és suficient! Infectaríem al servei!

`bb({body:"one_up", mouth:"small"})`

b: Ens hem de mudar a un territori a Yukon, Canadà, i rebre el menjar per drons!

`bb({body:"two_up", mouth:"normal"})`

b: I encara haurien d'estirilitzar el dron per treure els GERMES D'AIXAFAGUITARRES TRISTOS

`_.a2_attack_3 = "alone";`

`_.a2_hoodie_callback = "una quarentena";`

(#act2d)

# act2c_louder_law

`bb({eyes:"judge", body:"judge_1", mouth:"normal"})`

(...201)

```
bb({body:"judge_2"}, 0);
sfx("gravel");
```

(...168)

`bb({body:"judge_1"}, 0)`

(...168)

`bb({body:"judge_2"}, 0)`

(...168)

`bb({body:"judge_1"}, 0)`

(...501)

b: El GRAN PERVERTIT FASTIGÓS I PUDENT serà sentenciat a 72 hores a un d'aquells dispositius de humiliació pública medieval

b: a menys que secretament els hi *agradi* aquesta mena de coses

`bb({body:"scream_a_1"})`

b: perquè és un GRAN PERVERTIT FASTIGÓS I PUDENT

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "la llei";`

(#act2d)

# act2c_louder_butterfly

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: L'EFECTE PAPALLONA! Fas servir un vas de plàstic no biodegradable?

`bb({body:"two_up", mouth:"normal", eyes:"shock"})`

b: PUM, UN ABOCADOR FILTRA VERÍ I MATA UN NEN

`bb({body:"normal", mouth:"small", eyes:"suspect"})`

b: Sues i el cor batega anormalment?

`bb({body:"scream_a_1"})`

b: PUM, FAS QUE EL NOSTRE SISTEMA D'ASSISTÈNCIA MÈDICA CAIGUI I MILIONS MOREN

`_.a2_attack_3 = "bad";`

`_.a2_hoodie_callback = "l'efecte papallona";`

(#act2d)

# act2c_louder_zombies

`bb({body:"normal", mouth:"small", eyes:"angry"})`

b: Aquests zombis del plaer es balancejaran cap a tu susurrant.

`bb({body:"normal", mouth:"normal", eyes:"shock"})`

b: «LIIIIIKES». «LIIIIIIIIIIKES».

`bb({body:"scream_a_1"})`

b: I doncs et MOSSEGARAN i et convertiràs en un TIO SENSE PERSONALITAT i/o una GUARRA SENSE CAP!

`_.a2_attack_3 = "bad";`

_.a2_hoodie_callback = "zombis";

(#act2d)

# act2c_louder_hitler

`bb({body:"scream_a_1"})`

b: ELS NAZIS FAN EL PAS DE L'OCA ALS CARRERS ARA MATEIX

`bb({body:"one_up", mouth:"smile", eyes:"happy"})`

b: Dient, *què bé que la "gent bona" hagi passat l'estona amb coses com la "relaxació" i el "benestar"!*

`bb({body:"point", mouth:"smile", eyes:"happy_r"})`

b: *Ara podem continuar, el reich està al dia!*

`_.a2_attack_3 = "bad";`

_.a2_hoodie_callback = "en Hitler";

(#act2d)

# act2c_louder_ignore

`bb({body:"normal", mouth:"normal", eyes:"normal_r"})`

b: Ara que ho penso, tenim constància de si aquest edifici *té* un detector de monòxid de carboni?!

`bb({body:"two_up", mouth:"small", eyes:"normal"})`

b: I si estem sent enverinats *ARA MATEIX*?

`bb({body:"scream_a_1"})`

b: NO PREDIRÍEM LA NOSTRA MORT. SENZILLAMENT PARARÍEM D'EXISTIR PER SEMPRE MÉS I MÉ--

`_.a2_attack_3 = "harm";`

_.a2_hoodie_callback = "el monòxid de carboni";

(#act2d)

# act2c_different_social

`bb({body:"normal", mouth:"normal", eyes:"sad"})`

b: I si sóm *fonamentalment incapaços* de ser estimats o d'estimar a un altre?

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: I si alguna cosa es va trencar dins nostre temps enrere? O si mai ha existit en primer lloc?

`bb({body:"scream_a_1"})`

b: AHH ESTEM TRENCATS! TRENCADETS TRENCADETS TRENCADE--

`_.a2_attack_3 = "alone";`

(#act2d)

# act2c_different_moral

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: I si estem *fonamentalment podrits*?

`bb({body:"one_up", eyes:"sad"})`

b: Altres estan guiats a fer bones obres, pero si les fem, nomès són per culpabilitat o vergonya.

`bb({body:"normal", mouth:"small", eyes:"sad_r"})`

b: I si és la nostra naturalessa fer mal als altres? I si no podem ser res *però* una molèstia a la gent prop nostre?

`bb({body:"scream_a_1"})`

b: AHH ESTEM TRENCATS! TRENCADETS TRENCADETS TRENCADE--

`_.a2_attack_3 = "bad";`

(#act2d)

# act2c_punch

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: No soc irracional. La gent *posa drogues* als ponxos. Això és una cosa que passa de veritat.

`bb({eyes:"suspect"})`

b: Humà, et fa mal el cap? Tens els músculs relaxats? Crec que estem morint.

`bb({body:"scream_a_1"})`

b: AHHH ENS MORIM! ENS MORIM ENS MORIM ENS MORI--

`_.a2_attack_3 = "harm";`

_.a2_hoodie_callback = "ponxos";

(#act2d)

# act2d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"attacked"});
attack("20p", _.a2_attack_1);
```

(...401)

```
hong({body:"attacked_2"});
attack("20p", _.a2_attack_2);
```

(...401)

```
hong({body:"attacked_3"});
attack("20p", _.a2_attack_3);
```

(...1001)

h: M^ERDAAAA^!

h: M^ERDA^ M^ERDA^ M^ERDÍSSIMA^ *M^ERDA^ *

`bb({body:"two_up", mouth:"smile", eyes:"happy"});`

b: Iupi, humà! Què bé que em puguis sentir!

`bb({body:"normal", mouth:"small", eyes:"sad"})`

b: Perquè m'ignoraves?

`hong({body:"facepalm"})`

h: Santíssima ^hòstia^, ets idiota.

`hong({body:"facepalm_2"})`

h: Et saps aquella història dels nadius americans?

h: «Hi ha dos llops dins teu, un és la fe, l'altre és la desesperança. Quin guanya? El que donis de menjar».

```
hong({body:"facepalm_3"});
bb({eyes:"normal"});
```

h: Volia que *passessis fam*, ^imbècil^ sadista!

`hong({body:"smile", mouth:"smile"})`

h: Oblida-ho, provarè amb afirmacions positives.

h: *M'estimen. Soc bona persona. Soc intel·ligent. Tinc cert atractiu. Soc especial.*

`bb({eyes:"suspect"});`

[Mare meva, què narcissista!](#act2d_narcissist)

[Saps que el tema de les afirmacions ha sigut *desmentit*?](#act2d_disproven)

[oh 10 meu no donis crèdit a la gent indígena per històries així](#act2d_racist)

# act2d_disproven

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: De fet, poden *fer més mal* a la gent amb mala autoestima!

`bb({body:"one_up", mouth:"small", eyes:"normal"})`

b: Era un estudi molt ben dissenyat – un experiment al atzar i controlat, l'experimentador no sabia qui era a qual grup.

`bb({body:"two_up", mouth:"small", eyes:"normal_r"})`

b: Els resultats van demostrar que si ja tenies una baixa autoestima, repetir-te afirmacions positives et feien sentir *pitjor* que no pas callar-te!

`bb({body:"point", mouth:"normal", eyes:"closed"})`

b: Wood 2009, Ciències Psicològiques. Cerca-ho al Google Acadèmic, humà,

`bb({body:"scream_b_1"})`

b: I DESPRÉS PARA DE DESINFORMAR AMB NOTÍCIES FALSES

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_narcissist

`bb({body:"normal", mouth:"normal", eyes:"normal"})`

b: Has de veure els teus errors amb humiltat per crèixer com a persona!

`bb({body:"two_up", eyes:"suspect"})`

b: No pots posar ambientador a una habitació mugrossa! Cobrir els teus errors et fa pitjor a la llarga.

`bb({body:"chest", mouth:"smile", eyes:"closed"})`

b: Agraïdament, jo, com el teu llop guardià, et puc alertar dels teus errors. I ara mateix-

`bb({body:"scream_b_1"})`

b: TOT. TOT ESTÀ MALAMENT

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2d_racist

`bb({body:"normal", mouth:"normal", eyes:"suspect"})`

b: Els nadius americans són *persones de veritat*, no uns «salvatges nobles» que puguis nombrar per fer que els teus consells de bescuit xinès siguin més *exòtics*.

`bb({eyes:"suspect_r"})`

b: Estàs reduïnt a individuus i cultures complexes a frases ximples. Això és «racisme benevolent»!

`bb({body:"scream_b_1"})`

b: PARA DE SER RACISTA IDIOTA D'ULLS AMETLLATS

```
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2e)

# act2e

h: ^EM CAGO EN TOT^.

`hong({body:"yell", mouth:"yell"})`

h: Saps què? Ets *irracional*.

h: Tothom sap que les emocions són irracionals! Especialment el pànic!

`hong({body:"facepalm_2"})`

h: Ets una deixalla inútil de l'evolució, com el meu apèndix o els queixals del seny!

`hong({body:"yell", mouth:"yell"})`

h: ^Coi^, aquesta metàfora del llop és estúpida! Només ets un munt de neuroquímics al meu cap!

`hong({body:"cross", mouth:"cross"})`

h: Per què hauria d'escoltar a un tros de ^merda^ inútil i irracional que no existeix com tu?!

`bb({eyes:"sad", MOUTH_LOCK:true})`

b: ...

[Dimonis, humà. Realment fa molt de mal.](#act2e_hurtful)

[Soc un sentiment. Els sentiments són vàlids.](#act2e_valid)

[Humà, els *dos* sóm «només químics».](#act2e_rational)

# act2e_hurtful

`bb({body:"chest"})`

b: Soc *part* teva. Quan dius això, et fas mal a *tu mateix*.

`bb({body:"scream_a_1"})`

b: Per què et dones cops, humà? PARA DE DONAR-TE COPS.

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2e_rational

`bb({body:"normal", mouth:"normal", eyes:"normal_r"});`

b: Les teves motivacions són dopamina, els teus plaers són serotonina.

`bb({body:"one_up"});`

b: Les teves memòries són pesos sinàptics, el teu seny són senyals elèctriques que poden fallar.

`bb({eyes:"normal", body:"normal"});`

b: Així que si sent «només uns químics» *soc* irracional... doncs tu *també* ets irracional!

`bb({body:"two_up", eyes:"shock"});`

b: I si els *dos* sóm irracionals, doncs *mai* sabrem com arribar a la plenitud i la feliçitat!

`bb({body:"scream_a_1"})`

b: AHH ESTEM TRENCATS! TRENCADETS TRENCADETS TRENCADE--

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "bad");
```

(...2500)

(#act2f)

# act2e_valid

`bb({body:"normal", mouth:"normal", eyes:"suspect"});`

b: Espera... «ells» diuen que els sentiments són vàlids, i que sempre hauries d'acceptar les teves emocions.

`bb({eyes:"suspect_r"});`

b: Però «ells» també diuen que les emocions són irracionals, que no es pot confiar de les emocions.

`bb({eyes:"angry"});`

b: Per tots els céls, «ells» ens han mentit sempre!

`bb({body:"scream_a_1"})`

b: «ELLS» ENS DIUEN CONTRADICCIONS PER FER-NOS DEPENENTS DEL COMPLEXE INDUSTRIAL D'AUTOAJUDA

```
music(null);
hong({body:"attacked"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
attack("10p", "harm");
```

(...2500)

(#act2f)

# act2f

`hong({body:"defeated", MOUTH_LOCK:true});`

h: ...

h: Odio això. Tant de mal em fa que ho *odio*.

h: No et puc calmar. No et puc ignorar. No puc lluitar.

`bb({eyes:"suspect"});`

h: Sense importar el que faci, no em puc llibrar de tu.

`bb({body:"cry_1"});`

b: Potser NO HAURIES DE DESFER-TE DE MI.

`bb({body:"cry_2"});`

b: Com creus que em sento *jo*, humà?!

`bb({body:"cry_4", mouth:"cry", eyes:"cry"})`

b: Faig quant puig per ser el teu gos guardià, però no pares de veure'm com un Llop Malvat!

b: I doncs *m'esforço més* en apartar-te del perill! *De més* perills! *D'altres* perills!

`bb({eyes:"cry_2"})`

b: Però sense importar quant m'esforci en protegir-te, *encara* creus que soc el teu enemic!

`bb({body:"cry_5"});`

b: Què fai malament?!

`bb({body:"cry_2"});`

b: *Sé* que apesto al meu treball. Però *faig l'intent*, humà!

`bb({body:"cry_3"});`

b: ...el faig.

`bb({body:"cry_6", mouth:"right", eyes:"cry_r_1"});`

b: No has de fer cas als meus avisos, o concordar amb mi, o tan sols *estimar-me*.

`bb({eyes:"cry_r_2"});`

b: Només... vull que em tinguis paciència.

`bb({eyes:"cry_r_3"});`

b: Només vull que t'asseguis amb mi en comptes de girar cua i--

```
bb({eyes:"cry_r_4"});
hong({body:"listen"});
```

r: Ei.

```
hong({body:"look"});
Game.clearText();
publish("act2-in-2");
publish("hp_hide");
music('party1', {volume:0.4, fade:2});
```

(...2000)

```
publish("act2",["party_hunter",2]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Sembla que estàs tenint una lluita interna, nano.

```
publish("act2",["party_hunter",3]);
publish("act2",["party_hong",13]);
```

h2: N'era tan obvi?

```
publish("act2",["party_hunter",4]);
publish("act2",["party_hong",14]);
```

r: Estaves, ah, remugant a la teva suadora sobre {{_.a2_hoodie_callback}} o alguna cosa per l'estil.

```
publish("act2",["party_hunter",13]);
publish("act2",["party_hong",15]);
sfx("rustle", {volume:0.6});
setTimeout(function(){
 publish("act2",["party_hong",16]);
 sfx("concrete_step3", {volume:0.6});
},401);
setTimeout(function(){
 publish("act2",["party_hong",17]);
 sfx("concrete_step4", {volume:0.6});
},801);
```

h2: mare meva no m'entenc.

```
publish("act2",["party_hunter",7]);
publish("act2",["party_hong",18]);
sfx("squeak");
```

r: Ei. No estàs sol, nano. L'ansietat és súper normal.

```
publish("act2",["party_hunter",5]);
publish("act2",["party_hong",19]);
```

{{if _.act1_ending=="fight"}}
r: Coi, ahir mateix vaig sentir a algú al campus tenir un atac nerviós i trencar el seu móbil!
{{/if}}

{{if _.act1_ending=="flight"}}
r: Coi, ahir mateix vaig sentir a algú plorant i cargolant-se en públic!
{{/if}}

```
publish("act2",["party_hunter",2]);
```

r: Escolta, sé com se sent tenir a aquest animal al teu cap.

```
publish("act2",["party_hunter",8]);
```

r: *Tothom* ho sap. Això és el que m'impulsa a fer festes cada cap de setmana, per oblidar els nostres problemes, i a aquell animal.

```
publish("act2",["party_hunter",9]);
publish("act2",["party_hong",20]);
```

h2: però la meva ansietat...

```
publish("act2",["party_hunter",2]);
publish("act2",["party_hong",21]);
```

r: No t'angoixis, nano. Abans era com tu. Però doncs vaig trobar un petit truquet per fer que la veueta aquella es calli...

```
publish("act2",["party_hunter",3]);
Game.clearText();
music(null, {fade:1});
```

(...2001)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",22]);
sfx("rustle");
```

(...2501)

```
publish("act2",["party_hunter",10]);
publish("act2",["party_hong",23]);
sfx("rustle2");
```

(...1001)

```
publish("act2",["party_hunter",11]);
```

r: La meva pròpia mescla especial. És una mica més forta què... doncs, realment qualsevol cosa legal.

```
publish("act2",["party_hunter",12]);
publish("act2",["party_hong",24]);
```

r: Bottoms up, ^bee-yatch^!

```
hong({body:"hold"});
bb({body:"normal", mouth:"small", eyes:"wat"});
Game.clearText();
Game.WORDS_HEIGHT_BOTTOM = -1;
publish("act2-out-3");
publish("hp_show");
```

(...3500)

[Mare meva.](#act2g_1) `Game.OVERRIDE_CHOICE_LINE=true`

[No hauries de fer front a res així.](#act2g_2) `Game.OVERRIDE_CHOICE_LINE=true`

[No prenguis begudes de desconeguts.](#act2g_3) `Game.OVERRIDE_CHOICE_LINE=true`

# act2g_1

b: M--

(#act2g)

# act2g_2

b: N--

(#act2g)

# act2g_3

b: N--

(#act2g)

# act2g

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"forward", mouth:"forward"});
bb({body:"frazzled", mouth:"frazzled", eyes:"frazzled"});
```

h: Mmm, quin gin tónic tan exquisit!

h: Un cos amb un taste de «ignora-ho tot» amb un lleu regust a «mai més senteix res»!

b: Això és dolent, humà. Això és molt, molt dolent.

[*Així* és com començen les adiccions.](#act2h_opt1) `Game.OVERRIDE_CHOICE_LINE=true`

[*Sabia* que el hoste tenia un problema!](#act2h_opt3) `Game.OVERRIDE_CHOICE_LINE=true`

[A més, podrien haver drogar-lo!](#act2h_opt2) `Game.OVERRIDE_CHOICE_LINE=true`


# act2h_opt1

b: *Així* és com--

(#act2h)

# act2h_opt2

b: A més, podrie--

(#act2h)

# act2h_opt3

b: *Sabia* que--

(#act2h)

# act2h

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("40p", "harm");
```

(...2000)

```
hong({body:"back", mouth:"back"});
bb({body:"panicked", mouth:"panicked", eyes:"panicked"});
```

h: Sabrós, *i a sobre* més barat que la teràpia!

b: HUMÀ PARA JA

h: Hehehe!

h: I què faràs *tu*, ^imbècil^?

b: Ho sento molt, humà.

b: Farè servir el meu ATAC ESPECIAL

```
bb({body:"special_a"});
music('battle', {volume:0.5});
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act2h_attack) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act2h_attack) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act2h_attack) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`

# act2h_attack

```
bb({body:"special_b_1"});
hong({body:"forward", mouth:"forward"});
sfx("charging");
```

h: Què és aquesta ^merda^?

h: Em donaràs més la xapa o--

```
bb({body:"special_c"});
sfx("hadouken");
```

(...901)

(#act2i)

# act2i

```
publish("hide_tabs");
publish("show_special_attack");
Game.FORCE_CANT_SKIP = true;
music(null);
stopAllSounds();
```

(...5000)

```
publish("show_tabs");
hong({ body:"final", mouth:"final" });
bb({ body:"normal", mouth:"normal", eyes:"sad" });
attack("100p", _.SPECIAL_ATTACK);
Game.FORCE_CANT_SKIP = false;
setTimeout(function(){
TABTABTABTAB publish("remove_special_attack");
},30);
```

(...2500)

h: QUÈ ^COLLONS^

b: Perdona'm. Necessitava ensenyar-te les conseqüències.

{{if _.SPECIAL_ATTACK=="harm"}}
h: PODIA *VEURE* EL MEU CADÀVER. PODIA *SENTIR* LA SENSACIÓ DE REALMENT ESTAR MORT.
{{/if}}

{{if _.SPECIAL_ATTACK=="alone"}}
h: PODIA *VEURE* LA CARA DE DISGUST DE TOTHOM. PODIA *SENTIR* TOT EL QUE DEIEN.
{{/if}}

{{if _.SPECIAL_ATTACK=="bad"}}
h: PODIA *SENTIR* ELS OSSOS CRUIXINT. PODIA *TASTAR* LA SANG A L'AIRE.
{{/if}}

b: Ho sento, humà.

n: *ACABAL'LS*

[{LLUITA: Dona un cop al hoste.}](#act2j_fight) `Game.OVERRIDE_CHOICE_LINE=true`

[{FUGIDA: Anem-nos d'aquí.}](#act2j_flight) `Game.OVERRIDE_CHOICE_LINE=true`

# act2j_fight

`bb({ eyes:"angry" });`

b: Aquell psicópata volia aprofitar-se de tu.

b: Et volien corrompre, torbar-te com estan ells de torbats!

`bb({ body:"yell_angry_1" });`

b: Dona-li un cop! Una mà de llenya per a ells!

`bb({ body:"final_1" });`

b: DONA'LS UN COP DONA'LS UN COP DONA'LS UN COP DONA'LS UN COP DONA'LS UN COP DONA'LS UN COP DONA'LS UN COP DONA'LS UN CO--

`_.a2_ending = "fight";`

(#act2k)

# act2j_flight

b: *Sabia* que aquests () estaven molt torbats. Calmen els seus mals amb coses terribles!

`bb({ body:"yell_1" });`

b: I t'enganyen perquè facis el mateix! T'estan corrompint! Hem de sortir!

`bb({ body:"final_1" });`

b: SURT SURT SURT SURT SURT SURT SURT SURT SURT SUR--

`_.a2_ending = "flight";`

(#act2k)

# act2k

```
Game.clearText();
publish("act2-in-4");
publish("hp_hide");
music('party1', {volume:0.6, fade:1.5});
```

(...2001)

```
publish("act2",["party_hong",26]);
sfx("slide");
```

(...1001)

```
publish("act2",["party_hunter",14]);
Game.WORDS_HEIGHT_BOTTOM = 230;
```

r: Estàs bé, nano?

`publish("act2",["party_hunter",13]);`

{{if _.a2_ending=="fight"}}
(#act2k_fight)
{{/if}}

{{if _.a2_ending=="flight"}}
(#act2k_flight)
{{/if}}

# act2k_fight

```
Game.clearText();
publish("act2",["party_hunter",21]);
publish("act2",["party_hong",33]);
music(null);
sfx("hit");
```

(...1000)

```
sfx("record_scratch");
publish("act2",["party_hunter",22]);
publish("act2",["party_hong",34]);
publish("act2",["dee",6]);
publish("act2",["dum",6]);
```

r: T-tu...

```
publish("act2",["party_hunter",23]);
publish("act2",["party_hong",35]);
publish("act2",["dee",5]);
publish("act2",["dum",5]);
music('party1', {volume:0.6, fade:6});
```

r: ets un *masoca*.

r: M'agrada això. Veniu a la festa el cap de setmana que vé, monada.

```
publish("act2",["party_hunter",19]);
publish("act2",["party_hong",36]);
```

h2: d'acord adéu, ciao, adiós, au revoir

r: Potser l'animalet ha guanyat avui, però si tornes, et farè un breuatge fins i tot més intens!

h2: sayōnara, auf wiedersehen, zài jiàn, shalom

r: Tu i jo, nano, ensenyem a la bèstia qui mana!

(#act2k_end)

# act2k_flight

`publish("act2",["party_hong",36]);`

h: d'acord perdó m'he d'anar

`publish("act2",["party_hunter",16]);`

r: ^Collons^. L'animal ha guanyat avui, eh?

`publish("act2",["party_hunter",15]);`

h2: no no, només, eh, em vaig a fer la marató de tv3. he de córrer.

`publish("act2",["party_hunter",19]);`

r: Veniu a la meva festa el cap de setmana que vé. Et farè alguna cosa més intensa per tu.

h2: d'acord gràcies he de córrer córrer córrer córrer córrer

r: Tu i jo, nano, ensenyem a la bèstia qui mana!

(#act2k_end)

# act2k_end

```
Game.clearText();
publish("act2-out-5");
publish("act2-outro", ["end1"]);
music("hum", {fade:2, volume:0.6});
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2500)

```
publish("act2", ["act2_end",2]);
sfx("whoosh");
```

(...1000)

b: Humà! Estàs bé?!

```
publish("act2", ["act2_end","next"]);
```

b: Ai, per tan *poquet*. Realment podriem haver--

```
Game.clearText();
publish("act2", ["act2_end","next"]);
music(null);
sfx("squeak");
```

(...1500)

```
publish("act2", ["act2_end","next"]);
sfx("hit");
```

(...1000)

h: Vindrè a la festa de la setmana que vé.

h: El següent cop que hagi de lluitar, no només et *derrotarè*...

h: Sinò que a més et matarè a la ^merda^.

```
Game.clearText();
publish("act2", ["act2_end","next"]);
sfx("concrete_step1");
````

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step2", {volume:0.8});
```

(...901)

```
publish("act2", ["act2_end","next"]);
sfx("concrete_step3", {volume:0.5});
```

(...901)

`sfx("concrete_step4", {volume:0.25});`

(...3000)

`_.INTERMISSION_STAGE = 2;`

(#intermission)