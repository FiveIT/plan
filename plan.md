# Plan \<NUME\>

[Prezentare](prezentare.md) &bull; [Business plan][1] &bull; [Schematică bază de date][2]

**NOTĂ:** Pentru neclarități în legătură cu acest document, deschideți un issue.

## Rute client

<pre>
<a href=#home>/</a>
|-<a href=login>login</a>
|-<a href=register>register</a>
|-<a href=search>search</a>
|-<a href=upload>upload</a>
|-evaluate
| |-<a href=evaluate>[id]</a>
|-<a href=book>[book]</a>
  |-<a href=essay>[essay]</a>
</pre>

### Home

* pagina de întâmpinare
* **elevul** vede:
  * titlurile de cărți ([component](), [entitate](), [endpoint]()) 
* **profesorul** vede:
  * eseurile nerevizuite ([component](), [entitate](), [endpoint]())

#### Frontend

* bazat pe layout-ul **[bază](#layout-base)**
  * **titlu:** `Bun venit!/Acasă/etc.`
  * **slot:**
    * grid din titluri sau eseuri nerevizuite

##### Componente

###### Titlu de carte

* reprezintă un link către ruta [book](#book)
* afișează:
  * titlul
  * autorul
  * numărul de eseuri

###### Eseu nerevizuit

* reprezintă un link către ruta [evaluate](#evaluate)
* afișează
  * titlul cărții pentru care e făcut eseul
  * autorul cărții
  * autorul eseului (numele contului de elev)

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

[//]: # (TODO: Alte rute necesare/utile)

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

[//]: # (TODO)

[1]: https://docs.google.com/presentation/d/1bKMsCSciHUsiMy7Lg7-0SCBnQGAnBxZ8NDw0_tS32g0/
[2]: https://dbdiagram.io/d/602fa29efcdcb6230b20958d
