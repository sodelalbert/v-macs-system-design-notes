# Propozycja wyposażenia pojazdu

Podczas rozmowy z zespołem wykonującym zabudowę pojazdu w dniu **2025-10-22**
zaproponowano poniższe wyposażenie oraz omówiono możliwości jego integracji
z systemem V-MACS. Oznaczenia **READY** pochodzą z notatek ze spotkania.

## Ogrzewanie powietrzne

Rozważane urządzenia:

- **Eberspächer D4, 4 kW** — wskazany interfejs: CAN.
- **Webasto Air Top 4000** — w notatkach wskazano CAN oraz przewodowe sterowanie
  ręczne ustawieniami i nawiewem. Sposób komunikacji wymaga doprecyzowania.

## Klimatyzacja

- **Urządzenie:** dwufunkcyjny klimatyzator Truma Saphir.
- **Sterowanie:** pilot na podczerwień.
- **Status:** READY.

## Podpory stabilizujące pojazd

- **Urządzenie:** Linnepe Autolift.
- **Sterowanie:** pilot radiowy oraz panel ręczny. Wzmianka „auto” w notatkach
  wymaga doprecyzowania.
- **Złącze panelu:** opisane w notatkach jako „RJ6” — mniejsze złącze typu RJ;
  dokładne oznaczenie wymaga potwierdzenia.
- **Link:** [Linnepe Autolift — oferta na Allegro](https://allegro.pl/produkt/podnosnik-do-kampera-linnepe-autolift-5500kg-4szt-c7cc4c81-3daa-40e9-9425-653d4d038615?offerId=17456251329).

## Czujniki otwarcia drzwi

Do ustalenia pozostaje sposób pozyskiwania informacji o otwarciu drzwi:
oddzielne czujniki lub magistrala CAN pojazdu. Dostępność danych przez CAN
wymaga sprawdzenia.

## Czujniki temperatury

- **Na zewnątrz pojazdu:** czujnik do wyboru.
- **Wewnątrz pojazdu:** do rozważenia gotowe rozwiązanie, np.
  [Sonoff THS01](https://www.mediaexpert.pl/dom/inteligentny-dom/detektory/czujnik-temperatury-i-wilgotnosci-sonoff-ths01).

## Data i godzina

Źródłem daty i godziny ma być system Android.

## Maszt

- **Urządzenie:** Fireco.
- **Sterowanie:** styki zwierne oraz przewodowy pilot sterowany przez CAN.
- **Integracja:** MecMast.
- **Status:** READY.

## Oświetlenie LED

- **Zewnętrzne:** sterowanie przez styki zwierne. **Status: READY.**
- **Wewnętrzne:** oświetlenie ambientowe LED sterowane radiowo (RF).
  Do przygotowania: pilot z kołem wyboru kolorów.

## Monitorowanie akumulatorów

- **System:** Victron.
- **Interfejsy do sprawdzenia:** „RJ6”, VE.Direct, USB.
- **Prezentowane dane:** prąd [A], moc [W] i poziom naładowania akumulatorów [%].
- **Sygnalizacja:** informacja o prawidłowym naładowaniu akumulatorów.
- **Dokumentacja:** do uzupełnienia linki do dokumentacji VE.Direct na stronie producenta.

## Kamery 360°

- **Rejestrator:** NVR.
- **Do uzupełnienia:** szczegóły rozwiązania mają zostać przesłane.

## Sterowanie markizą

- **Sterowanie:** ON/OFF. Podczas otwierania należy przez cały czas przytrzymywać
  przycisk sterujący.
- **Status:** READY.

## Zasilanie i uruchamianie systemu

Zasilanie jest dostępne, gdy pojazd jest uruchomiony. Podczas postoju operator
włącza cały system: sieć, przełączniki sieciowe, dostęp do Internetu oraz V-MACS.
