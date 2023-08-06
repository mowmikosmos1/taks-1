## Instrukcja zakładania konta na GitHubie i klonowania projektu na macOS

### 1. Zakładanie konta na GitHubie:
1. Otwórz przeglądarkę i odwiedź [GitHub](https://github.com/).
2. Kliknij **Sign up**.
3. Wypełnij formularz i kliknij **Create account**.
4. Postępuj zgodnie z instrukcjami na ekranie.

### 2. Instalacja Git za pomocą instalatora:
1. Przejdź na [Git Downloads](https://git-scm.com/downloads).
2. Kliknij **Mac OS X** i pobierz instalator.
3. Otwórz pobrany plik `.dmg` i postępuj zgodnie z instrukcjami.

### 3. Konfiguracja Git:
1. Otwórz **Terminal** (`Cmd + Spacja`, wpisz "Terminal").
2. Wprowadź:

```bash
git config --global user.name "Twoja Nazwa"
git config --global user.email twoj@email.com
```

### 4. Klonowanie repozytorium:
1. Odwiedź stronę projektu na GitHubie.
2. Kliknij **Code** i skopiuj adres URL (opcja HTTPS).
3. Otwórz Terminal, przejdź do odpowiedniej lokalizacji:

```bash
cd ~/Pulpit
```

4. Klonuj repozytorium:

```bash
git clone https://github.com/nazwaUzytkownika/nazwaRepozytorium.git
```


## Instrukcja dodawania commitów i pushowania na GitHub

### 1. Dodawanie zmian do indeksu (staging area):
Aby dodać zmienione pliki do indeksu (staging area), użyj poniższego polecenia:

```bash
git add .
```

*Tip*: Jeżeli chcesz dodać konkretny plik, użyj `git add nazwa_pliku`.

### 2. Tworzenie commita:
Aby utworzyć nowy commit z dodanymi zmianami, użyj poniższego polecenia:

```bash
git commit -m "Krótki, opisowy komunikat dotyczący commita"
```

### 3. Pushowanie zmian na GitHub:
Aby wysłać lokalne commity do zdalnego repozytorium na GitHub, użyj poniższego polecenia:

```bash
git push origin nazwa_branch
```

*Tip*: Jeśli pracujesz na głównej branch, zastąp `nazwa_branch` przez `main` lub `master` w zależności od nazewnictwa w twoim repozytorium.

### Wskazówki dotyczące nazywania commitów:
1. Używaj krótkich, jednolinijkowych komunikatów opisujących zmiany.
2. Zacznij komunikat od czasownika w formie imperatywu (np. "Dodaj", "Popraw", "Usun").
3. Unikaj niejasnych komunikatów typu "Poprawki" lub "Aktualizacja". Zamiast tego opisz, co dokładnie zrobiłeś.

### Ogólne zasady dotyczące commitowania:
1. Commituj często. Nie czekaj, aż uzbiera się dużo zmian – lepiej mieć historię z wieloma małymi commitami.
2. Każdy commit powinien dotyczyć jednego konkretnego zadania lub poprawki. Unikaj mieszania różnych zmian w jednym commicie.
3. Przed pushowaniem upewnij się, że kod działa. Nie pushuj niedokończonych funkcji lub błędów.
4. Regularnie synchronizuj (pull) zmiany z głównym repozytorium, aby być na bieżąco z pracami innych osób.
