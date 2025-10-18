# Auto-Bump Selfbot dla Discord

## Opis Projektu
Ten projekt to automatyczny selfbot do bumpowania serwerów na Discordzie. Selfbot ten pomaga w utrzymaniu wysokiego miejsca w rankingach serwerów poprzez automatyczne wysyłanie komendy `/bump` na wyznaczonym kanale. Jest idealny dla właścicieli serwerów Discord, którzy chcą zwiększyć widoczność swojego serwera bez ręcznego bumpowania.

**Uwaga:** Używanie selfbotów na Discordzie może naruszać Warunki Usługi Discord. Używasz tego na własne ryzyko. Projekt ten jest przeznaczony do celów edukacyjnych i testowych.

## Wymagania Systemowe
- **Node.js** (wersja 16 lub nowsza) – do uruchomienia skryptu JavaScript.
- **npm** – menedżer pakietów Node.js, zazwyczaj instalowany wraz z Node.js.
- Konto Discord z tokenem użytkownika (wymagane do działania selfbota).
- Licencja (wymagana przez projekt).

## Darmowa Licencja
- ```D6Q1M-8X3PL-2R9SZ```

## Instalacja
1. Pobierz wszystkie pliki projektu do jednego folderu (np. `bumptool`).
2. Otwórz terminal (cmd lub PowerShell) w folderze projektu.
3. Uruchom `build.bat`, aby zainstalować wszystkie niezbędne zależności:
   ```
   build.bat
   ```
   To zainstaluje pakiety takie jak `discord.js-selfbot-v13`.

## Konfiguracja
Przed uruchomieniem skonfiguruj plik `config.json` zgodnie z Twoimi potrzebami:

```json
{
  "license": "TWOJA_LICENCJA_TUTAJ",  // Wprowadź swoją licencję (wymaganą przez projekt)
  "token": "TWOJ_TOKEN_DISCORD_TUTAJ",  // Wprowadź swój token użytkownika Discord
  "channelId": "ID_KANALU_BUMP"  // ID kanału, na którym ma być wysyłana komenda /bump
}
```

### Jak uzyskać token Discord?
1. Otwórz Discord w przeglądarce.
2. Otwórz narzędzia deweloperskie (F12).
3. Przejdź do zakładki "Network" i odśwież stronę.
4. Znajdź żądanie i skopiuj token z nagłówków lub lokalnego storage.

### Jak uzyskać ID kanału?
1. Włącz tryb dewelopera w ustawieniach Discord (Użytkownik > Zaawansowane > Tryb dewelopera).
2. Kliknij prawym przyciskiem na kanał i wybierz "Kopiuj ID".

**Ważne:** Nie udostępniaj swojego tokenu nikomu – to klucz do Twojego konta!

## Uruchamianie
1. Upewnij się, że konfiguracja w `config.json` jest poprawna.
2. Uruchom `start.bat`:
   ```
   start.bat
   ```
   To uruchomi selfbota, który zaloguje się na Twoje konto i zacznie bumpować.

Selfbot będzie:
- Automatycznie wysyłać `/bump` co pewien czas (zgodnie z logiką w kodzie).
- Sprawdzać licencję przed uruchomieniem.
- Obsługiwać błędy, takie jak brak komendy slash lub próba użycia komendy tekstowej.

## Struktura Plików
- `index.js` – Główny plik skryptu selfbota (zawiera logikę bumpowania).
- `config.json` – Plik konfiguracyjny (edytuj go przed uruchomieniem).
- `build.bat` – Script instalacyjny (uruchom raz na początku).
- `start.bat` – Script uruchamiający (użyj do startu selfbota).
- `README.md` – Ten plik z instrukcjami.

## Rozwiązywanie Problemów
- **Błąd licencji:** Upewnij się, że licencja w `config.json` jest poprawna. Projekt sprawdza licencję online.
- **Błąd połączenia:** Sprawdź połączenie internetowe i adres serwera licencji w kodzie.
- **Selfbot nie bumpuje:** Sprawdź ID kanału i upewnij się, że masz uprawnienia do wysyłania wiadomości na tym kanale.
- **Błędy Node.js:** Upewnij się, że Node.js jest zainstalowane i dodane do PATH.

## Aktualizacje i Wsparcie
- Projekt może wymagać aktualizacji zależności – uruchom `build.bat` ponownie po zmianach.
- Jeśli napotkasz problemy, sprawdź konsolę po uruchomieniu `start.bat` – wyświetla szczegółowe logi.

Dziękuję za używanie tego projektu! Pamiętaj o odpowiedzialnym używaniu narzędzi Discord.

---

*Autor: IceEgg*
