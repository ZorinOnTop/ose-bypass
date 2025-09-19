<div align="center">
  <img src="https://github.com/ZorinOnTop/ose-bypass/blob/main/img/logo.png" alt="OSE Bypass" width="128" height="128" />
  <h1 style="margin: 0;">OSE Bypass</h1>
</div>


Hej, jestem [zorin](https://github.com/ZorinOnTop)! <br><br>Jeśli denerwuje Cię, że w szkole coś jest zablokowane przez OSE, rozumiem. Ten repo zawiera przegląd tego, jak działa sieć OSE i jakie mechanizmy są wykorzystywane do filtrowania treści. To nie jest instrukcja "jak włamać się do systemu", tylko wyjaśnienie działania oraz uwagi o tym, co naprawdę działa, a co to tylko mito.

<br>Miłej edukacji i czytania :D

# Co to jest OSE?

**OSE (Ogólnopolska Sieć Edukacyjna)** dostarcza szkołom łącze o przepustowości podstawowej 100 Mb/s. Usługa jest dofinansowana i w podstawowym wariancie jest bezpłatna dla szkół. Możliwe jest też zamówienie wyższej przepustowości za dodatkową opłatą. Prawdopodobnie, OSE korzystają z łączy Vectry (reszta internetu, która jest hostowana np. na OVH) i Orange (dla stron które są hostowane w Orange), po sprawdzeniu w [IPInfo](https://ipinfo.io/AS204679#block-upstreams).

> [!NOTE]
> Darmowy internet OSE jest dostępny głównie dla nauczycieli, a dla uczniów zwykle tylko w pracowni informatycznej (według mojej szkoły). Jeśli w sieci jest wielu nauczycieli online w tym samym czasie, połączenie może chwilowo się przerywać, a przeglądarka wyświetla komunikat "Połączenie zostało zresetowane". To normalne ograniczenie infrastruktury i nie ma związku z blokowaniem stron.

# Jak OSE filtruje ruch?

OSE stosuje kilka warstw bezpieczeństwa:
- **DNS (serwery NASK)** - wszystkie zapytania w sieci szkolnej trafiają do centralnych serwerów NASK. To one decydują, czy domena jest dostępna, czy przekierowywana na komunikat o blokadzie. DNS to tylko jedna z warstw filtrowania.
- **Centralne proxy / SWG** - ruch WWW (w tym HTTPS) jest często kierowany przez centralne bramy bezpieczeństwa, które analizują adresy URL i zawartość stron.
- **ICAP / integracja skanów** - system może przesyłać treść do skanów antywirusowych i filtrów kategorii, co pozwala na bardziej zaawansowaną analizę i blokowanie treści w czasie rzeczywistym.

# Certyfikaty i HTTPS

Na szkolnych urządzeniach instalowany jest **certyfikat OSE**, aby umożliwić analizę zaszyfrowanego ruchu HTTPS przez systemy bezpieczeństwa.
> [!NOTE]
> Usunięcie certyfikatu nie powoduje "ominięcia filtrów". Wręcz przeciwnie — brak certyfikatu może spowodować problemy z poprawnym przeglądaniem stron.


Metody "obejścia" — co naprawdę działa?
- **Zmiana sieci (np. użycie mobilnego hotspotu)** - jeśli korzystasz z innego łącza niż OSE, filtry nie obowiązują, bo jesteś w innej sieci. To nie jest „hak”, tylko normalna zmiana sieci.
> [!NOTE]
> Jeżeli korzystasz z laptopa, będzie ci łatwiej odłączyć kabel Ethernet. Sieć OSE jest tylko przez Wi-Fi i Ethernet szkolny. W przypadku komputerów, będzie trudnej jeżeli komputer nie ma Karty sieciowej WI-FI oraz dostęp do kabla Ethernet jest utrudniony. Jeżeli twoja szkoła korzysta z [Active Directory (czyli użytkowników zarządzanych przez serwer jako "Inny użytkownik")](https://pl.wikipedia.org/wiki/Active_Directory), to nie należy odpinać kabla Ethernet, bo wtedy nikt się nie zaloguje na komputerze
- **Triki typu "404 → wejście na stronę główną"** *[(credit dla mari-fones)](https://github.com/ZorinOnTop/ose-bypass/issues/4)* — to tylko anegdota. W rzadkich przypadkach może zadziałać, ale nie jest niezawodne ani oficjalne.
- **Zmiany ustawień systemowych / usuwanie certyfikatów** - w większości komputerów szkolnych wymagane są uprawnienia administratora. Próby ingerencji mogą spowodować utratę dostępu do stron.

# Dla użytkowników z Laptopem

1. Możesz użyć mobilnego hotspotu (oczywiście pierw odłączając kabel Ethernet), aby połączyć się z Internetem poza siecią OSE.
2. W tym przypadku filtry OSE nie obowiązują, bo korzystasz z innego łącza.
> To najprostsza i legalna metoda obejścia ograniczeń sieci szkolnej.

# 404 trick (anegdota)
Niektóre osoby opisują metodę polegającą na wpisaniu losowego podadresu strony (np. jczddskl) i następnie wejściu na stronę główną. To może działać w bardzo specyficznych sytuacjach, ale **nie jest niezawodną ani oficjalną metodą**.

# Zakończenie

Dziękuje za przeczytanie całego poradnika. Jeżeli nie chce ci się odpalać Hotspot'a, to zostawiam ci programy które są zablokowane.

Chcesz podziękować? Kliknij na gwiazdkę, nic nie kosztuje a motywuje! 🧡
