# latvian_women_short_prose_corpus

English below [click here](#SUMMARY) 

## KOPSAVILKUMS

Šajā repozitorijā ir apkopoti faili un kods, kas attiecas uz rakstu "Kārkla, Z., Matulis, H., 2022. Creation and Analysis of Corpus of Short Prose by Latvian Women Writers".

Divi galvenie datu analīzes un datu vizualizācijas faili – [**_050_TURPINATA_kermena_vardi_analize.ipynb**](_050_TURPINATA_kermena_vardi_analize.ipynb) un [**_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb**](_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb).

Mapē [**source_files**](source_files) pieejami visi csv, xlsx, txt faili kas tiek izmantoti kā izejas faili Jupyter Notebook failos, kā arī datu analīzes starprezultāti no šiem Jupyter Notebook faliem.

Mapē [**visualizations_pdf_files**](visualizations_pdf_files) pieejami dažādi rezultātu vizualizāciju faili pdf formātā.

**Sieviešu īsprozas korpuss** (259 teksti, 1893—2002) apstrādātā veidā noSketchEngine platformā ir pieejams [**šeit**](http://hdl.handle.net/20.500.12574/69). Atsevišķie teksti ir lemmatizēti, izmantojot ailab.nlp.lv morfoloģisko tageri. Autortiesību ierobežojumu dēļ pilni teksti nav izlasāmi. Taču ja jums pētnieciskos vai citos pamatotos nolūkos ir vajadzība tekstiem piekļūt, sazinieties, rakstot uz e-pastu haralds.matulis@gmail.com.


## FAILI

Šeit aprakstīti repozitorijā pieejamie faili, to loģiskā iepazīšanas secībā. Failu sapratnei var noderēt iepazīšanās ar augstākminēto rakstu, kur aprakstīti pētījuma mērķi, analizēti iegūtie starprezultāti un aprakstīti veiktie soļi. Failu nosaukumu numerācija saglabāta no oriģinālā projekta. Faili ir nedaudz patīrīti, taču pamatā tie ir darba faili, tāpēc vietumis informācija var atkārtoties.

[**_81_full_18885_words_sorted.xlsx**](/source_files/_81_full_18885_words_sorted.xlsx) – Excel fails, kur tabulārā formātā doti visi atrastie 18885 "ķermeņa vārdi" un to "konteksts" – 5 vārdi pirms un 5 vārdi pēc. Failā ir sekojošas kolonnas: "fleksīvā forma", "lemma", "vārdšķira" – attiecas uz atrasto "ķermeņa vārdu"; "indekss tekstā" – apzīmē atrastā ķermeņa vārda atrašanās vietu konkrētajā tekstā; "teksta_fragments" – ķermeņa vārds iekš konteksta; "teksta nosaukums".
Teksti šajā failā ir sakārtoti hronoloģiski, no vecākā uz jaunāko.

[**_40_kermena_vardi_vardskira_konteksts_18855_atrasti.csv**](source_files/_40_kermena_vardi_vardskira_konteksts_18855_atrasti.csv) – csv formāta fails, kurā ir visa tā pati informācija, kas iepriekšējā Excel failā, tikai csv formātā. No šī faila tiek ielasīta informācija, kas turpmāk tiek izmantota Jupyter Notebook failos, tāpēc šis fails šeit tiek dots. Taču verot šo failu Excel programmā, varētu būt problēma ar latviešu burtiem – tāpēc ieskata gūšanai labāk lietot iepriekšējo Excel failu (_81_full_...)

[**_83_five_percent_sample_AR_KATEGORIJAM_pec_tuvlasijuma.xlsx**](_83_five_percent_sample_AR_KATEGORIJAM_pec_tuvlasijuma.xlsx) – Excel fails, kurā izveidota izlase ar 5 procentiem visu atrasto ķermeņa vārdu, un ar tuvlasījuma metodi katrs morfoloģiskā tagera atrastais ķermeņa vārds klasificēts kādā no 5 grupām: "patiess ķermeņa vārds", "neattiecas uz cilvēku", "metafora", "idiomātisks izteiciens", "nepareizi atpazīts VAI nav ķermeņa vārds". Šī izlase tika veidota ņemot katru 20 atrasto ķermeņa vārdu no hronoloģiski sakārtotiem tekstiem. Vairāk par klasifikācijas grupām un atradumiem skatīt rakstā.


[**_050_TURPINATA_kermena_vardi_analize.ipynb**](_050_TURPINATA_kermena_vardi_analize.ipynb) – Jupyter Notebook DATU ANALĪZES fails ar šādiem starprezultātiem: 
+ "5 procentu izlases faila izveidošana";
+ "Komentāri ejot cauri failam un skatoties izņēmumus starp ķermeņa vārdiem" (garāks saraksts nekā pdf rakstā);
+ ķermeņa vārdu faila (18855) attīrīšana no nepareizi atpazītajiem vārdiem un saīsināšana uz 17835 rindām. (Precizētais, saīsinātais 17835 ķermeņa vārdu fails csv formātā pieejams: [**_54_PRECIZETS_kermena_vardi_vardskira_konteksts_17835_attiriti.csv**](_54_PRECIZETS_kermena_vardi_vardskira_konteksts_17835_attiriti.csv))
+ visi unikālie atrastie ķermeņa vārdi latviski (74 – nošķirot atsevišķi vārdu pamatformas un deminutīvus), un daudzums katram vārdam.
+ tabula ar top10 ķermeņa vārdiem - latviski, angliski, absolūtie skaitļi, procentuālais īpatsvars. (Atsevišķā failā šī tabula pieejama: [**_87_top10_lemmas_latviski_angliski_procenti.xlsx**](_87_top10_lemmas_latviski_angliski_procenti.xlsx))
+ ķermeņa vārdu sadalījums pa 4 grupām – "VISS_ĶERMENIS", "ĶERMEŅA_DAĻAS", "GALVA_UN_DAĻAS", "CITI_VĀRDI" – iekš katra teksta. Pieejami arī kā atsevišķi faili: absolūtajos skaitļos [**_88_kermena_vardi_4_grupas_absolute_counts.xlsx**](_88_kermena_vardi_4_grupas_absolute_counts.xlsx) un relatīvajos skaitļos "uz 100 vārdiem" [**_89_kermena_vardi_4_grupas_RELATIVE_counts.xlsx**](_89_kermena_vardi_4_grupas_RELATIVE_counts.xlsx). Rezultāti šajos divos failos sakārtoti, sākot ar visblīvāko ķermeņa vārdu izplatību.


[**_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb**](_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb) – Jupyter Notebook DATU VIZUALIZĀCIJAS fails ar šādiem starprezultātiem:
+ Top10 biežākie ķermeņa vārdi = roka, acs, galva, seja, kāja, mats, plecs, lūpa, pirksts, mute
+ Top10 biežākie ķermeņa vārdi – to relatīvā izplatība KATRĀ TEKSTĀ
+ Top10 biežākie ķermeņa vārdi – relatīvā izplatība pa DEKĀDĒM
+ angliski: Most Used Body Words – their Relative Frequency in DECADES
+ Top10 biežākie ķermeņa vārdi – to relatīvā izplatība pa vēsturiskiem LAIKMETIEM
+ kopējā ķermeņa vārdu relatīvā izplatība – uz 100 vārdiem – hronoloģiski visos tekstos
+ angliski: Relative Frequency of Body Words – per 100 Words – chronologically in all texts
+ ķermeņa vārdi uz 100 vārdiem – relatīvā izplatība pa DEKĀDĒM
+ ķermeņa vārdi uz 100 vārdiem – relatīvā izplatība pa LAIKMETIEM



[papildināts 27.12.2022]










## SUMMARY

This repository contains files and code related to "Kārkla, Z., Matulis, H., 2022. Creation and Analysis of Corpus of Short Prose by Latvian Women Writers".

The two main data analysis and data visualisation files are [**_050_TURPINATA_kermena_vardi_analize.ipynb**](_050_TURPINATA_kermena_vardi_analize.ipynb) and [**_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb**](_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb).

The [**source_files**](source_files) folder contains all csv, xlsx, txt files that are used as output files in Jupyter Notebook files, as well as intermediate data analysis results from these Jupyter Notebook files.

The [**visualizations_pdf_files**](visualizations_pdf_files) folder contains a variety of results in pdf format.

The **Latvian Women Short Prose Corpus** (259 texts, 1893-2002) is available in processed form from the SketchEngine platform at [**here**](http://hdl.handle.net/20.500.12574/69). The individual texts have been lemmatised using the ailab.nlp.lv morphological tagger. Due to copyright restrictions, the full texts cannot be made public. However, if you need access to the texts for research or other legitimate reasons, please contact haralds.matulis@gmail.com.


## FILES

This describes the files available in the repository, in their logical order. To understand the files, it may be useful to consult the above-mentioned article, which describes the objectives of the study, analyses the intermediate results obtained and describes the steps taken. The numbering of the file names is kept from the original project. The files have been cleaned up a bit, but they are basically working files, so information may be repeated in places, but in general everything should work.

[**_81_full_18885_words_sorted.xlsx**](_81_full_18885_words_sorted.xlsx) - Excel file giving all 18885 "body words" found and their "context" - 5 words before and 5 words after - in tabular format. The file contains the following columns: "inflectional form", "lemma", "part of speech" - referring to the found "body word"; "index in text" - denoting the location of the found body word in the given text; "text_fragment" - body word within the context; "text name".
The texts in this file are arranged chronologically, from oldest to newest.

[**_40_kermena_vardi_vardskira_konteksts_18855_atrasti.csv**](_40_kermena_vardi_vardskira_konteksts_18855_atrasti.csv) - csv format file containing all the same information as the previous Excel file, but in csv format. This file is used to read in the following Jupyter Notebook files, so this file is given here. However, when opening this file in Excel, there might be a problem with the Latin characters - so it is better to use the previous Excel file (_81_full_...) if only to gain overview of the data.

[**_83_five_percent_sample_AR_KATEGORIJAM_pec_tuvlasijuma.xlsx**](_83_five_percent_sample_AR_KATEGORIJAM_pec_tuvlasijuma.xlsx) - Excel file containing a sample of 5 percent of all the body words found; by using the close reading method, each body word found by the morphological tagger is classified into one of 5 groups: "true body word", "does not refer to a person", "metaphor", "idiomatic expression", "misrecognized OR not a body word". This sample was made taking every 20th of body words found in the chronologically ordered texts. For more information on the classification in groups and the findings, see the article.


[**_050_TURPINATA_kermena_vardi_analize.ipynb**](_050_TURPINATA_kermena_vardi_analize.ipynb) - Jupyter Notebook DATA ANALYSIS file with the following intermediate results: 
+ "Creating a 5 percent sample file";
+ "Comments on exceptions amongst found body words" (longer list than in the pdf article);
+ cleaning the body words file (18855) of falsely identified words and truncating it to 17835 lines. (The refined, truncated 17835 body word file in csv format is available at: [**_54_PRECIZETS_kermena_vardi_vardskira_konteksts_17835_attiriti.csv**](_54_PRECIZETS_kermena_vardi_vardskira_konteksts_17835_attiriti.csv))
+ all unique body words found in Latvian (74 - separating base form and diminutives), and the quantity for each word.
+ table with top 10 body words - Latvian, English, absolute numbers, percentages. (In a separate file this is available: [**_87_top10_lemmas_latviski_angliski_procenti.xlsx**](_87_top10_lemmas_latviski_angliski_procenti.xlsx))
+ breakdown of body words into 4 groups - "WHOLE_BODY", "BODY_PARTS", "HEAD_AND_PARTS", "OTHER_WORDS" - within each text. Also available as separate files: in absolute numbers [**_88_kermena_vardi_4_grupas_absolute_counts.xlsx**](_88_kermena_vardi_4_grupas_absolute_counts.xlsx) and in relative numbers "per 100 words" [**_89_kermena_vardi_4_grupas_RELATIVE_counts.xlsx**](_89_kermena_vardi_4_grupas_RELATIVE_counts.xlsx). The results in these two files are sorted starting with the texts with highest frequency of body words.


[**_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb**](_70_TURPINATS_VIZUALIZACIJAS_kermena_vardi.ipynb) - Jupyter Notebook DATA VISUALIZATION file with the following intermediate results:
+ Top10 most frequent body names = hand, eye, head, face, leg, hair, shoulder, lip, finger, mouth
+ Top10 most frequent body words - their relative distribution IN EACH TEXT
+ Top 10 most frequent body words - relative distribution by TEXT
+ Most Used Body Words - their Relative Frequency in DECADES
+ Top10 Most Frequent Body Words - their Relative Frequency by Historical PERIOD
+ Relative frequency of total body words - per 100 words - chronologically in all texts
+ Relative Frequency of Body Words - per 100 Words - chronologically in all texts
+ Relative frequency of body words - per 100 words - by DECADES
+ Body words per 100 words - relative frequency by TIME

[last updated on 27.12.2022]












