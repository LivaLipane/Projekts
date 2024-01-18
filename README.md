# SPORTA ZĀLES "MYFITNESS" UN RTU MEŽA IELAS SALĪDZINĀŠANA

## Programmas uzdevums:
### Noteikt, vai izdevīgāk ir  apmeklēt "Myfitness" sporta zāli vai RTU sporta zāli Meža ielā, pēc viena apmeklējuma maksas. RTU sporta zālē ir fiksēta viena apmeklējuma cena neatkarīgi no mēnesī apmeklēto reižu skaita vai vizītes ilguma. Otrā sporta klubā- fiksēta mēneša maksa. Ja mēnesī zāles apmeklējums nav pietiekams, esošā sporta zāle vairs nav izdevīga un ir vērts apdomāt abonementa maiņu.

## Python bibliotēkas:
### Pathlib tiek izmantots, lai izveidotu objektu, kas pārstāv ceļu uz failu, izmantojot ievadīto faila nosaukumu. Tālāk tas tiek izmantots faila atvēršanai un citām operācijām. Ar PTPDF2 palīdzību informācija tiek apstrādāts PDF dokuments, no kura tiek iegūta nepieciešamā informācija (mēneša rēķins un datums). Izmantojot bibliotēku Openpyxl, tiek nolasīta un analizēta informācija no Excel failiem. Šajā gadījumā tiek salīdzināti datumi un veiktas atbilstošās informācijas iegūšana.

## Programmas darbības aprakstīšana:
### Ar Pathlib palīdzību lietotājs izvēlas, kura mēneša rēķinu vēlas apskatīt- jūliju, augustu vai septembri. No atbilstošā rēķina (PDF fails) iegūst divas vērtības- mēnesi un summu (kas katru periodu var mainīties, piemēram, papildus soda naudas piešķiršanas dēļ). Tā kā Excel failā mēnesis ir ierakstīts vārdiski, ir izveidots papildus CSV fails, lai katru periodu sasaistītu ar atbilstošo datumu (septembris, 09). Tālāk tiek piemeklēts atbilstošā mēneša Excel fails, kas satur apmeklējumu skaitu konkrētajā mēnesī, un saskaita apmeklētos datumus. Rēķina summu dala ar datumu skaitu un iegūst "Myfitness" konkrētā mēneša viena apmeklējuma maksu. Ja tā ir mazāka par RTU sporta zāles 3 EUR, tad nav vērts mainīt abonementu. Ja ir lielāka,- vajadzētu pievērst uzmanību nākotnes datiem un nepieciešamības gadījumā manīt to.
