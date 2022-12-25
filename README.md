# latvian_women_short_prose_corpus

English below [ saite ]

## KOPSAVILKUMS

Šajā repozitorijā ir apkopoti faili un kods, kas attiecas uz rakstu "xx". Ja jūs neesat šeit nokļuvuši no paša raksta, ar to varat iepazīties ŠEIT (saite uz pdf failu šajā repozitorijā). Tā ir raksta pre-print versija.

Divi galvenie datu analīzes un datu vizualizācijas faili – **_050_TURPINATA_kermena_vardi_analize.ipynb** un **_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb**.

Mapē **source_files** pieejami visi csv, xlsx, txt faili kas tiek izmantoti kā izejas faili Jupyter Notebook failos, kā arī datu analīzes starprezultāti no šiem Jupyter Notebook faliem.

Mapē **visualizations_pdf_files** pieejami dažādi rezultātu vizualizāciju faili pdf formātā.

**Sieviešu īsprozas korpuss** (259 teksti, 1893—2002) apstrādātā veidā ir pieejams [saitē] (https://korpuss.lv/id/%C4%AAsprozaS). Atsevišķie teksti ir lemmatizēti, izmantojot ailab.nlp.lv morfoloģisko tageri. Autortiesību ierobežojumu dēļ pilni teksti nav izlasāmi. Taču ja jums pētnieciskos vai citos pamatotos nolūkos ir vajadzība tekstiem piekļūt, sazinieties, rakstot uz e-pastu haralds.matulis@gmail.com.


## FAILI

Šeit aprakstīti repozitorijā pieejamie faili, to loģiskā iepazīšanās secībā. Failu sapratnei var noderēt iepazīšanās ar augstākminēto rakstu, kur aprakstīti pētījuma mērķi, analizēti iegūtie starprezultāti un aprakstīti veiktie soļi. Failu nosaukumu numerācija saglabāta no oriģinālā projekta. Faili ir nedaudz patīrīti, taču pamatā tie ir darba faili, tāpēc vietumis informācija var atkārtoties, bet kopumā visam vajadzētu strādāt.

**_81_full_18885_words_sorted.xlsx** – Excel fails, kur tabulārā formātā doti visi atrastie 18885 "ķermeņa vārdi" un to "konteksts" – 5 vārdi pirms un 5 vārdi pēc. Failā ir sekojošas kolonnas: "fleksīvā forma", "lemma", "vārdšķira" – attiecas uz atrasto "ķermeņa vārdu"; "indekss tekstā" – apzīmē atrastā ķermeņa vārda atrašanās vietu konkrētajā tekstā; "teksta_fragments" – ķermeņa vārds iekš konteksta; "teksta nosaukums".
Teksti šajā failā ir sakārtoti hronoloģiski, no vecākā uz jaunāko.

**_40_kermena_vardi_vardskira_konteksts_18855_atrasti.csv** – csv formāta fails, kurā ir visa tā pati informācija, kas iepriekšējā Excel failā, tikai csv formātā. No šī faila tiek ielasīta informācija, kas turpmāk tiek izmantota Jupyter Notebook failos, tāpēc šis fails šeit tiek dots. Taču verot šo failu Excel programmā, varētu būt problēma ar latviešu burtiem – tāpēc ieskata gūšanai labāk lietot iepriekšējo Excel failu (_81_full_...)

**_83_five_percent_sample_AR_KATEGORIJAM_pec_tuvlasijuma.xlsx** – Excel fails, kurā izveidota izlase ar 5 procentiem visu atrasto ķermeņa vārdu, un ar tuvlasījuma metodi katrs morfoloģiskā tagera atrastais ķermeņa vārds klasificēts kādā no 5 grupām: "patiess ķermeņa vārds", "neattiecas uz cilvēku", "metafora", "idiomātisks izteiciens", "nepareizi atpazīts VAI nav ķermeņa vārds". Šī izlase tika veidota ņemot katru 20 atrasto ķermeņa vārdu no hronoloģiski sakārtotiem tekstiem. Vairāk par klasifikācijas grupām un atradumiem skatīt rakstā.


**_050_TURPINATA_kermena_vardi_analize.ipynb** – Jupyter Notebook DATU ANALĪZES fails ar šādiem starprezultātiem: 
+ "5 procentu izlases faila izveidošana";
+ "Komentāri ejot cauri failam un skatoties izņēmumus starp ķermeņa vārdiem" (garāks saraksts nekā pdf rakstā);
+ ķermeņa vārdu faila (18855) attīrīšana no nepareizi atpazītajiem vārdiem un saīsināšana uz 17835 rindām. (Precizētais, saīsinātais 17835 ķermeņa vārdu fails csv formātā pieejams: **_54_PRECIZETS_kermena_vardi_vardskira_konteksts_17835_attiriti.csv**)
+ visi unikālie atrastie ķermeņa vārdi latviski (74 – nošķirot atsevišķi vārdu pamatformas un deminutīvus), un daudzums katram vārdam.
+ tabula ar top10 ķermeņa vārdiem - latviski, angliski, absolūtie skaitļi, procentuālais īpatsvars. (Atsevišķā failā šī tabula pieejama: **_87_top10_lemmas_latviski_angliski_procenti.xlsx**)
+ ķermeņa vārdu sadalījums pa 4 grupām – "VISS_ĶERMENIS", "ĶERMEŅA_DAĻAS", "GALVA_UN_DAĻAS", "CITI_VĀRDI" – iekš katra teksta. Pieejami arī kā atsevišķi faili: absolūtajos skaitļos (**_88_kermena_vardi_4_grupas_absolute_counts.xlsx**) un relatīvajos skaitļos "uz 100 vārdiem" (**_89_kermena_vardi_4_grupas_RELATIVE_counts.xlsx**). Rezultāti šajos divos failos sakārtoti, sākot ar visblīvāko ķermeņa vārdu izplatību.


**_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb** – Jupyter Notebook DATU VIZUALIZĀCIJAS fails ar šādiem starprezultātiem:
+ Top10 biežākie ķermeņa vārdi = roka, acs, galva, seja, kāja, mats, plecs, lūpa, pirksts, mute
+ Top10 biežākie ķermeņa vārdi – to relatīvā izplatība KATRĀ TEKSTĀ
+ Top10 biežākie ķermeņa vārdi – relatīvā izplatība pa DEKĀDĒM
+ angliski: Most Used Body Words – their Relative Frequency in DECADES
+ Top10 biežākie ķermeņa vārdi – to relatīvā izplatība pa vēsturiskiem LAIKMETIEM
+ kopējā ķermeņa vārdu relatīvā izplatība – uz 100 vārdiem – hronoloģiski visos tekstos
+ angliski: Relative Frequency of Body Words – per 100 Words – chronologically in all texts
+ ķermeņa vārdi uz 100 vārdiem – relatīvā izplatība pa DEKĀDĒM
+ ķermeņa vārdi uz 100 vārdiem – relatīvā izplatība pa LAIKMETIEM



[kad pēdējoreiz papildināts]








