# Codex Allegro ToTenSklep

Wewnętrzna integracja właściciela, używana do obsługi jego własnych kont Allegro.
Nie jest usługą oferowaną innym sprzedawcom.

## Funkcje

- Odczyt ofert i uzupełnianie ich parametrów na wyraźne polecenie właściciela.
- Wspólna obsługa Centrum wiadomości, dyskusji i reklamacji z oznaczeniem konta.
- Odczyt informacji o zamówieniach oraz ustawieniach sprzedaży.
- Przygotowywanie propozycji odpowiedzi, które wymagają zatwierdzenia.

Zapisy wymagają konkretnego zlecenia właściciela. Integracja sprawdza ID konta,
treść operacji i uprawnienia, prowadzi audyt oraz zapobiega ponownemu wykonaniu
tego samego zlecenia. Same testy połączenia nie wysyłają wiadomości ani nie
zmieniają ofert i zamówień.

## Połączenie i dane

Połączenie korzysta z OAuth 2.0 Authorization Code. Właściciel loguje się i
zatwierdza dostęp na stronie Allegro. Hasła do kont Allegro nie są przechowywane
przez integrację. Tokeny pozostają w centralnym, zaszyfrowanym magazynie, poza
repozytorium kodu i interfejsami projektów korzystających z integracji.

Odczyt profilu służy potwierdzeniu ID konta przed zapisem. Dane kont i wiadomości
są przetwarzane na potrzeby własnej obsługi sprzedaży i nie są publikowane na tej
stronie. Aplikacja nie wymaga zgód do płatności, One Fulfillment ani edycji profilu
do opisanych funkcji.

## Identyfikator i kontakt

Nazwa zarejestrowanej aplikacji: **Codex Allegro ToTenSklep**.

Identyfikator HTTP:
`Codex-Allegro-ToTenSklep/1.0.0 (+https://github.com/Kamillobumbum/allegro-app-info)`

Kontakt techniczny z właścicielem:
[zgłoszenia w repozytorium opisu aplikacji](https://github.com/Kamillobumbum/allegro-app-info/issues).
