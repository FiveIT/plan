# Utilizator

Utilizatorul este, alături de lucrare, principala entitate de pe platformă.

## Numele utilizatorului

Pentru identificarea acestuia pe platformă, utilizatorul își specifică numele real al acestuia (nume de familie + prenume + nume mijlociu).

## Adresa de email

Adresa de email este utilizată, din nou, pentru identificarea utilizatorului pe platformă. Cum numele unui utilizator nu este garantat să fie unic comparat cu cel al celoraltor utilizatori, este nevoie de o modalitate pentru diferențierea acestora. Adresele de email sunt constrânse să fie unice, ceea ce înseamnă că este garantată identificarea facilă a utilizatorilor de către alți utilizatori, unde este necesar.

Adresa este vizibilă altor persoane în diferite măsuri și în anumite circumstanțe.

## Școala utilizatorului

Reprezintă unitatea de învățământ unde utilizatorul învață/predă.

Din nou, este vizibilă altor persoane în diferite măsuri și în anumite circumstanțe.

## Rolul utilizatorului

Există, evident, două roluri: cel de **elev** și cel de **profesor**. Utilizatorii care nu și-au făcut un cont sunt considerați anonimi, iar cei care nu s-au înregistrat după crearea contului au drepturi restrânse.

### Înregistrarea utilizatorului

După ce își creează contul, utilizatorul este redirecționat spre a se înregistra. Procesul de înregistrare constă în specificarea numelui și școlii sale.

Cum fără aceste date utilizatorul nu poate fi identificat pe paltformă, acesta nu poate să încarce lucrări și să se asocieze cu profesori.

## Asocieri între utilizatori

Elevii și profesorii se pot asocia între ei. În acest mod, elevii pot beneficia de opinia personală a profesorului lor de la clasă și primi o revizuire mai rapidă, mai ales dacă e o lucrare deja verificată la oră de către profesor.

O asociere este compusă din:

- inițiator (elev sau profesor)
- elev
- profesor

Este necesar ca inițiatorul să fie una dintre părți (elevul sau profesorul). După inițierea asocierii, aceasta se află în stadiul de _așteptare_, deoarece inițiatorul așteaptă aprobarea sau respingerea celeilalte părți. Când cealaltă parte răspunde asocierii, stadiul acesteia se schimbă din _așteptare_ în _aprobată_ sau _respinsă_. În primul caz, utilizatorii sunt asociați, iar în al doilea inițiatorul primește o înștiințare în legătură cu asocierea refuzată.

## Confidențialitatea datelor utilizatorului

"Date" se referă la: nume, școală și email.

- utilizatorii anonimi nu obține nicio informație despre elevi.
- datele profesorilor sunt accesibile de către orice persoană.
- profesorii pot accesa datele elevilor, pentru a putea permite inițierea asocierilor de către profesori.
