# Problemy z Crystal Launcherem

Obecnie (na dzień 13.11.2025) Crystal Launcher pokazuje komunikat o wpisaniu klucza weryfikacyjnego z powodu wrzucania launchera na inne strony.
<br>
<img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/javaw_v1tHAUSSjh.png"/>

# Jak rozwiązać problem? (na komputerze)

1. Wejdź na [oficjalną stronę Crystal Launchera](https://crystal-launcher.pl/)
2. Skopiuj klucz weryfikacyjny (i przeklikaj ukryte reklamy)
3. Wklej klucz weryfikacyjny do launchera.
Jednak gdy OSE blokuje stronę Crystal Launchera, przewiń dalej.

# Jak rozwiązać problem? (na telefonie)
1. Wejdź na [oficjalną stronę Crystal Launchera](https://crystal-launcher.pl/)
2. Przepisz klucz weryfikacyjny z telefonu.
3. Przepisz klucz weryfikacyjny do komputera.

Jednak gdy OSE blokuje serwery weryfikacyjne Crystal Launchera, przewiń dalej.

# Jak rozwiązać problem? (bez wchodzenia na strone)
1. Kliknij klawisze Windows + R (lub prawy przycisk na logo Windowsa i wybierz "Uruchom")
2. Gdy pojawi ci się okienko pod tytułem "Uruchom", wklej lub przepisz to:
```
%appdata%\Crystal-Launcher
```

4. Gdy pojawi ci się okienko z plikami Crystal Launcher, otwórz plik **config.prop**. Usuń wszystko z pliku i wklej to:
```
#configuration-data
#Thu Nov 13 14:48:24 CET 2025
launch.count=1
autotuner.set=true
launcher.verified=true
crystal.modcacheversion=2
memory.min=1024
memory.max=2048
user.banned=false
first_run=false
```
5. Zapisz plik i uruchom ponownie launchera!
