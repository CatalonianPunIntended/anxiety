# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (la partida s'ha desat)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *sospira*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Doncs, què ^carai^ és la moral d'aquesta història?

`hong({body:"one_up", eyes:"annoyed"})`

h: Què hem *après*? *Vaig* fer coses estúpides, els meus «amics» *em van* manipular, i quasi *morim*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[Seh, per no parlar de la factura de l'hospital.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[Seh, per no parlar del fetge.](#act4a_liver)
{{/if}}

[Seh, allò era *la* pitjor de les possibilitats.](#act4a_worst)

[Seh, tenia la raó.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: I tant. No crec que el meu segur cobreixi «fer el burro».

`hong({eyes:"annoyed", mouth:"normal"});`

b: Així i tot... hem sobreviscut!

`hong({eyes:"normal"});`

h: ?

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: Ens hem tret uns anys de la nostra esperança de vida...

`bb({eyes:"surprise"});`

b: Però encara *tenim* esperança de vida! Hem sobreviscut!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ?

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: Així i tot...

h: Hm?

`bb({eyes:"surprise"});`

b: Hem sobreviscut!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: Però... tu també tenies raó.

`hong({eyes:"surprise"});`

h: Hm?

`bb({eyes:"normal"});`

b: Jo *era* el llop que cridava pel llop. Doncs, quan el perill *de veritat* va venir, amb justa raó, no em vas creure.

`bb({eyes:"surprise_r"});`

b: Encara i amb això, hem sobreviscut!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: Després de tot pel que hem passat, encara estem aquí.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h: Estàs molt calmat considerant que hem tingut una experiència propera a la mort.
{{/if}}

{{if !_.INJURED}}
h: Estàs molt calmat considerant que hem tingut una *experiència propera* a una experiència propera a la mort.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: Well, it makes everything else less scary in comparison. It's also got me thinking.

`bb({eyes:"normal", mouth:"normal"});`

b: Si barallar-me amb tu està malament perquè no et protegeixo de res...

h: Però barallar-me amb tu *també* està malament perquè només fa que et posis a cridar més...

`bb({eyes:"normal_r"})`

b: Potser...

`bb({eyes:"normal"})`

h: Potser no hem de lluitar.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: No soc un Llop Malvat. Però no soc un llop guardià, tampoc.

`bb({eyes:"sad_d"})`

b: Soc un gos agitat d'un refugi.

`bb({eyes:"sad"})`

b: Hem passat per coses grosses. Potser trauma o negligència. I això ha fet que jo em possi a fer:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: BUB BUB BUB BUB BUB

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: Però no *vull* ser un gos covard! Et vull protegir! Vull ser un bon gos!

`bb({eyes:"sad", mouth:"normal"});`

b: Humà... podries domesticar aquest llop?

`hong({eyes:"sad"})`

h: Jo.... ho provaré.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: Vinga. Relacions sanes amb les emocions. Les relacions necessiten comunicació. Doncs, comuniquem-nos.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: Els cinc minuts que venen potser semblaran molt cursis, però fem com si res.

```
hong({body:"hands_2", mouth:"normal"});
```

h: Estimat llop intern... com et sents *tu*?

n2: PORS USADES EN TOTAL:

*DANY FÍSIC* *MARGINACIÓ* *MALA PERSONA*

n2: QUINA POR VOLS DISCUTIR PRIMER? (POTS PROVAR LES ALTRES DESPRÉS)

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[Tinc por que ens puguin fer mal.](#act4_harm)

[Tinc por que ens deixin sols.](#act4_alone)

[Tinc por que ens vegin com mala gent.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: Vull protegir la teva necessitat a la integritat física,

`bb({eyes:"sad_d"})`

b: Però *tot el que ens envolta* sembla tan perillós. Tan ple de tragèdia i mal.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: No sé, *he* escollit què dir molta estona. Què vols dir *tu*, humà?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Un altre cop, és el teu torn, humà. Què penses?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vols afegir alguna cosa, humà?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tens raó. Protegim-nos, doncs.](#act4_harm_skills)

[Fiquem-nos en *més* perill, doncs.](#act4_harm_exposure)

[Gràcies.](#act4_thanks) `_.thanks_for = "per la meva integritat física";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: Ara... com? Tinc urpes i ullals, però només soc una metàfora.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: Podríem aprendre defensa personal? Unir-nos a una comunitat que es protegeixen l'un a l'altre? Millorar la nostra salut general i límits personals?

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: Potser, però...

[Com comencem?](#act4_harm_skills_start)

[I si res funciona?](#act4_harm_skills_work)

[I si ens passem amb la «seguretat»?](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: Tantes coses que podem fer, tantes coses que hem d'arreglar de nosaltres mateixos. Com hem de *començar*?

`hong({ body:"shrug", eyes:"surprise" })`

h: Ara mateix estem començant.

`bb({ eyes:"normal", mouth:"narrow" })`

b: Ep?

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: Ara mateix estem practicant la comunicació. Ens permetrà detectar millor el perill, amb menys falsos positius,

`hong({ eyes:"surprise" });`

h: I *això* ens protegirà del perill!

`hong({ eyes:"normal", mouth:"normal" });`

h: I, per tant: això *és* defensa personal.

`bb({ eyes:"normal_r" })`

b: Ah. Esperava més d'això:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: Tens raó, no podem protegir-nos al 100%...

`hong({ body:"one_up" });`

h: Però fins i tot una millora de l'1% té encara té valor, no creus?

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: No veus el got 99% buit, però 1% ple?

`bb({ eyes:"normal" });`

h: I que encara té un valor si et trobes varat al desert.

`bb({ eyes:"closed" });`

b: D'acord. De baix a dalt, doncs.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: Vull dir, la raó per què no em feies cas era perquè *jo* em vaig passar amb la seguretat!

`bb({ body:"normal", eyes:"normal" })`

h: Nah, tens raó. Volem estar segurs amb moderació. Tot sempre amb moderació.

`bb({ eyes:"suspect" })`

b: Espera, *TOT* amb moderació?

`hong({ eyes:"annoyed" })`

h: *Un nombre moderat de coses* amb moderació.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: Moltes gràcies per fer els teus arguments recursivament consistents.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *QUÈ*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: Vull dir, diguem que hi ha un gos espantat pels llamps.

`hong({ body:"hands_1" });`

h: Un truquet que fan els entrenadors és posar sorolls de llamps a un volum baix, i donen al gos una llaminadura si romanen tranquils.

`hong({ body:"hands_2" });`

h: Amb el temps, l'entrenador apuja el volum a poquet a poquet fins que el gos superi la seva por.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: Es diu teràpia d'exposició!

`hong({ body:"point", eyes:"normal" });`

h: Com ets un gos, podria funcionar igual, no? Tots els mamífers tenen la mateixa resposta de lluitar o fugir.

`hong({ body:"normal" });`

[I si ens insensibilitzem *en excés*?](#act4_harm_exposure_overboard)

[I si ens exposem a perills *de veritat*?](#act4_harm_exposure_hurt)

[Soc un llop, no un gos.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: I t'ensenyaré a ser amable i pacient fins que et domestiqui com a un gosset maco i petitó.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: Ai.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: *Acabem* de veure el que passa quan ignores el perill – et poses en situacions *realment* perilloses

`bb({ eyes:"angry_r", body:"one_up" })`

b: A més, amb *tanta* insensibilització no ens tornaríem en psicòpates?

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: En no res menjarem crispetes mentre veiem pornografia snuff!

`hong({ eyes:"annoyed" })`

h: Crec... que hi ha una distinció entre allò i els llamps.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: Però *on*, humà? *On hi és?!*

`hong({ eyes:"surprise", body:"one_up" })`

h: No ho sé. Però *tu* em pots ajudar!

`hong({ eyes:"normal", body:"normal" })`

H: Treballar i negociar amb tu, marquem la diferència.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: D'acord. Però no tinc polzes, així que l'hauràs de traçar tu.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: Un exemple: hem saltat d'una maleïda *teulada!*
{{/if}}

{{if !_.INJURED}}
b: Un exemple: quasi saltem d'una maleïda *teulada!*
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: Nah, tens raó. Un *pot* passar-se del límit.

`hong({ eyes:"normal" });`

h: Per això, si fem teràpia d'exposició, començarem amb calma, i anirem avançant al nostre ritme.

h: Abans de trobar-nos amb perill *real*, parem.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: Jo faig la distinció entre sentir llamps i presentar-nos en mig una tempesta amb un barret d'alumini.

(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: Espera, cap discussió a favor en contra del qual penso? Només... «gràcies»?

`hong({ eyes:"surprise", body:"shrug" })`

h: Sí! Aprecio que et preocupis {{_.thanks_for}}.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: Estàs bé?

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: Mai m'has donat *les gràcies* a mi abans.

`hong({ mouth:"smile" });`

h: Aii el meu llop del pànic gran i pelut.

(#act4_something_else)

# act4_thanks_2

h: Fins i tot si en faig un gra massa, aprecio que et preocupis {{_.thanks_for}}.

`bb({ eyes:"annoyed" })`

b: Para el carro... no estaràs repetint «gràcies» només per no parlar del perill, oi?

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: Però les coses són complexes, i no sempre tenim pensades les nostres respostes.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: No és com si la vida et donés una llista amb tres respostes possibles de diàleg.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: Però per ara, almenys et puc donar les gràcies.

b: I, gràcies a tu també, per escoltar-me pacientment.

`bb({ eyes:"closed" });`

b: Petit mamífer sense pèls.

(#act4_something_else)

# act4_thanks_3

h: Fins i tot si els teus lladrucs m'espanten, només estàs inquietat {{_.thanks_for}}.

`bb({ eyes:"smile_r" });`

b: Ep, si no pares d'afavorir-me així, l'internet tindrà idees estranyes nostres.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: Vinga, soc un nano vulnerable fent batxi i tu ets un llop que fa por. Què és el pitjor que po--

`hong({ eyes:"normal", body:"point" });`

h: Pensant-ho millor, no responguis.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: Vull ajudar-te a cobrir aquella intensa i humana necessitat de pertànyer...

`bb({ eyes:"sad_u" });`

b: Però em preocupa que si algú mai ens conegueren – de *veritat* – s'allunyarien.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: No sé, *he* escollit què dir molta estona. Què vols dir *tu*, humà?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Un altre cop, és el teu torn, humà. Què penses?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vols afegir alguna cosa, humà?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Tens raó: treballem la nostra vida social.](#act4_alone_skills)

[Crec que li agradem a la gent. I si provem de veure?](#act4_alone_experiment)

[Gràcies.](#act4_thanks) `_.thanks_for = "pel meu benestar social";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: Podem practicar capacitats socials com ara fer preguntes, escoltar i empatitzar, obrir-se i ser vulnerables, etc.?

`hong({ eyes:"normal_l" });`

h: O tenir millors hàbits socials, com organitzar estones amb amics o anar a quedades?

`hong({ body:"one_up" });`

h: També podríem aprendre a acceptar el rebuig.

`hong({ eyes:"normal" });`

h: O aprendre que la gent *no* ens rebutgen, sinó que estan cansats o tenen una Cara de Dona Odiosa.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: Són moltes opcions. Però sobre «aprendre capacitats socials»...

[Estariem *manipulant?*](#act4_alone_skills_manipulative)

[No ens faria *més manipulables?*](#act4_alone_skills_manipulated)

[I si tot això falla?](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: Però no són els assassins en sèrie que llegeixen les emocions de les seves víctimes «empàtics»?

`bb({ eyes:"annoyed" });`

b: Però no va Charles Manson guanyar-se amistats i influenciar a gent?

`hong({ eyes:"annoyed", body:"chin" });`

h: No, tens raó.

h: Les «capacitats socials» no són res si no ens importa *realment* la gent.

`hong({ body:"normal" });`

h: Bàsicament, no siguem uns ^cabrons^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: Ja tens un pòster motivacional per a tu.

`hong({ body:"shrug", mouth:"narrow" });`

h: «No Siguis ^Cabró^™»

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: Esdevindrem en un fregapeus que digui «Benvolguts», dient «Gràcies» i «Si us plau» mentre ens trepitgen!

`bb({ mouth:"scream", eyes:"scream" })`

b: Abraçarem tants fanals, que se'ns quedaran els braços plens de ronya i alumini!

```
bb({ mouth:"normal", eyes:"normal" });
hong( body:"chin" });
```

h: Nah, tens raó. Les «capacitats socials» no poden ser només per complaure a la resta, també han de posar *barreres.*

`hong( body:"one_up" });`

h: No podem invitar a ningú a casa, si abans no tenim parets que l'aguantin.

```
hong( eyes:"angry", mouth:"narrow" });
bb( eyes:"annoyed", mouth:"smile" });
```

h: També... re: la imatge dels braços... *eugh??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: Podríem fallar. Oblida-ho, realment *fallarem*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: I està bé! Fallar és com tothom aprèn coses noves!

`hong({ body:"normal", eyes:"normal" });`

h: Fallem cap endavant entre els dos, vinga?

`bb({ eyes:"normal_r" });`

b: I tant, suposo... al pitjor dels casos, podem escapar del poble amb una nova identitat.

`bb({ eyes:"normal" });`

h: Crec que això només costa dos bitcoins avui dia.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Podem fer uns experiments!

`hong({ body:"chin" });`

h: Podem trucar a un amic per xerrar, retrobar-nos amb un vell col·lega o senzillament parlar amb un barista.

`hong({ body:"normal" });`

h: Potser ens adonem que som més agradables del que pensem.

`bb({ eyes:"annoyed" });`

[I si això són petites «victóries» fàcils?](#act4_alone_experiment_cheap)

[I si això és una molèstia pels altres?](#act4_alone_experiment_burden)

[Però una xerrada no és el nostre jo *real*!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: Si ens posem un somriure sense profunditat, mai connectarem amb ningú,

`bb({ eyes:"super_sad" });`

b: *Però* si ens obrim, altres veuran el nostre pertorbador interior!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Fes volta.

b: Què.

`hong({body:"hands_1"})`

h: Quan els gossos volen demostrar amor i confiança, es fan vulnerables exposant la panxa.

`hong({body:"one_up"})`

h: Potser *encara* no tenim la seguretat per estar massa vulnerables, però si entrenem el que cal,

`hong({body:"normal", eyes:"surprise"})`

h: Un dia podrem ensenyar a la gent el nostre jo real – pertorbats, humans.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: Faré volta si em dones una llaminadura.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Dir «hola» al barista no és exactament el premi d'or a les Olimpiades Xerrameques.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: Ho serà per a *nosaltres!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: A l'arena social, no seríem ni pes ploma, però ens apropem a... pes quark.

`hong({ body:"normal", eyes:"normal" });`

h: Si hem de començar amb victòries petites i fàcils, que així sigui. Haurem de trepitjar el 1r esglaó abans del 1000è.

b: Sí! Potser després de dir «Hola», podem continuar amb un...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *«Com estàs?»*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *«Tot bé!»*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Potser el barista només vol fer els maleïts cafès, no ser un *experiment* per demostrar que les nostres capacitats socials són terribles.

`bb({ eyes:"annoyed" })`

h: Doncs, si resulta que nosaltres *som* una molèstia...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: També està bé saber-ho!

`hong({ eyes:"normal" });`

h: Podem aprendre com preguntar de forma proactiva a la gent amb què se senten còmodes, per respectar els límits de la resta.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Ja m'entens, són les estupideses als pamflets de l'hospital.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: Vull defensar les teves necessitats morals, el desig de ser millor persona,

`bb({ eyes:"sad_d" })`

b: Però sembla que, al cap i a la fi, estem tan essencialment... trencats.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: I no em diguis que *no* estem malament del cap. Hem saltat d'un *sostre*.
{{/if}}

{{if !_.INJURED}}
b: I no em diguis que *no* estem malament del cap. Quasi saltem d'un *sostre*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: No sé, *he* escollit què dir molta estona. Què vols dir *tu*, humà?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Un altre cop, és el teu torn, humà. Què penses?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: Vols afegir alguna cosa, humà?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Estem trencats. Arreglem-nos.](#act4_bad_fix)

[Estem trencats. Acceptem-ho.](#act4_bad_accept)

[Gràcies.](#act4_thanks) `_.thanks_for = "pel meu benestar moral";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: Podem treballar a tenir millors hàbits, intentar tenir una vida similar al que valorem.

`hong({body:"one_up"});`

h: I si ho necessitéssim, podem tenir ajuda professional – un terapeuta o orientador.

`hong({body:"normal"});`

h: Hi han de formes per arreglar-nos.

[I si no podem arreglar tot?](#act4_bad_fix_cant)

[I si arreglem *massa*?](#act4_bad_fix_too_much)

[No ens podem permetre ajuda professional.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, tens raó.

h: No podem arreglar-ho tot.

`bb({mouth:"scream", eyes:"scream_sad"});`

b_ Ahhh ho sabia estarem trencats per sempre!

`hong({eyes:"surprise"});`

h: Però almenys podem estar *menys* trencats.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Les ferides se sanen amb el temps, però mai se'n van. I està bé.

`bb({eyes:"annoyed_r"});`

b: Potser. A més,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Les cicatrius són *sexis.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: No facis això si us plau.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: Potser sonarà malaltís el que diré, però... una part meva *vol* aquest desordre.

`bb({ eyes:"angry" })`

b: Vull dir, sense ell, no seríem *avorrits?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Sense el desordre, no seria el nostre art bàsic i sense ànima?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Sense el desordre, no seríem incapaços de connectar amb amics amb aquest desordre?

`bb({ eyes:"sad", body:"chest" })`

b: Si mai estem satisfets amb la vida, pararíem d'inspirar-nos a fer grans obres?

`hong({ MOUTH_LOCK:true })`

h: ...

h: Si és possible tenir por a... «no tenir més pors»...

h: No crec que ens quedarem sense pors.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, sí! Buf! Quina alegria!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: «Doctor, em fa angoixa pagar 100 $/hora només per a què em preguntis *"com et fa sentir això?"*»

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: «Mm-hmm. I com et fa sentir això?»

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, és una preocupació molt raonable.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: I realment és un fàstic que la assistència per la salut mental no sigui assequible per a molta gent.

`hong({ eyes:"normal", mouth:"normal" });`

h: Però, sempre hi ha opcions de baix cost o fins i tot de franc:

`hong({ body:"chin" })`

h: Grups d'ajuda, teràpia en línia, centres de salut per a estudiants o sense ànims de lucre...

`hong({ body:"hands_1" })`

h: Treballar hàbits com la meditació, dormir bé, parlar amb amics regularment, aprendre coses noves...

`hong({ body:"hands_2" })`

h: Anar a la biblioteca per agafar llibres de préstec sobre psicoteràpia basats en evidències.

`hong({ body:"one_up" })`

h: Hi ha una llista molt ampla al final d'aquest joc!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Caram, la quarta paret no ha durat massa.

`hong({ body:"point" });`

h: Algunes coses Són més importants que les conveniències narratives. Com ara la salut mental.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: Vull dir, això és el que diuen els terapeutes, oi? Que acceptis les teves emocions, fins i tot les negatives?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Un moment.

[«Acceptar» com en *rendir-se*?](#act4_bad_accept_give_up)

[«Acceptar» com en *aprovar*?](#act4_bad_accept_approve)

[«Acceptar» com en *punt per punt*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Creus que Martin Luther King podria haver dit «Ai que mal no podem asseure'ns al davant de l'autobús, però hem d'*acceptar*»?

`bb({ eyes:"angry_r", body:"two_up" });`

b: Per què el complex industrial d'autoajuda pensa que retre l'espasa és una mena de *saviesa profunda*?

`bb({ eyes:"annoyed", body:"normal" });`

h: Crec que els terapeutes diuen que hem d'«acceptar» les coses dolentes en el sentit de reconèixer que estan allà i que és difícil canviar-les,

h: Però no necessàriament s'ha de trencar un compromís per canviar.

`bb({ eyes:"suspect" });`

b: Doncs, els terapeutes haurien de dir *reconèixer*, no *acceptar*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Sí, i ara que ho dius, «acceptar» és bastant confús.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Jo ho puc *reconèixer*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Com si fos *bo* el que estiguem trencats? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: Tots els guionistes de Hollywood que romantitzen les malalties mentals són uns punyeters!

`bb({ eyes:"angry", body:"two_up" });`

b: Tenir una malaltia mental és *una parida*! Arrabassen *vides* a la gent! Per què hauríem d'«acceptar-ho»?!

`bb({ body:"normal" });`

h: Crec que els terapeutes diuen que hem d'«acceptar» les nostres emocions en el sentit de ser pacients amb elles.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Com amb les sorres movedisses, on cal més estirar-se i esperar amb paciència,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Lluitar contra tu, la meva por, m'ha portat a l'hospital.
{{/if}}

{{if !_.INJURED}}
h: Lluitar contra tu, la meva por, quasi em porta a l'hospital.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: La solució, però, és fer el que fem ara – no lluitar, sinó conviure amb paciència.

`bb({ eyes:"annoyed" });`

b: Doncs haurien de dir *allò* en comptes d'una paraula tan complicada com «acceptar».

`hong({ body:"chin", eyes:"annoyed" });`

h: Sí, i ara que ho dius, «acceptar» és bastant confús.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: No accepto «acceptar».

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: Però ja *sabem* que no hauries de fer-me cas punt per punt.

`bb({ eyes:"sad_u", body:"two_up" });`

b: El problema és que et vull ajudar, però se'm dona fatal trobar les paraules!

`bb({ eyes:"sad", body:"normal" });`

h: Crec que els terapeutes diuen que hem d'«acceptar» les nostres emocions en el sentit de «no lluitar contra elles o ignorar-les».

`hong({ eyes:"surprise", body:"one_up" });`

h: Escoltar-te, treballar *amb* tu, però no prendre el que diguis com si fos a missa.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Doncs, els terapeutes haurien de dir *allò* en comptes d'un mot tan confús com ara «acceptar».

`hong({ body:"chin", eyes:"annoyed" });`

h: Suposo que també se'ls dona fatal escollir les paraules, a més.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Vols discutir alguna cosa més?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: Tens alguna cosa més al teu trist cor?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[Tinc por que ens puguin fer mal.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[Tinc por que ens deixin sols.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[Tinc por que ens vegin com mala gent.](#act4_bad)
{{/if}}

[Nah, ja estic bé.](#act4c_prelude)

# act4_something_else_2

h: D'acord, crec que hem discutit totes les nostres pors.

b: Sí, només hi ha tres pors.

h: Sip, tres exactes.

b: Quina conveniència.

(#act4c)

# act4c_prelude

h: Bona xerrada, grup.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b: Això no és només un *joc*, saps.

`bb({eyes:"angry_d", body:"one_up"})`

b: Formar una relació sana amb les teves emocions no és tan fàcil com clicar botons a la pantalla.

`bb({eyes:"sad", body:"normal"})`

b: *Podem* estar en pau?

b: *Podem* treballar junts, com un equip?

`hong({eyes:"sad", body:"one_up"})`

h: Ara,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: D-Disculpa...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: U-U-Us importaria si segués amb vosaltres per menjar?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *Aquest* és qui t'agrada? I per què s'asseu com si fos un psicòpata assassí?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Preguntar a qui t'agrada si pots seure al seu costat? No t'adones que semblem uns *pesats*?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *Aquest* és qui t'agrada? Hem interromput la seva pau i calma! Som una càrrega!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: V-Vull dir- està, està bé si no vols, només...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Espera, no et vaig veure a la festa?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Sí, i tant! Pots venir.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Perdona, però estimaria estar en pau ara.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Sí, estaves al sofà! A la primera festa que vaig atendre...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Quan vaig tenir un atac de pànic i vaig donar un cop a l'hoste.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Quan vaig tenir un atac de pànic i vaig sortir corrents.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Espera humà, potser els estem incomodant.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no volia fer-vos sentir incòmodes!

`publish("act4", ["hong_to_alshire",4]);`

h2: Estava recordant un rostre amable, ja està.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH HO SABIA! ÉS UN PSICÒPATA PERILLÓS IMPULSIU!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH LA SEVA PRIMERA IMPRESSIÓ NOSTRA HA SIGUT «HA VIST EL NOSTRE TRAUMA»! ENS ODIA!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH HEM REMEMORAT EL TRAUMA D'ALGÚ. LA NOSTRA PRESÈNCIA FA MAL ALS ALTRES.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Un segon, humà, semblen incòmodes.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, cap pressió!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Només dic que si vols seure aquí pots fer-ho.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: SÓN *MASSA* AMISTOSOS! COM EN TED BUNDY, L'ASSASSÍ EN SÈRIE!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: NOMÉS SÓN AMABLES PERQUÈ SOM NOSALTRES! NINGÚ *VOLDRIA* ESTAR AMB NOSALTRES!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH SEMPRE FEM QUE ELS ALTRES SE SENTIN MALAMENT! SOM UN GRA AL CUL DE LA TERRA!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Un segon, humà, potser els estem incomodant.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no volia semblar maleducat!

`publish("act4", ["hong_to_alshire", 6]);`

h2: Només necessito un temps per processar les meves emocions. No t'ho prenguis malament.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: QUINA MENA DE RETORÇATS PENSAMENTS TENEN?! QUINS DESITJOS PERVERSOS OMPLEN AQUEST COR PSICÒPATA?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: ENS HAN REFUTAT PERSONALMENT! MAI SEREM ESTIMATS!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: HEM INTERROMPUT EL SEU PROCESSAMENT EMOCIONAL! ARA ESTAN TRAUMATITZATS PER SEMPRE I LA CULPA ÉS NOSTRA!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE CÓRRE

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: Heh. Que estrany. Em pregunto que els passava pel cap.

`publish("act4", ["hong_closer", 2]);`

h: Què deies?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Eh, m'he oblidat. Una cosa de treball i equips?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: Diuen que has de «fer pau» amb les teves emocions com si aquestes fossin *criminals de guerra*.

`publish("act4", ["bb_closer", 7]);`

b: Però vull tenir més que pau amb tu! Vull que siguem *aliats!*

`publish("act4", ["bb_closer", 3]);`

b: Vull ser un bon gos guardià. Com la set i la fam són alarmes per a les necessitats físiques,

`publish("act4", ["bb_closer", 8]);`

b: Vull ser l'alarma per a les teves necessitats *psicológiques* – les teves necessitats de seguretat, de pertànyer, de bondat.

`publish("act4", ["bb_closer", 1]);`

b: Però... se'm dona de pena el meu treball, necessito que m'entrenis.

`publish("act4", ["bb_closer", 4]);`

b: Però no soc ni «sempre vàlid», ni «sempre irracional». Només... faig l'intent. Doncs, si us plau,

`publish("act4", ["bb_closer", 30]);`

b: Ajuda'm a ajudar-te!

`publish("act4", ["bb_closer", 6]);`

b: Encara que ensenyar trucs a un gos vell *serà* un procés llarg. Potser faran falta *anys.*

`publish("act4", ["bb_closer", 3]);`

b: I de vegades aniré cap enrere, tornaré als meus antics hàbits.

`publish("act4", ["bb_closer", 2]);`

b: Lladraré a les ombres. T'espantaré amb les meves paraules. Potser et mostro imatges intrusives de... coses.

`publish("act4", ["bb_closer", 9]);`

b: Ho sento! Soc com un gos agitat d'un refugi! Els gossos agitats es caguen al teu llit de tant en tant!

`publish("act4", ["bb_closer", 4]);`

b: Però si em tens paciència... i et quedes i t'asseus amb mi...

`publish("act4", ["bb_closer", 8]);`

b: Potser pots domesticar a aquest llop.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Bon gos.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Bon humà.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: AAAAA ENCARA MENGES SOL QUINZE CIGARRETES AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA ENCARA NO POTS PRODUIR MENTRE MENGES SOM PARÀSITS DE LA SOCIETAT AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA ESTÀS MENJANT ENCARA MÉS PA BLANC AAAAA
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: BUB BUB BUB BUB BUB

(#credits)

