## Instrukcja używania media query w HTML i CSS

`Media query` to narzędzie w CSS, które pozwala na stosowanie styli w zależności od pewnych warunków, takich jak szerokość ekranu czy rozdzielczość. Jest to kluczowy element responsywnego projektowania stron internetowych.

### 1. Dodawanie viewportu do HTML:

Aby media query działały poprawnie, ważne jest, aby dodać następujący znacznik `meta` w sekcji `<head>` Twojego dokumentu HTML:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

### 2. Wybieranie breakpointów:

"Breakpointy" to punkty, w których styl Twojej strony zostanie dostosowany w reakcji na zmianę szerokości ekranu. Typowe breakpointy to:

- 600px: Smartfony w poziomie i mniejsze tablety w pionie.
- 768px: Większość tabletów w pionie.
- 992px: Komputery stacjonarne i duże tablety w poziomie.
- 1200px: Duże ekrany komputerów stacjonarnych.

*Tip*: Wybieraj breakpointy w oparciu o treść, a nie urządzenia. Sprawdzaj, jak Twoja strona wygląda na różnych szerokościach i ustal breakpointy tam, gdzie widzisz potrzebę dostosowania designu.

### 3. Pisanie kodu CSS z media query:

Podstawowa składnia media query to:

```css
@media (max-width: 600px) {
    /* style dla ekranów o szerokości do 600px */
}
```

Przykład:

```css
/* Styl dla dużej wersji strony */
h1 {
    font-size: 36px;
}

@media (max-width: 600px) {
    /* Styl dla mobilnej wersji strony */
    h1 {
        font-size: 24px;
    }
}
```

W powyższym przykładzie, nagłówek `<h1>` będzie miał rozmiar 36px na ekranach większych niż 600px, ale jego rozmiar zostanie zmniejszony do 24px na ekranach o szerokości 600px lub mniej.

---