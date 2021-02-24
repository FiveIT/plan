# Plan \<NUME\>

[Prezentare](prezentare.md) &bull; [Business plan][1] &bull; [Prototip][2] &bull; [Schematică bază de date][3]

**NOTĂ:** Pentru neclarități în legătură cu acest document, deschideți un issue.

## Rute client

<pre>
<a href=#home>/</a>
|-<a href=login>login</a>
|-<a href=register>register</a>
|-<a href=search>search</a>
|-<a href=upload>upload</a>
|-<a href=write-menu>write</a>
| |-<a href=write>[essay]</a>
|-evaluate
| |-<a href=evaluate>[essay]</a>
|-<a href=book>[book]</a>
| |-<a href=essay>[essay]</a>
|-<a href=character-redirect>[character]</a>
  |-<a href=character>[essay]</a>
</pre>

### Home

* pagina de întâmpinare
* **elevul** vede:
  * titlurile de cărți sau personaje ([component](#titlu-de-carte-sau-personaj), [entitate](), [endpoint]()) 
* **profesorul** vede:
  * eseurile nerevizuite ([component](#eseu-nerevizuit), [entitate](), [endpoint]())

#### Frontend

* bazat pe layout-ul **[bază](#layout-base)**
  * **titlu:** `Bun venit!/Acasă/etc.`
  * **slot:**
    * grid din titluri sau eseuri nerevizuite

#### Backend

* serveste index.html și bundle-urile

### Login

[//]: # (TODO)

### Register

[//]: # (TODO)

### Search

[//]: # (TODO)

### Upload

[//]: # (TODO)

### Evaluate

[//]: # (TODO)

### Book

    /[book]
    |-[essay]

[//]: # (TODO)

### Essay

* subrută a [book](#book)

[//]: # (TODO)

[//]: # (TODO: Rutele nou-adaugate + alte rute necesare/utile)

### Write menu

    /
    |-[essay]

* afișează eseurile începute anterior (draft-urile) ([component](#draft))
* permite elevului să înceapă un eseu nou

### Write

* subrută a [write-menu](#write-menu)
* afișează [editorul de text](#editor-text), unde se editează lucrarea identificată de ID-ul [essay]

## Componente

### Titlu de carte sau personaj

* reprezintă un link către ruta [book](#book) sau [character](#character-redirect)
* afișează:
  * titlul/numele personajului
  * autorul/opera din care face parte
  * numărul de eseuri

### Eseu nerevizuit

* reprezintă un link către ruta [evaluate](#evaluate)
* afișează
  * titlul cărții/numele personajului pentru care e făcut eseul
  * autorul cărții/titlul cărții din care face parte
  * tipul lucrării (eseu/caracterizare)

### Vizualizator text

* afișează textul pentru citit

[//]: # (TODO: descriere completă)

### Draft

* este un link către a edita un eseu deja început ([rută](#write))
[//]: # (TODO: Rolul informațiilor afișate este de a ajuta elevul în a recunoaște cu ușurință draft-ul pe care îl caută. Există informații mai utile pentru aceasta?)
* afișează
  * opera/personajul pentru care este scris eseul
  * ultima dată și oră la care a fost editat
  * numărul de cuvinte

## Layout-uri

### <a name=layout-base></a>Bază

* **header:**
  * căutare
  * buton login/înregistrare
  * (dacă utilizatorul este logat) buton setări cont
* separator
* titlul paginii (completat în funcție de rută)
* slot pentru conținutul rutei

## Endpoint-uri API

[//]: # (TODO: GraphQL? Având în vedere că permite alegerea payload-ului necesar pe frontend oferă o flexibilitate mai mare și lipsa necesității de a crea endpoint-uri ca într-un REST API. Totuși, este o tehnologie nefamiliară tuturor.)

[1]: https://docs.google.com/presentation/d/1bKMsCSciHUsiMy7Lg7-0SCBnQGAnBxZ8NDw0_tS32g0/
[2]: https://www.figma.com/file/eNTTW9Hj7KzglbLifcj8Zt/Prototip
[3]: https://dbdiagram.io/d/602fa29efcdcb6230b20958d
