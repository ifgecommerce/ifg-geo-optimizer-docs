---
title: IFG GEO Optimizer
description: Dokumentacja, FAQ i strony prawne aplikacji Shopify IFG GEO Optimizer.
lang: pl
---

# Polityka prywatności

<div class="lang-switcher">
{% include lang-switcher.html current="pl" slug="privacy" %}
</div>

**IFG GEO Optimizer** — aplikacja Shopify do Generative Engine Optimization
Ostatnia aktualizacja: lipiec 2026

## 1. Administrator danych

Administratorem danych osobowych przetwarzanych za pośrednictwem **IFG GEO Optimizer** jest:

**IFG eCommerce** — z siedzibą w Rzymie, we Włoszech
E-mail: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Jakie dane zbieramy

- **Dane konta sprzedawcy (poprzez OAuth Shopify)**: domena Twojego sklepu, token dostępu API oraz adres e-mail przypisany do Twojego konta Shopify.
- **Dane katalogu (tylko do odczytu)**: tytuły produktów, opisy, dostawca, ceny, opcje i specyfikacje techniczne — wykorzystywane do przeprowadzania audytów, symulowania zachowania crawlerów, oceny ekstrahowalności treści oraz tworzenia FAQ lub przepisanych opisów.
- **Konfiguracja sklepu**: Twój aktywny plan, szczegóły polityki zwrotów i wysyłki oraz dane firmy wprowadzone w Ustawieniach, zapisane audyty, wersje robocze FAQ i przepisanych treści oraz zapytania, które wybierasz do monitorowania widoczności AI.
- **Wiadomości czatu wsparcia**: tekst, którym wymieniasz się z wbudowanym asystentem AI, w tym transkrypcja przekazywana nam, gdy wyraźnie poprosisz o rozmowę z człowiekiem.
- **Anonimowy ruch sklepu (Web Pixel, Grow/Unlimited)**: gdy odwiedzający trafia na stronę produktu z rozpoznanego silnika AI (ChatGPT, Perplexity, Claude, Gemini, Copilot), zapisujemy silnik, adres URL strony i znacznik czasu — wyłącznie wtedy, gdy odwiedzający wyraził już zgodę na analitykę przez baner cookie Twojego sklepu. Nie zbieramy żadnego identyfikatora odwiedzającego, ciasteczka ani danych sesji.
- **Dane techniczne**: znaczniki czasu żądań, wewnętrzne identyfikatory rekordów oraz logi systemowe.

> Aplikacja **nigdy nie prosi o dane osobowe klientów końcowych ani ich nie otrzymuje** — żadnych nazwisk, adresów e-mail, adresów zamieszkania ani zamówień. Żądane uprawnienia Shopify to `read_products`, `write_products` (katalog i dane strukturalne), `read_themes` (sprawdzanie, czy osadzenie motywu jest aktywne) oraz `write_pixels` (aktywacja powyższego anonimowego pixela ruchu).

## 3. Dlaczego przetwarzamy te dane i na jakiej podstawie prawnej

Przetwarzamy te dane, aby świadczyć usługę, dla której zainstalowałeś aplikację — na podstawie art. 6 ust. 1 lit. b) RODO, wykonania umowy: analizowanie i poprawianie widoczności Twojego katalogu w generatywnych wyszukiwarkach, w tym wspomagane przez AI tworzenie FAQ i przepisywanie treści, czat wsparcia w aplikacji, cotygodniowe śledzenie widoczności AI dla wybranych przez Ciebie zapytań oraz anonimowy pomiar ruchu polecanego przez AI — wszystko zainicjowane albo przez sprzedawcę, albo, w przypadku pixela ruchu, uwarunkowane zgodą na Twoim storefroncie.

## 4. Jak zbieramy te dane

Dane konta są zbierane jednorazowo, poprzez proces OAuth Shopify, przy instalacji. Dane katalogu są odczytywane przez Admin API Shopify wyłącznie wtedy, gdy inicjujesz działanie z poziomu dashboardu. Pixel ruchu działa na Twoim storefroncie i raportuje zdarzenia wyłącznie po uzyskaniu zgody; nic innego nie działa w tle bez Twojej inicjatywy.

## 5. Komu udostępniamy dane

- **Google Firebase / Cloud Firestore** — przechowuje Twoją konfigurację, sesje i wersje robocze. Google LLC (USA) uczestniczy w ramach EU-US Data Privacy Framework. Dane są przechowywane w regionie europe-west1 (Belgia).
- **Anthropic PBC (USA)** — dostarcza model Claude wykorzystywany do tworzenia FAQ, przepisywania treści oraz czatu wsparcia w aplikacji, wyłącznie na Twoje wyraźne działanie. Otrzymuje tylko atrybuty produktu lub tekst czatu, które podajesz — nigdy dane klientów.
- **OpenAI, Inc. (USA)** oraz **Perplexity AI, Inc. (USA)** — wykorzystywane wyłącznie do cotygodniowego śledzenia widoczności AI dla zapytań, które wyraźnie wybierasz do monitorowania. Otrzymują wyłącznie tekst monitorowanego zapytania — nigdy dane klientów.
- **Google LLC (USA)** — dostarcza model Gemini, wykorzystywany w ten sam sposób co OpenAI/Perplexity powyżej, do śledzenia widoczności (odrębne zastosowanie od Firebase/Firestore, które służy wyłącznie do przechowywania danych).
- **Resend, Inc. (USA)** — wysyła nam powiadomienie z nazwą sklepu i transkrypcją czatu wsparcia, wyłącznie gdy wyraźnie poprosisz o rozmowę z człowiekiem w czacie wsparcia.
- **Shopify Inc.** — sama platforma oraz źródło infrastruktury Admin API i Web Pixel, z których korzysta aplikacja.

Nie sprzedajemy danych i nie wykorzystujemy ich do marketingu ani profilowania behawioralnego.

## 6. Jak długo przechowujemy dane

- **Tokeny sesji**: zarządzane przez cykl życia tokenów offline Shopify, rotowane automatycznie.
- **Konfiguracja, audyty, wersje robocze i zdarzenia ruchu**: przechowywane przez cały okres, w którym aplikacja jest zainstalowana. Odinstalowanie uruchamia webhook `shop/redact` Shopify, który całkowicie usuwa konfigurację i sesje Twojego sklepu.
- **Logi techniczne**: przechowywane zgodnie ze standardowym okresem retencji logów Google Cloud.

## 7. Twoje prawa

Na podstawie art. 15–22 RODO możesz zażądać dostępu do swoich danych, sprostowania nieprawidłowych danych lub ich usunięcia — najprostszym sposobem jest odinstalowanie aplikacji — lub wnieść sprzeciw wobec przetwarzania. Możesz też złożyć skargę do lokalnego organu ochrony danych osobowych. Ponieważ aplikacja nigdy nie przetwarza danych osobowych klientów końcowych, webhooki zgodności `customers/data_request` i `customers/redact` odpowiadają, potwierdzając, że nie ma nic do wyeksportowania ani usunięcia.

## 8. Bezpieczeństwo

Cały ruch odbywa się przez HTTPS/TLS 1.2+. Tokeny uwierzytelniające Shopify nigdy nie są ujawniane przeglądarce. Każdy webhook jest weryfikowany kontrolą HMAC SHA-256 w czasie stałym, zanim zostanie przetworzony. Baza danych jest dostępna wyłącznie z backendu, uwierzytelnianego poprzez własną tożsamość usługi platformy hostingowej — w kodzie nie ma statycznych poświadczeń, a bezpośredni dostęp klienta jest odrzucany przez własne reguły bezpieczeństwa bazy danych. Dane są szyfrowane zarówno w spoczynku, jak i w trakcie przesyłania.

## 9. Zmiany

Możemy od czasu do czasu aktualizować niniejszą politykę. Istotne zmiany zostaną odzwierciedlone tutaj, wraz z aktualną datą u góry strony.

---

**Masz pytania dotyczące swoich danych?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Powrót do Centrum pomocy](index.html)
