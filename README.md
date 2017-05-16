Drop-Down-Box
===================
Allegro summer e-xperience 2017
Maciej Wójcik

----------

To repozytorium zawiera kod komponentu na zadanie stażowe w allegro summer e-xperience.
Komponent został napisany z użyciem biblioteki do JavaScript’u  Polymer w wersji 2.0.
Komponent jest responsywny i interaktywny.  Wykorzystuje najnowsze technologie do budowy web-components.
Zachęcam do obejrzenia demo komponentu dostępnego na [github-pages.](http://maciejwwojcik.github.io/drop-down-box/)


----------


Instalacja
-------------

Po pierwsze trzeba mieć zainstalowane [npm](https://nodejs.org/en/) , oraz [Polymer CLI](https://www.npmjs.com/package/polymer-cli)

Do instalacji będziemy potrzebować zainstalowanego **GIT**'a na komputerze

Polymer CLI instalujemy wpisując po kolei poniższe komendy:

    npm install npm@latest –g
    npm install -g bower
    npm install -g polymer-cli@next

Istnieją dwie drogi instalacji komponentu.
Można ściągniąć kod źródłowy z githuba, albo zainstalować komponent wpisując w konsole

    bower install MaciejWWojcik/drop-down-box


a następnie wpisując

    bower install

Uruchomienie komponentu następuje poprzez wpisanie w konsole

    polymer-serve

na konsoli pojawi się informacją na jakim adresie i porcie został wystawiony dany komponent.



----------


Sposób użycia
-------------------
**Wszystko jest opisane na** [github-pages](http://maciejwwojcik.github.io/drop-down-box/)

Komponentu używamy jak każdy inny element deklarując go w kodzie html

    <drop-down-box></drop-down-box>

i importując plik drop-down-box.html w nagłówku

**Komponent powinien już działać**

Możemy dodać do niego różne parametry, żeby zmienić jego zachowanie:

 - `is-active` powoduje włączenie na stałe zielonego podkreślenia, które
   normalnie pokazuje, ze został wybrany element z listy

 - `is-wrong` powoduje włączenie na stałe czerwonego podkreślenia, które normalnie
   wyświetla się, gdy walidacja pola jest włączona, a użytkownik nie
   wybrał, żadnego elementu z listy.

 - `is-disable` powoduje zablokowanie elementu.

 - Używając parametru `default=”element`” możemy wybrać domyślny
   wybrany element, który będzie wyświetlony i zwracany nawet jeśli
   użytkownik nic nie zaznaczy.

Oprócz tego, żeby modyfikować zachowanie naszego elementu i jego wygląd możemy korzystać, z funkcji opisanych w API, oraz zmieniając dowolnie style.  Element jest responsywny, można go dopasować do swoich potrzeb.



API
-------------------
Poniżej przedstawiam listę funkcji przygotowanych dla developera.

`setItems(string[])` – zmienia aktualną listę elementów na liście z podaną w argumencie
`getCurrentItem()` – zwraca aktualnie wybrany element z listy
`setDisabled(Boolean)` – ustawia zmienną disabled zgodnie z argumentem funkcji
`enable()` – ustawia zmienną disabled na false
`disable()` – ustawia zmienną disabled na true
`setValidator(Boolean)` – włącza lub wyłącza walidacje pola zgodnie z argumentem funkcji
`setActiveParam(Boolean)` – ustawia wartość zmiennej is-active zgodnie z argumentem
`setWrongParam(Boolean)` - ustawia wartość zmiennej is-wrong zgodnie z argumentem
