# GymTracker

Aplikacja mobilna GymTracker — prosta aplikacja do śledzenia treningów siłowych i postępów.

Opis
--
GymTracker pomaga rejestrować ćwiczenia, serie, powtórzenia i ciężary, dzięki czemu możesz śledzić swoje postępy i planować treningi.

Najważniejsze funkcje
--
- Tworzenie i edycja planów treningowych
- Rejestrowanie serii, powtórzeń i ciężarów
- Historia treningów i podsumowania postępów
- Proste, czytelne UI (Android)
- Możliwość eksportu/backupów (jeśli zaimplementowane)

Wymagania
--
- Java (kod źródłowy w Javie)
- Android Studio (zalecane najnowsze wydanie)
- Android SDK (min. API poziom zgodny z projektem)
- JDK 11 lub nowsze (zgodnie z konfiguracją Gradle w projekcie)
- Gradle (projekt zawiera wrapper — ./gradlew)

Instalacja (lokalnie)
--
1. Sklonuj repozytorium:
   git clone https://github.com/kacperszczudlo/gymtracker.git
2. Otwórz projekt w Android Studio:
   - File → Open → wybierz folder projektu
3. Pozwól Android Studio pobrać zależności i zbudować projekt.
4. Uruchom na emulatorze lub urządzeniu fizycznym.

Budowanie z linii poleceń
--
- Przy pierwszym uruchomieniu:
  ./gradlew clean
- Zbudowanie debug APK:
  ./gradlew assembleDebug
- Uruchom testy jednostkowe:
  ./gradlew test

Uruchamianie
--
- W Android Studio: Run → wybierz konfigurację i kliknij Run.
- Z linii poleceń możesz użyć adb do instalacji:
  adb install -r app/build/outputs/apk/debug/app-debug.apk

Architektura projektu
--
Projekt napisany jest w Javie i powinien być zorganizowany w typowe warstwy:
- UI (Activities / Fragments)
- Warstwa danych (baza danych, repozytoria)
- Logika aplikacji (usługi / ViewModels / kontrolery)
Dokumentacja struktury kodu i konwencji znajdzie się w katalogu docs/ jeśli zostanie dodana.

Dodawanie zrzutów ekranu
--
Umieszczaj zrzuty ekranu w katalogu `screenshots/` w repozytorium i referuj je w README, np:
- screenshots/screen1.png
- screenshots/screen2.png

Kontrybuowanie
--
Dzięki za zainteresowanie! Jeśli chcesz kontrybuować:
1. Forkuj repozytorium.
2. Stwórz branch: `git checkout -b feature/nazwa-funkcji`
3. Dodaj testy, jeśli to możliwe.
4. Zrób PR opisując zmiany i powód (opisuj kontekst, przykłady użycia).
5. Zachowuj konwencję kodu — Java, czytelne nazwy, krótkie metody.

Zgłaszanie błędów i propozycje
--
- Użyj Issues na GitHubie: https://github.com/kacperszczudlo/gymtracker/issues
- W zgłoszeniu podaj kroki reprodukcji, oczekiwane i rzeczywiste zachowanie oraz logi/stacktrace jeśli dostępne.

Plan rozwoju (pomysły)
--
- Synchronizacja z chmurą / konto użytkownika
- Eksport i import planów treningowych (CSV/JSON)
- Wykresy postępów
- Integracja z WearOS / urządzeniami fitness

Licencja
--
Domyślnie brak pliku LICENSE w repo — dodaj plik LICENSE z licencją, którą chcesz użyć (MIT, Apache-2.0 itp.). Jeśli chcesz, mogę dodać przykładową licencję.

Kontakt
--
Autor repozytorium: @kacperszczudlo  
E-mail / dodatkowe informacje: dodaj w pliku CONTRIBUTING.md lub w profilu GitHub.

Uwagi końcowe
--
Jeżeli chcesz, mogę:
- Dopasować README do konkretnych elementów projektu (np. dodać przykładowe komendy DB, fragmenty konfiguracji Gradle, konkretne minimalne API),
- Dodać plik LICENSE (np. MIT) i podstawowy CONTRIBUTING.md,
- Wygenerować przykładowe zrzuty ekranu / grafikę README.
