Nazwa narzędzia: USBWriteBlocker.exe

Wersja: 1.0
Suma kontrolna SHA256: 35E47416F7B8D85AE3B1329DA63B4AC70559EF66FE48BFC995AF14A6ED6164F0
Rozmiar pliku: 19 KB
Napisany pierwotnie w Windows Batch, następnie przepisany do języka C# (w oparciu o .NET Framework 4.x).
Skompilowany do pliku wykonywalnego .exe z nagłówkiem pliku MZ.

Autor: Author: Michał Sołtysik
Cybersecurity Analyst & Consultant | Deep Packet Inspection Analyst | Digital Forensics Examiner | SOC Trainer | CyberWarfare Organizer
Analityk i Konsultant ds. Bezpieczeństwa Cybernetycznego | Analityk Specjalizujący się w Głębokiej Inspekcji Pakietów | Ekspert ds. Kryminalistyki Cyfrowej | Trener SOC (Centrum Operacji Bezpieczeństwa Cybernetycznego) | Organizator Działań w Cyberwojnie
Oficjalna strona: https://michalsoltysik.com/
LinkedIn: https://www.linkedin.com/in/michal-soltysik-ssh-soc/
Treści z zakresu cyberbezpieczeństwa: https://www.youtube.com/playlist?list=PL0RdRWQWldOAAKBqOVEutxKMP-a6CNoLY
Accredible: https://www.credential.net/profile/michalsoltysik/wallet
Credly: https://www.credly.com/users/michal-soltysik
Email: me@michalsoltysik.com

Cel: Zaawansowany write blocker USB (narzędzie uniemożliwiające zapis danych na nośnikach USB w celu ochrony ich oryginalnej zawartości) z funkcją audytowania i modułem edukacyjnym, umożliwiający włączanie, wyłączanie i monitorowanie mechanizmu Write Protection oraz rekomendujący prawidłowe metody akwizycji i zabezpieczania dowodów cyfrowych.
Licencja: Darmowa do użytku osobistego i komercyjnego.

Aplikacja wykonuje następujące funkcje:

(1) uruchamia się jako aplikacja konsolowa wymagająca uprawnień administratora, aby mogła wykonywać operacje na poziomie systemowym;
(2) prezentuje komunikaty w konsoli w formie kolorowej: zielony dla informacji standardowych, czerwony dla ostrzeżeń i dobrych praktyk, niebieski dla statusów i komunikatów systemowych;
(3) wyświetla kolejne ekrany edukacyjne opisujące trzy podstawowe metody akwizycji danych: cold (na wyłączonym systemie), live (na działającym systemie) oraz logical (logiczna, obejmująca wybrane pliki/partycje); dodatkowo prezentuje najlepsze praktyki postępowania z dowodami cyfrowymi oraz standardy i wytyczne RFC 3227 i ISO/IEC 27037:2012 dotyczące obsługi dowodów cyfrowych i zachowania łańcucha dowodowego;
(4) pobiera listę wszystkich wolumenów w systemie za pomocą WMI (Windows Management Instrumentation) i prezentuje szczegółowe informacje: litera dysku, typ (Removable - nośnik wymienny, Fixed - dysk stały, Network - dysk sieciowy, CDROM - napęd CD/DVD, RAMDisk - dysk RAM), system plików, etykieta woluminu, rozmiar i wolna przestrzeń w gigabajtach;
(5) umożliwia zarządzanie mechanizmem Write Protection dla urządzeń USB - jest to funkcja systemu Windows, która blokuje możliwość zapisu danych na podłączonych nośnikach USB i pozwala chronić ich oryginalną zawartość przed modyfikacją; użytkownik może włączyć, wyłączyć lub sprawdzić aktualny status tego mechanizmu;
(6) wymusza zapis logów działań na wskazanym nośniku USB - log zawiera datę i godzinę utworzenia, wszystkie akcje użytkownika (włączenie lub wyłączenie ochrony, sprawdzenie statusu) oraz bieżące znaczniki czasu; plik logu otrzymuje nazwę w formacie usb_write_blocker_log_RRRR-MM-DD_GG-MM.txt, np. usb_write_blocker_log_2025-09-07_18-15.txt;
(7) informuje użytkownika, że zmiany w ochronie zapisu obowiązują jedynie dla nowo podłączonych urządzeń USB, natomiast już podłączone nie są objęte działaniem;
(8) zapewnia bezpieczne zakończenie działania - wyświetla podsumowanie, potwierdzenie zapisania logu, umożliwia decyzję o wyjściu i kończy pracę z 20-sekundowym odliczaniem.