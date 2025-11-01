# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: Salut!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *Ah* això sí que m'emplena.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: Saps, nano...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: Concretament, m'ha emplenat la bufeta.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: Em recordes a quan era més jove. Quan l'animal al meui cap em tormentava.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: M'agrada poder tornar el favor, i ajudar-te a matar a la bèstia tal i com jo vaig matar la meva.

```
publish("act3",["roofhunter",2]);
```

r: Ep, una pregunta: veritat o rep--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: REPTE!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: Haha! Bé.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: D'acord. Veus la piscina d'un blau claret d'allà baix?

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: Sí? A sis plantes d'aquí?

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: Salta.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: Espera, què?

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: L'animalet ha començat a queixar-se, oi?

```
publish("act3",["roofhunter",23]);
```

r: *Oh nooooo és perillós, no ho facisssss.*

```
publish("act3",["roofhunter",22]);
```

r: Això és per què necessitem reptes mortals! Festes a tope! Carpe diem! Esnifar coca del ^cul^ d'una prostituta, #YOLO!

```
publish("act3",["roofhunter",10]);
```

r: Mostra al animal que ens importa un *rave* els seus comentaris de ^merda^! Salta'n.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: Eh, però de vegades, em... la por té un sentit...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: Ho sento, et creus la propaganda de McMindfulness que diu que sentir-se malament és *bo?*

```
publish("act3",["roofhunter",17]);
```

r: Els ^imbècils^ que controlen aquest món ens donen a la *resta* ansietat i depressió,

```
publish("act3",["roofhunter",18]);
```

r: I doncs fan que les TED Talks ens diguin que «hem d'acceptar» estar ^fotuts^ i que «apreciem» al dimoni sadista al nostre cap!

```
publish("act3",["roofhunter",6]);
```

r: Nano, sé que *tu* saps que l'animal *fa mal* a la gent com nosaltres. Que *tortura* a gent com nosaltres.

```
publish("act3",["roofhunter",19]);
```

r: No és el nostre amic. És una bèstia salvatge, que ha de ser o bé *tranquil·litzada*...

```
publish("act3",["roofhunter",20]);
```

r: O bé ficar-li una *bala al cap*.

```
publish("act3",["roofhunter",27]);
```

r: Sinò, deixaràs que et guanyi.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: No. T'equivoques.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
 music('battle_dark_loop');
});
```

h2: No deixarè que guanyi.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: ^Collonut^! Crec en tu, nena! Mata'l! <3

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: no no no no no no

n: AQUEST CAPÍTOL TÉ DOS FINALS POSSIBLES. UN ÉS *MOLT, MOLT DOLENT.*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: ESCULL SÀVIAMENT. PROTEGEIX AL TEU HUMÀ

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAAH

`bb({ mouth:"normal" });`

n: BONA SORT

```
Game.clearText();
bb({ eyes:"start" });
```

[Humà, pots MORIR aquí!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[Això és estúpid i autodestructiu!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[Aquests boigs no són els teus amics!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: A--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: A--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Saps, podria creure't... si no ho haguessis intentat tantíssims cops.

h: Ets el llop que diu «que ve el llop».

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Ja has provat amb això.

b: humà, si us plau...

`hong({ eyes:"look_right" });`

h: Oh, *perdona* que les farmacèutiques no aprovin l'automedicació.

h: Mira'm, ^imbècil^, *tots* tenim formes de fer-te callar la ^puta^ boca.

`hong({ body:"look_up", eyes:"look_up" });`

h: Hi ha qui s'abraona al treball.

`hong({ body:"look_down", eyes:"look_down" });`

h: Hi ha qui s'abraona al sexe, les drogues, i actualitzar les recomanacions del Facebook.

`hong({ body:"normal", eyes:"look_right" });`

h: Hi ha qui s'abraona amb altra gent.

`hong({ eyes:"angry" });`

h: Jo m'abraonaré amb la piscina.

[T'has alcoholitzat i a SIS PLANTES](#act3_bad_1_harm)

[Caram, així em dones les gràcies?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[D'acord, ho reconec. L'he espifiada.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Fins i tot si caus a l'aigua, la tensió superficial et trencarà les costelles i una commoció *com a mínim!*

h: Ah.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: Vaig veure un rus fer això al YouTube un cop.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: J- Perdona, i les *gràcies*?

`bb({ eyes:"angry" });`

b: Això és precisament perquè *existeixo!* Perquè els humans no es poden protegir a si mateixos!

b: He intentat salvar-te el teu estúpid cul tota la meva vida i ara tu ho tiraràs t--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: UAU acabes de dir l'eufemisme més *^putíssimament^* brutal del mil·lenni!

`hong({ body:"yell_2" });`

h: Sí, tros de ^merda^ ple de sang! L'has espifiada un munt!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Més notícies, Capità Obvi?

[Però la venjança no soluciona res!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[Però ara *sí* que tinc la raó!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[T'he fet mal.](#act3_good_2a)


# act3_good_1_fail_revenge

b: Necessites tenir una relació més saludable amb les teves emocions, en comptes d'ofegar-les am--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: Si us plau, baixa l'ampolla i par--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: sisplau... no...

h: Tens una barra de via molt baixeta, llop.

h: Si fos tu, ara em pensaria les meves paraules amb cura.

`bb({ eyes:"normal" });`

[Vinga. M'he cansat de protegir-te.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[Tenia la raó.](#act3_bad_2_right)

[Ho sento.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: Vinga, salta. Mira quant m'importa.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Vinga. I de baix a dalt.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: ESPERA NO ALLÒ ERA PSICOLOGIA INVERSA HAVIES DE FER EL *CONTRARI* DEL QUE ET DEMANA--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: *Et* poses en perill. Els teus «amics» *t'estan* manipulant. I *tu* estàs manipulant als teus «amics».

`bb({ eyes:"sad" });`

b: Així doncs, humà... per què no em creus?!

h: Perquè tu mai creus en *mi*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Altres llops guardians tenen humans que es prenen el temps d'entrenar-los, per *aprendre* a treballar junts.

b: En comptes d'odiar als llops guardians per intentar protegir-los! Per què tu no pot--

`bb({ eyes:"normal" });`

h: Resposta ^fotuda^ment incorrecta.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *«L'única cosa a témer és el temor mateix».*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *«No et preocupis, sigues feliç!»*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: Tota la gent sàvia dels nostres temps diu: les emocions negatives són *dolentes!*

`hong({ eyes:"less_angry" });`

h: No cal dir-ho! Per això les van anomenar *negatives!*

b: humà... sisplau...

`hong({ eyes:"normal" });`

h: Fa una estona deia: «Vull alliberar-me d'aquest dolor».

h: Tinc el meu desig. No tinc dolors, ni penes, ni ansietat...

h: No sento absolutament res.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: Em vaig obsessionar tant amb protegir-te del dolor, que no vaig caure que *jo* era la causa d'aquest.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NO. F^OTIS^.

`hong({ body:"yell_1" });`

h: ^CAGO EN TOT^. Tant de temps et feia falta per adonar-te?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: Podies haver-nos salvat de tants perills, ^imbècil^ gran i suau. Com no has caigut en això abans?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...et *disculpes.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Disculpes per *què*?

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[Sento no haver sigut un bon protector.](#act3_good_3_protector)

[Sento no respectar-te.](#act3_good_3_respect)

[Ho sento.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[Sento tenir un humà tan horrible!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[Sento no respectar-te.](#act3_good_3_respect)

[Sento fer-te mal.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: És el meu deure avisar-te del perill real, però només lladrava als cotxes i al carter.

`bb({eyes:"sorry_up"});`

b: Lladrava a les ombres. Lladrava massa.

`bb({eyes:"sorry"});`

b: Només té sentit que vulguis posar-me un boç.

`bb({eyes:"sorry_down"});`

b: Ho sento.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: Jo havia de ser el *teu* gos guardià, però actuava com si haguessis d’*obeir-me*.

`bb({eyes:"sorry_up"});`

b: Hi ha una diferència entre protector i director de presó, i m'he passat del límit.

`bb({eyes:"sorry_down"});`

b: Ho sento.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: Em vaig obsessionar tant amb protegir-te del dolor, que mai vaig parar-me a pensar que *jo* era la causa.

`bb({eyes:"sorry_up"});`

b: He sigut un mal gos.

`bb({eyes:"sorry_down"});`

b: Ho sento.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Seh, total, ja era una mala idea.

h: Només he fet això per molestar-te i, doncs, ho he fet.

h: Deixem-ho com un empat, d'acord?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Vinga.

h: Vinga.

n: *EMPAT*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh, *vinga*. Després de tot el que t'ha fet l'animalet, et *rendeixes?*

r: Què et passa, nano? Tens *por?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Sí.

h2: Tinc por.

`publish('hong-next')`

h2: I està bé!

`publish('hong-next')`

h2: Està bé tenir por.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Han tancat la porta?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
