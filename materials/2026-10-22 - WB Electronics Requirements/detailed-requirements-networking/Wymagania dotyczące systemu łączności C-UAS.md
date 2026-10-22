# Wymagania dotyczące systemu łączności C-UAS

|  | Wymagania dotyczące systemu łączności C-UAS | SPEŁNIENIE<br>WYMAGANIA | Wymaganie<br>obligatoryjne |
| --- | --- | --- | --- |
| **I** | **ARCHITEKTURA ŁĄCZY I SIEĆ LOKALNA** |  |  |
| 1. | System łączności musi jednocześnie obsługiwać co najmniej trzy niezależne interfejsy dostępu do sieci zewnętrznej: jeden<br>podstawowy interfejs WAN oraz minimum dwa zapasowe interfejsy komórkowe LTE/5G wykorzystujące odrębne karty<br>SIM. | □ TAK □ NIE |  |
| 2. | W przypadku braku sieci GSM system łączności powinien zapewniać połączenie do sieci Internet za pomocą<br>alternatywnych metod komunikacji – sieć satelitarna, LoRa lub podobne. | □ TAK □ NIE |  |
| 3. | System musi pracować w trybie MultiWAN/Failover, w którym wybór aktywnego łącza jest dokonywany automatycznie na<br>podstawie skonfigurowanego priorytetu oraz wyniku cyklicznych testów dostępności poszczególnych interfejsów. | □ TAK □ NIE |  |
| 4. | System musi pełnić funkcję serwera DHCPv4 dla sieci lokalnej wewnątrz pojazdu i automatycznie przekazywać klientom<br>przewodowym oraz bezprzewodowym co najmniej: adres IPv4, maskę podsieci, adres bramy domyślnej i adresy serwerów<br>DNS. | □ TAK □ NIE |  |
| 5. | System łączności powinien wspierać technologię VLAN lub pokrewną do wydzielenia ruchu zewnętrznego (Internet) oraz<br>ruchu wewnątrz pojazdu. | □ TAK □ NIE |  |
| 6. | Interfejsy komórkowe muszą obsługiwać LTE kategorii co najmniej 6, agregację pasm oraz automatyczne przełączanie<br>kart SIM w przypadku braku sieci, utraty transmisji danych, słabego sygnału albo osiągnięcia limitu danych. | □ TAK □ NIE |  |
| 7. | Administrator musi mieć możliwość konfiguracji podsieci, zakresu puli adresów, czasu dzierżawy, wykluczeń oraz<br>rezerwacji adresów na podstawie adresu MAC, a także podglądu aktywnych dzierżaw DHCP. Konfiguracja musi być<br>zachowana po restarcie systemu. | □ TAK □ NIE |  |
| 8. | Sieć lokalna wewnątrz pojazdu musi być dostępna jednocześnie przez interfejsy Ethernet. | □ TAK □ NIE |  |
| 9. | Sieć lokalna wewnątrz pojazdu musi być dostępna przez Wi‑Fi w pasmach 2,4 GHz i 5 GHz, w trybie punktu dostępowego,<br>z obsługą co najmniej standardu IEEE 802.11ac oraz zabezpieczeń WPA2 i WPA3. Klienci Wi‑Fi muszą uzyskiwać<br>konfigurację IP z lokalnego serwera DHCP i dostęp wyłącznie do usług dopuszczonych regułami bezpieczeństwa. | □ TAK □ NIE |  |
| **II** | **KONFIGURACJA, ZARZĄDZANIE I PREZENTACJA STANU** |  |  |
| 10. | System musi udostępniać szyfrowany interfejs administracyjny HTTPS, wymagający uwierzytelnienia użytkownika.<br>Dostęp administracyjny z sieci zewnętrznych musi być możliwy wyłącznie przez szyfrowany tunel lub bezpieczny system<br>zdalnego zarządzania. | □ TAK □ NIE |  |
| 11. | Uprawniony administrator musi mieć możliwość włączania i wyłączania interfejsów, zmiany ich metryk, konfiguracji celów<br>i interwałów testów, progów uznania łącza za dostępne lub niedostępne oraz definiowania reguł, polityk i kolejności<br>przełączania. | □ TAK □ NIE |  |
| **III** | **CIĄGŁOŚĆ TRANSMISJI I AUTOMATYCZNE PRZEŁĄCZANIE** |  |  |
| 12. | Dostępność każdego łącza musi być weryfikowana cyklicznie na podstawie odpowiedzi z co najmniej dwóch niezależnych<br>adresów IP lub usług DNS. Interwał testu musi być konfigurowalny. | □ TAK □ NIE |  |
| 13. | Po uznaniu aktywnego łącza za niedostępne system musi, bez udziału operatora, skierować ruch przez kolejne dostępne<br>łącze zgodnie z ustalonym priorytetem, w czasie nie dłuższym niż 60 s. Po stabilnym odzyskaniu łącza o wyższym<br>priorytecie system musi automatycznie do niego powrócić. | □ TAK □ NIE |  |
| 14. | Zmiana lub awaria łącza zewnętrznego nie może powodować zatrzymania usług sieci lokalnej, w tym DHCP i DNS, ani<br>utraty konfiguracji. Tunele szyfrowane oraz połączenia aplikacyjne systemu C-UAS muszą być automatycznie ponawiane<br>po zmianie aktywnego łącza i publicznego adresu IP. | □ TAK □ NIE |  |
| **IV** | **BEZPIECZEŃSTWO, MONITOROWANIE I WERYFIKACJA** |  |  |
| 15. | System musi synchronizować czas z serwerem NTP | □ TAK □ NIE |  |
| 16. | System powinien rejestrować zmianę stanu i przełączenie każdego łącza wraz ze znacznikiem czasu. | □ TAK □ NIE |  |
| 17. | System powinien umożliwiać prezentację aktualnego stanu łączna i dostępności do sieci Internet. | □ TAK □ NIE |  |
| 18. | Odbiór systemu musi obejmować udokumentowane testy zaniku i powrotu każdego skonfigurowanego interfejsu WAN,<br>potwierdzające kolejność i czas przełączania, utrzymanie usług sieci lokalnej. | □ TAK □ NIE |  |
