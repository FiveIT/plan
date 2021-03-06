# IDEE 

[**Business plan**][1]

*Nume* este o platformă ce pune la dispoziția elevilor cea mai mare colecție de eseuri și comentarii pentru operele cerute la bacalaureat. Scopul platformei este de a veni în ajutor tuturor elevilor: de la cei care nu reușesc să înțeleagă cerințele unui eseu de bac până la elevii de 10 care doresc să își perfecționeze lucrările și să își extindă perspectiva asupra operelor. Astfel, *Nume* poate asigura succesul tuturor elevilor la examenul de bacalaureat, indiferent de nevoile lor actuale.

## <a name="utilizatori"></a>Utilizatorii

Utilizatorii, înregistrați sau nu, sunt definiți după cum urmează:

* <a name="beneficii"></a>**Beneficii/Funcționalități disponibile**

  Nu este nevoie de un cont pentru a avea acces la colecția de eseuri și comentarii, [editorul de eseuri](#editor) și la [detectorul de plagiat](#plagiat). Utilizatorii ce au un cont beneficiază și de aceste funcționalități, la care se adaugă cele următor precizate.

  Elevii pot încărca propriile lor [lucrări](#continut), acestea fiind trecute prin procesul de [revizuire](#revizuire) al conținutului. De altfel, aceștia pot oferi [feedback](#feedback) pentru experiența lor pe platformă.

  Profesorii, în schimb, pot încărca lucrări fără ca acestea să mai fie revizuite. Aceștia au acces la lucrările care sunt în procesul de revizuire, putând verifica eseurile oricărui elev care dorește să-și publice lucrările pe platformă. Dacă au elevi [asociați](#asocieri), pot aproba sau respinge lucrările pe care elevii lor doresc să le încarce.
  
  Pentru mai multe informații despre rolul profesorilor pe platformă, vedeți secțiunea [Profesorii](#profesori).

* <a name="asocieri"></a>**Asocieri/relații între utilizatori**

  Elevii se pot asocia unuia sau mai multor profesori, pentru a primi aprobarea lucrărilor pe platformă fără a mai trece prin procesul de [revizuire](#revizuire). Asocierea se face numai dacă profesorul acceptă cererea (conceptual este similar unei cereri de prietenie, dar care nu este reciprocă).

  De exemplu, dacă un profesor are ca elev un utilizator existent, când respectivul încarcă un eseu, profesorul îl aprobă în funcție de evaluarea făcută la clasă.

* <a name="inregistrare"></a>**Înregistrarea/Crearea conturilor**

  Pentru a se înregistra, utilizatorii vor fi prezentați cu un formular simplu.

  În primul rând, formularul va cuprinde câmpuri pentru introducerea unui email și a unei parole. Parola nu va trebui să se supună vreunei constrângeri (desigur, decât o lungime minimă, ar fi ridicole parolele de o literă; pentru mai multe detalii, vezi [acest articol][2]).

  În al doilea rând, acesta va cuprinde o alegere unică pentru tipul contului: *elev* sau *profesor*. Dacă utilizatorul dorește să se înregistreze ca și profesor, va trebui să-și dovedească profesia.

  În ultimul rând, noul utilizator înregistrat își va preciza numele complet. Acesta va fi utilizat pentru detalierea cererilor de asociere și în alte locuri ce necesită cunoașterea persoanei care a inițiat acțiunea respectivă. Numele nu va apărea public (spre exemplu, ca autor al eseurilor încărcate).

* <a name="autentificare"></a>**Autentificarea**

  Utilizatorul se autentifică folosind email-ul si parola. Sesiunea acestuia va putea fi, desigur, reținută (funcția *remember me*).
  
  [//]: # (TODO: Oare să scăpăm de autentificarea clasică prin user și parolă? Argumente pro? Argumente contra?) 

## <a name="continut"></a>Conținutul

1. <a name="incarcare"></a>**Încărcarea conținutului**

    Lucrările de pe platformă sunt trimise de către elevi. Pentru cea mai bună experiență de utilizator, sunt acceptate o multitudine de formate:

    * Fișiere plain-text (`.txt`)
    * Fișiere Microsoft Office Word (`.doc`/`.docx`) și OpenOffice (`.odt`)
    * Surse publice Google Docs
    * Imagini (`.jpg/.jpeg`, `.png`, `.pdf`) ce conțin text imprimat sau scris de mână.

    După ce fișierul (fișierele) sunt încărcate, serverul extrage textul folosind serviciul corespunzător formatului. Conținutul fiind acum într-un format plain-text, este procesat pentru a asigura spațierea, capitalizarea, indentarea paragrafelor și utilizarea diacriticelor corecte și consistente. Acest pas pregătește lucrarea pentru [revizuire](#revizuire), dacă este necesar, și [publicare](#publicare).

    Totuși, înainte de a trimite lucrarea spre [revizuire](#revizuire), elevul mai are o șansă de a edita posibile greșeli (de ex. de recunoaștere a textului din poze) sau să-și ajusteze exprimarea, dacă i se pare necesar. Când totul este în regulă, elevul confirmă materialul, acesta fiind trimis în stagiul de revizuire.

1. <a name="revizuire"></a>**Revizuirea conținutului**

    Pentru a asigura calitatea și standardul lucrărilor, după [încărcare](#incarcare) acestea trec printr-un proces de revizuire. Există două cazuri particulare în acest proces:

    1. Lucrarea elevului nu a fost revizuită

        În această situație, eseul său este expus tuturor profesorilor înregistrați pe site pentru revizuire.

    1. Lucrarea elevului a fost revizuită fizic de un profesor

        În această situație, dacă profesorul este înregistrat pe site și contul elevului este [asociat](#asocieri) cu cel al respectivului profesor, elevul poate cere confirmarea profesorului respectiv (vezi secțiunea anterioară [beneficii](#beneficii)).

        În schimb, dacă profesorul nu este înregistrat elevul completează un mic formular cu numele profesorului și o adresă de email pentru a-l contacta. Autoritatea persoanei identificate de datele de contact precizate va fi stabilită de personalul platformei. Dacă există deja un cont de profesor identificat de adresa respectivă de email, elevul este invitat să se asocieze cu profesorul respectiv, procesul desfășurându-se apoi ca în paragraful anterior.
    
    În revizuire profesorul urmărește exact ceea ce urmărește la clasă, ținând cont de cerințele pentru bac. Înainte să ajungă în acest proces, lucrările pot trece printr-un filtru contra obscenităților, [plagiaturii](#plagiat) sau nerespectarea cerințelor ce pot fi determinate algoritmic, cum ar fi numărul de cuvinte sau poate chiar atingerea tuturor punctelor (introducere, curent literar, descrierea titlului, când există conflictul etc.). Ideea este ca acest proces de revizuire să se automatizeze cât de mult posibil, pentru a reduce nevoia de un număr mare de profesori implicați.

1. <a name="publicare"></a>**Publicarea conținutului**

    După ce lucrarea trece cu succes prin stagiile de [încărcare](#incarcare) și [revizuire](#revizuire), aceasta este publicată automat. După publicare, lucrarea este vizibilă tuturor utilizatorilor platformei, aceștia putând să o utilizeze spre a-și crea propriile lor lucrări. Aceasta nu mai poate fi reeditată! Schimbările subsecvente rezultă în necesitatea unei noi revizii de către profesor și complică strategiile de optimizare a performanței platformei.
    
    Conținutul încărcat va putea primi și un feedback anonim, nevizibil publicului, de la elevi: a fost de ajutor eseul pentru scopul tău? Dacă un eseu primește feedback negativ semnificativ, se va considera eliminarea acestuia de pe site. De ce nu este public acest feedback? Încercăm să evităm efectul de turmă. În mod natural, elevul va căuta cel mai bine privit conținut de pe platformă, voturile pozitive pentru acesta crescând exponențial, iar restul eseurilor, deși mai complexe, provocatoare, vor rămâne în umbră, conținutul astfel normalizându-se la un standard mediocru.

1. <a name="explorare"></a>**Explorarea conținutului**

    Elevul poate vedea toate lucrările de pe platformă, fie că este logat, fie că nu. Pe prima pagină este întâmpinat de o listă cu operele și personajele pentru care sunt publicate lucrările și de asemenea poate căuta opera sau personajul care îl interesează. Când găsește ceea ce caută, elevului îi va fi afișată o lucrare aleatorie și cu ajutorul unui buton poate să continue să răsfoiască printre eseuri, în ordine aleatorie. Desgiur, se poate întoarce înapoi, poate salva eseuri (ca și un bookmark), dar mai mult de atât: când găsește un paragraf, o idee care i se pare interesantă, acesta o poate salva la [idei](#idei).

    <a name="idei"></a>Ideile sunt grupate după opera sau personajul abordat în opera din care sunt luate. Elevul le poate vedea atunci când scrie un eseu în [editor](#editor). Acest sistem permite elevului să găsească ceea ce i-a atras atenția rapid, fără să mai caute printre eseurile salvate sau prin colecția întreagă.

## <a name="editor"></a>Editorul de eseuri

Punem la dispoziție elevilor atât posibilitatea de a încărca lucrări deja făcute, cât și de a le compune la noi pe platformă. Editorul de eseuri este un mediu simplu de editare text, care îți permite să răsfoiești prin eseuri (cele salvate sau chiar aleatoriu) și prin [ideile](#idei) tale salvate în timp ce scrii textul. Când ai terminat, îl publici, iar apoi îl poți exporta în formate cum ar fi Word.

## <a name="profesori"></a>Profesorii

Deoarece platforma garantează calitatea conținutului, este nevoie de profesori pentru a se asigura de aceasta: respectă lucrarea cerințele pentru bac? este corect dpdv gramatical, ortografic, al vocabularului? Astfel, profesorii [revizuiesc](#revizuire) lucrările după criteriile necesare și perspectiva lor personală.

## <a name="feedback"></a>Feedback

Vrem să ne asigurăm că experiența elevului pe platformă este una valoroasă, din care a învățat și care l-a ajutat să-și atingă scopul. Singurul mod prin care ne putem asigura că viziunea noastră se înfăptuiește nu poate fi altul decât un mijloc de comunicare cu utilizatorii platformei. Astfel că elevii pot lăsa un mesaj descriind experiența lor, ajutându-ne să o îmbunătățim după cum e cazul. Acest feedback va fi cerut automat, de exemplu după încărcarea primului eseu, sau după mai mult timp de utilizare al platformei.

## <a name="plagiat"></a>Plagiatura

Se pot ridica obiecții când vine vorba de posibilitățile de plagiatură pe care această platformă le poate oferi. Elevii pot copia cu exactitate conținutul altor esee și dat fiind numărul mare de surse este imposibil pentru profesor să recunoască plagiatura. Aceasta e o problemă ce nu exista până acum, dat fiind numărul mic de surse și calitatea lor slaba, însă cum această platformă rezolvă aceste două puncte slabe, consecințele negative trebuie combătute.

Platforma oferă astfel un detector de plagiat. Acesta caută prin baza de date a platformei fragmente din textul dat care se regăsesc și în alte texte, folosind o tehnică de diffing. După căutare, un raport este generat, care indică posibilele surse plagiate și un procentaj de plagiatură, astfel că cel care evaluează textul respectiv este capabil să tragă o concluzie finală asupra originalității textului.

Încărcarea textului pentru verificare se face asemenea [încărcării](#incarcare) unui eseu normal. Detectarea de plagiat este si un pas în [revizuirea](#revizuire) textului.

[1]: https://docs.google.com/presentation/d/1bKMsCSciHUsiMy7Lg7-0SCBnQGAnBxZ8NDw0_tS32g0
[2]: https://lifehacker.com/how-password-constraints-give-you-a-false-sense-of-secu-1830564360
