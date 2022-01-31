<div style="width: 100%; display: flex; justify-content: center"><img src="./imgs/logo.png" width="200"></div>

# Tworzenie dostępnych stron - WCAG w praktyce

<table>
 <tr>
     <td><img src="./imgs/pills.png" width="60" style="margin: 10px" /></td>
     <td style="text-align: justify;" >Dokument poświęcam zebraniu podstawowoych informacji na temat developmentu z świadomym implementowaniem standardu WCAG.</td>
 </tr>
</table>

## Na dobry początek...

### Co to jest dostępność?

Zapewnienie dostępu do informacji możliwie największej liczbie użytkowników niezależnie od:

<ul style="list-style-type: none;" >
    <li><img src="./imgs/age.png" /> wieku</li>
    <li><img src="./imgs/disability.png" /> niepełnosprawności</li>
    <li><img src="./imgs/pc.png" /> sprzętu</li>
    <li><img src="./imgs/disc.png" /> oprogramowania</li>
</ul>

### Co to jest standard WCAG?

Standard WCAG to zbiór wytycznych odnoszących się do implementacji dostępnych stron WWW oraz dokumentów cyfrowych (np. PDF).

### Dla kogo standard WCAG został stworzony?

Dostępność cyfrowa została stworzona dla wszystkich użytkowników komputerów - nie tylko tych nie w pełni sprawnych.

### Przydatne narzędzia

<img src="./imgs/tools.png" > Podstawowowe:
- NVDA
- WAVE
- HeadingsMap
- Dev tools przeglądarki

<img src="./imgs/toolbox.png" > Dodatkowe:
- ARC Toolkit
- W3C Markup Validation Service
- Color Contrast Analyser

## Filary WCAG

- Postrzegalność
- Funkcjonalność
- Zrozumiałość
- Solidność

## WAI ARIA

### Co to jest ARIA?

Jest to zbiór atrybutów dodawanych do znaczników HTML.

<ul style="list-style-type: none;" >
    <li><img src="./imgs/masks.png" /> Role(s) - mówi czytnikowi, że element jest czymś innym niż wskasuje na to znacznik.</li>
    <li><img src="./imgs/crate.png" /> Prop(s) - określa dodatkowe atrybuty spoza standardu HTML.</li>
    <li><img src="./imgs/rocket.png" /> State(s) - określa aktualny stan elementu.</li>
</ul>

### Roles

- alert - ostrzeżenie
- status - komunikat
- button - przycisk
- checkbox
- dialog - okno dialogowe
- progressbar - pasek postępu
- slider - suwak

<span style="color:yellow; background: black;">Uwaga! Rola nie zastępuje znaczenia semantycznego znacznika. \<button /> =/= \<div role="button"> </span>

### Props

- aria-atomic - który zmieniony tekst odczytać
- aria-controls - który element jest sterowany
- aria-describedby - opisany przez elment(y)
- aria-haspopup - czy jest rozwiajny
- aria-label - etykieta tekstowa
- aria-labelledby - etykieta z elementu
- aria-live - obszar aktywny
- aria-readonly - tylko do odczytu
- aria-required - czy wymagany
- aria-setsize - ilość elementów w zestawie
- aria-posinset - aktualna pozycja w zestawie

### States

Stany mamy dwa - true/false.

- aria-checked - czy zaznaczony
- aria-disabled - czy aktywny
- aria-expanded - czy rozwinięty
- aria-hidden - czy ukryty
- aria-invalid - czy prawidłowy
- aria-pressed - czy wciśnięty
- aria-selected - czy wybrany

Źródła
- https://www.w3.org/
- https://www.flaticon.com/
