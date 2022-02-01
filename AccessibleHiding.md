# Sposoby na ukrywanie elementów ze strony

## Ukrycie całkowite
 Tradycyjna forma ukrycia elementów przy użyciu CSS:
- `display: none;`
- `visibility: hidden;`

## Ukrycie 'dostępne'

Ukrycie to pozwoli na zniknięcie elementu z ekranu, a będące nadal dostępne dla czytników ekranu.
- ustawienie rozmiaru elementu na `0`,
- odpowiednie pozycjonowanie elementu poza ekranem (`left: -1000px; top: -1000px;`),
- zastosowanie wcięcia poza ekran (`text-indent: -1000em;`),
- ukrycie za pomocą `clip: rect(0px,-1000px,200px,0px);` i `position: absolute;`

### Boostrap:
```css
.sr-only {
      position: absolute;
      width: 1px;
      height: 1px;
      padding: 0;
      margin: -1px;
      overflow: hidden;
      clip: rect(0, 0, 0, 0);
      white-space: nowrap; /* added line */
      border: 0;
}
```

### Implementacja

```html
<span class="sr-only">Hide me from the screen</span>
```

### Najczęstsze wykorzystanie:
- przyciski


## Ukrycie dla czytników ekranu

Zastosowanie powyższego ukrycia pozwoli na ukrycie elementu dla czytników ekranu.

### Najczęstsze elementy potrzebującego tego zabiegu:
- ikony,
- tworzenie komponentów tj. `pokaż więcej`/`ukryj`, `checkbox'y`, `radiolista`,
- obrazy.

### Implementacja

```html
<span aria-hidden="true">Hide me for Screen Readers</span>
```
