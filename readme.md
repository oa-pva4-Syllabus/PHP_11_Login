# PVA4 - Programování a vývoj aplikací
## Lekce 11: Přihlášení uživatele

Dnes doplníme do své existující aplikace funkci přihlášení uživatele a zabezpečenou stránku.

1. Vytvoř si pomocný formulář, který ti bude generovat zabezpečené (hashované) heslo
    - zvol si vlastní bezpečnostní algoritmus

2. Vytvoř si v konfiguračním souboru pole `users` s min 3 uživateli, kteří budou mít povolené přihlášení do aplikace.
    - Evidované údaje o uživateli jsou `email`, `jméno`, `příjmení`, `id uživatele`, `telefon`

4. Vytvoř přihlašovací formulář `login.php`
    - Formulář pro zadání uživatelského jméno a hesla.
    - Odesílá se na stránku pro zpracování přihlášení.
    - Stránka přijímá parametry error a zobrazí zprávu uživateli při neplatném přihlášení

4. Zpracuj přihlášení `loginService`
    - Ověř heslo uživatele.
    - Při úspěchu
      -  vytvoř session
      -  přesměruj na stránku `dashboard`
    - Při neúspěchu
      -  vrať na login s chybovou hláškou uživateli.

5. Dashboard
    - Zobraz informace o přihlášeném uživateli.
    - Vytvoř tlačítko na odhlášení.
    - Zkontroluj, že se na stránku nedostane nepřihlášený uživatel.

6. Odhlášení
    - Zpracuj akci odhlášení.
    - Zajisti zrušení session.
    - Uživatel bude přesměrován na přihlašovací stránku.

7. Rozšiř chráněný obsah
   - Přidej ochranu i na další stránku aplikace.
