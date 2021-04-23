# Ghid pentru dezvoltare

Următoarele paragrafe conțin câteva sfaturi pentru a menține un standard bun al calității codului, a asigura funcționarea corectă a acestuia, și integrarea mai ușoară a echipei în proiect.

## Limba utilizată în cod

Preferați limba engleză pentru denumiri de variabile, mesaje interne de eroare etc., iar pentru interfață folosiți limba română, evident.

Ideea este următoarea: peste tot folosim API-uri și funcții care sunt denumite în limba engleză, documentațiile online despre limbaje, librării, tehnologii sunt toate în engleză, iar atunci termenii devin mai familiari. Datorită acestor factori, urmărind să menținem codul în limba engleză reușim să reducem încărcătura mentală a codului și devine mai ușor de citit.

## Formatare și linting

Păstrând codul formatat corespunzător și linterele "fericite", codul devine uniform, ușor de citit pentru toți, utilizează practicile idiomatice ale limbajului, nu conține lucruri inutile și devine mai puțin complex, chiar îmbunătățindu-i puțin performanța.

Linterele pot deveni enervante, mai ales dacă nu înțelegem ce vor de la noi. Soluția pentru asta este și va fi întotdeauna Google, unde se poate găsi ușor ce înseamnă o astfel de eroare și motivația din spatele verificării respective. Pentru un cost mic pe moment, îmbunătățim codul și ne îmbogățim cunoștințele pe termen lung.

## Testare

E neplăcut să le scrii. Pot deveni repetitive, îți pierzi răbdarea și le lași baltă. Tocmai ai lăsat baltă cea mai bună posibilitate de-ați documenta modul de funcționare al codului, cea mai sigură modalitate de verificare și prevenire a erorilor de implementare, și te-ai condamnat la un timp dublu pierdut săptămâna următoare, când realizezi că nu merge așa cum vrei. Mai rău, îngheață site-ul în timpul prezentării! Auăleu...

Acum că te-am convins, urmărește ca în testele tale să mimezi cât mai exact modul în care utilizatorul va folosi programul. Gândește-te la toate variantele de execuție ce pot avea loc și modelează-le prin testele tale. Cu alte cuvinte, încearcă să automatizezi ceea ce în mod normal ai face de mână. Testele trebuie să ofere siguranță, și numai mimând utilizarea reală o vor face.

Este important de ținut minte că testele nu trebuie să ruleze corect doar pe calculatorul tău. Acestea vor fi rulate la fiecare pull request, un total alt mediu față de calculatorul tău, ba chiar vor fi rulate și în mediul de producție. Asigură-te că vor funcționa peste tot la fel, folosește-te de variabile de mediu (environment variables) și documentează orice configurare suplimentară de care e nevoie.

## Pull requests

Când deschizi un pull request, oferă-i un titul sugestiv în primul rând. În descriere, menționează issues-urile care sunt legate de pull request-ul tău și informații ce consideri că sunt utile, care descriu schimbările tale (de exemplu, descrie lucruri a căror motivație nu este chiar evidentă, se folosesc de o funcționalitate nepopulară a limbajului/platformei etc.).

Utilizează keyword-uri de închidere: de exemplu, dacă PR-ul tău rezolvă issue-ul cu ID-ul 14, scrie așa în descriere:

```md
Close #14
```

Dacă rezolvi un issue cu un checklist pentru task-uri, bifează ceea ce ai rezolvat/implementat acolo, nu scrie în descrierea pull request-ului, pentru că repeți inutil informație.

Ca să fie un PR complet, cere review-ul unei persoane, adaugă-l în proiectele corespunzătoare și adaugă-i milestone-ul de care ține acest PR. De exemplu, pentru implementarea unei funcționalități sau a unor teste pentru frontend, vei cere review-ul unei persoane care se ocupă de frontend, vei adăuga PR-ul la proiectul "Frontend" si îi vei atribui milestone-ul "MVP concurs 4IT50".
