<div align="center">
  <img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/logo.png" alt="OSE Bypass" width="128" height="128" />
  <h1 style="margin: 0;">OSE Bypass</h1>
</div>


Hej, jestem [zorin](https://github.com/ZorinOnTop)! <br><br>Wkurza cię internet w szkole czyli od [OSE](https://ose.gov.pl/)? Spoko, nie jesteś sam. Tutaj jest poradnik, oraz jak działa sieć [OSE](https://ose.gov.pl/). To naprawdę nie jest cała filozofia. Zapytasz mnie po co to robię? Z jednego powodu.
<br>**BLOKOWANIE NIESŁUSZNYCH STRON**. Chcesz sobie zagrać w [osu!](https://osu.ppy.sh/) bo masz trochę luzu i możesz robić co chcesz. Wchodzisz na stronę osu!, ale... Jest zablokowana? Przyszykowałem dla was poradnik z tego powodu.

<br>Miłego wchodzenia na strony!

# Jak działa sieć OSE?

[**OSE**](https://ose.gov.pl/) daje dla szkół darmowy internet **100Mb/s** (szkoły mogą dokupić prędkość internetu). Wszystko dofinansowywane z srodków państwa, czyli jest **darmowy**. Ale niestety niektóre strony są zablokowane (jest komunikat OSE lub Polączenie zostało zresetowane.) Na wszystkich komputerach/laptopach szkolnych instaluje się [**OSE Certyfikat**](https://ose.gov.pl/certyfikaty-ose). Lecz nic to nie da, myślicie sobie że usunięcie certyfikatu [OSE](https://ose.gov.pl/) jest niemożliwe bo nie macie hasła Administratora? Faktycznie, nie można usunąć certyfikatu ale czy blokada zostaje jak jest ten certyfikat włączony? Nie.

<br>

[**OSE**](https://ose.gov.pl/) korzysta z własnych DNS Serverów do blokowania stron. Komputer gdy jest podłączony do Internetu, pyta się przez DHCP jaki ma mieć Adres IP itd. Też się pyta o Serwery DNS. Ale jak działa taki serwer DNS? Bardzo prosto. Klient (komputer) wpisuje sobie google.pl. Wtedy Klient pyta się serwera DNS, jaki Adres IP ma google.pl, Wtedy wysyla do klienta Adres IP i tak pokazuje strone. Tutaj jest przykład w wersji obrazkowej.

<img src="https://wiki.dataspace.pl/wp-content/uploads/2019/12/Adnotacja-2019-12-06-190357.png">

A teraz na przykładzie internetu od [**OSE**](https://ose.gov.pl/). Praktycznie to samo lecz nie do końca. Klient wpisuje google.pl, tak samo pyta się serwera DNS jaki adres ip ma google.pl, lecz sprawdza czy google.pl jest zablokowany. Jak domena jest zablokowana to wysyła Adres IP z komunikatem o zablokowanej stronie. A jak nie ma google.pl w zablokowanych, to wysyła adres ip strony google.pl. Tutaj jest komunikat OSE:

<img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/osezablokowane.png">

OSE prawdopodobnie stosuje także protokoły takie jak **ICAP** (Internet Content Adaptation Protocol). Dzięki ICAP możliwe jest:
- Dynamiczne analizowanie treści stron i blokowanie ich na podstawie kategorii (np. "Gry", "Social Media" itp.).
- Skanowanie pobieranych plików pod kątem wirusów.
- Modyfikacja ruchu HTTP w czasie rzeczywistym.


# Jak obejść sieć OSE?

Dobra, koniec gadania. Właśnie co potrzebujecie to:
* Telefon (naładowany może być)
* Internet (z pakietem)

# Dla użytkowników z Laptopem

1. Odepnij kabel Ethernet.
2. Włącz hotspot'a
3. Podłącz się z Hotspot'em.

Tak, to tyle! XD

<img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/ApplicationFrameHost_IevwcSiBGr.png">

# Dla użytkowników z Komputerem

Lepiej tego nie rób. A jak jesteś hardcorem to praktycznie to samo robisz co z Laptopem lecz musisz sprawdzić:

1. Czy jest karta sieciowa (powinno być Wi-Fi w komputerze)

Ale powiesz zorin, co ty gadasz. Wystarczy że się przez panel sterowania wyłączy karte ethernet. Oj byczku nie, potrzebujesz hasła Administratora. Nawet na zdjęciu pokaże:

<img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/explorer_Iq3XLOAyln.png">

# Nie masz internetu, lub nie chcesz ryzykować?
Dziękuje [CodingInMyDream](https://github.com/CodingInMyDream) za kolejny bypass <3

Spokojnie, też znajdzie się na to sposób ([i]problem jest taki, że działa na niektórych stronach, jak crazygames.pl[i]).
Wystarczy wejść na stronę z blokadą OSE, wpisać losowe znaki do strony np. ksdais9sdj (chodzi mi o https://crazygames.pl/ksdais9sdj) i boom. Macie 404? Wystarczy wejść na stronę główną. (Metoda na 404 działa, lecz ze stroną główną niektóre strony).

Link do kolejnego bypassa: https://github.com/ZorinOnTop/ose-bypass/issues/4

# Pare informacji, które mogą być przydatne

Większość szkół posiada [Active Directory](https://pl.wikipedia.org/wiki/Active_Directory), czyli własne użytkowniki. Możesz odpiąć kabel Ethernet i podłączyć się pod swojego hotspota, Tylko kiedy nie ma nauczyciela, tylko nie zapomnij podpiąć znowu kabel ethernet, aby inni uczniowie mogli korzystać z komputera ;)

# Zakończenie

Dziękuje za przeczytanie całego poradnika. Jeżeli nie chce ci się odpalać Hotspot'a, to zostawiam ci programy które są zablokowane.

Chcesz podziękować? Kliknij na gwiazdkę, nic nie kosztuje a motywuje! 🧡
