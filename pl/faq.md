---
title: IFG GEO Optimizer
description: Dokumentacja, FAQ i strony prawne aplikacji Shopify IFG GEO Optimizer.
lang: pl
---

# Najczęściej zadawane pytania

<div class="lang-switcher">
{% include lang-switcher.html current="pl" slug="faq" %}
</div>

**Jaka jest różnica między GEO a SEO?**
Tradycyjne SEO optymalizuje pod wyszukiwarki, które rankingują i wyświetlają listy linków. GEO (Generative Engine Optimization) optymalizuje pod systemy AI, które czytają Twoje treści i generują odpowiedź lub rekomendację bezpośrednio — ChatGPT, Perplexity, Gemini, Claude i Google AI Overviews. Te dwie dyscypliny się pokrywają, ale GEO zajmuje się rzeczami, których klasyczne narzędzia SEO nie sprawdzają: czy strona produktu ma kompletne dane strukturalne, czy crawler AI faktycznie potrafi odczytać Twoją treść bez wykonywania JavaScriptu, oraz czy Twój tekst jest napisany w sposób łatwy do zacytowania.

**Czy aplikacja ma kiedykolwiek dostęp do danych moich klientów?**
Nie, żadne dane osobowe klientów. Uprawnienia Shopify aplikacji to `read_products`, `write_products`, `read_themes` i `write_pixels` — odczyt i ulepszanie katalogu, sprawdzanie, czy osadzenie motywu jest aktywne, oraz aktywacja anonimowego pixela ruchu sklepu (patrz niżej). Aplikacja nigdy nie prosi o zamówienia ani dane klientów. Pełny opis znajdziesz w [Polityce prywatności](privacy.html).

**Czym jest pixel ruchu polecanego przez AI i czy śledzi moich klientów?**
W planach Grow i Unlimited niewielki Web Pixel wykrywa, kiedy odwiedziny sklepu pochodzą ze znanego silnika AI (poprzez referrer przeglądarki) i raportuje silnik, stronę oraz znacznik czasu — nic, co identyfikowałoby odwiedzającego, żadnych ciasteczek, żadnych danych sesji. Działa wyłącznie wtedy, gdy odwiedzający wyraził już zgodę na analitykę przez baner cookie Twojego sklepu (Customer Privacy API Shopify). Służy do wyświetlania kafelka na Dashboardzie („Ruch polecany przez AI, ostatnie 7 dni") — uzupełnienie śledzenia Widoczności AI, które mówi, czy jesteś wspominany, ale nie mówi, czy ta wzmianka kogoś do Ciebie wysyła.

**Co dokładnie zmienia przycisk „Napraw" w audycie katalogu?**
Zapisuje brakujące dane strukturalne schema.org w metapolu produktu — na przykład specyfikacje techniczne wyprowadzone z istniejących już opcji produktu. Nigdy nie dotyka tytułu, opisu, zdjęć ani ceny produktu i nigdy nie wymyśla danych, których nie może zweryfikować: brakujący kod kreskowy, na przykład, pozostaje brakujący zamiast być zgadywany.

**Czy odpowiedzi FAQ i przepisane opisy są wymyślane przez AI, czy oparte na moim rzeczywistym produkcie?**
Model widzi wyłącznie dane produktu, które już posiadasz — tytuł, opis, dostawcę i specyfikacje techniczne — i ma wyraźne polecenie, by nie dodawać niczego, czego nie ma w tych danych. Przeglądasz każde FAQ lub przepisany opis, zanim zostanie opublikowany; nic nie trafia na stronę automatycznie.

**Co dzieje się z moimi danymi, jeśli odinstaluję aplikację?**
Konfiguracja Twojego sklepu, zapisane audyty, wersje robocze FAQ i przepisanych treści, monitorowane zapytania widoczności oraz zdarzenia ruchu polecanego przez AI są automatycznie usuwane, gdy Shopify powiadomi nas o odinstalowaniu. Aplikacja nie zatrzymuje niczego po Twoim odejściu.

**Czy mogę anulować lub obniżyć plan bez kontaktu z pomocą techniczną?**
Tak. Wejdź w **Cennik** wewnątrz aplikacji i przełącz się na Free w dowolnym momencie — działa to natychmiast, bez konieczności wysyłania e-maila.

## Limity planów

| Funkcja | Free | Grow | Unlimited |
|---|---|---|---|
| Audyt katalogu | Pierwsze 20 produktów, jednorazowo, bez historii | Cały katalog + historia | Cały katalog + historia |
| Symulator crawlera | 20/miesiąc | 300/miesiąc | 1000/miesiąc |
| Porównanie z konkurencją | 10/miesiąc | 50/miesiąc | 150/miesiąc |
| Generowanie FAQ | Niedostępne | 500/miesiąc | 500/miesiąc |
| Przepisywanie treści | Niedostępne | 300/miesiąc | 300/miesiąc |
| Widoczność AI (monitorowane zapytania) | Niedostępne | 5 zapytań | 15 zapytań |
| Pixel ruchu polecanego przez AI | Niedostępne | Wliczone | Wliczone |
| Czat wsparcia AI | 1000 wiadomości/miesiąc | 1000 wiadomości/miesiąc | 1000 wiadomości/miesiąc |
| Języki interfejsu | Wszystkie 30 | Wszystkie 30 | Wszystkie 30 |

Cena miesięczna: Free 0 USD, Grow 9,99 USD, Unlimited 19,99 USD. Rozliczenie roczne w planach Grow/Unlimited to w przybliżeniu dwa miesiące gratis w porównaniu z płatnością miesięczną.

**Dlaczego plan Free obejmuje tylko 20 produktów?**
Ma to pozwolić Ci zobaczyć realne wyniki na Twoim własnym katalogu, zanim zdecydujesz się na płatny plan. Grow i Unlimited znoszą ten limit i zachowują pełną historię wcześniejszych audytów.

**Czy naprawdę istnieje limit generowania FAQ nawet w planie Unlimited?**
Tak — 500 generacji miesięcznie, celowo, nawet w najwyższym planie. Dzięki temu funkcja pozostaje opłacalna przy obecnej cenie; jeśli masz katalog o dużej skali i potrzebujesz więcej, skontaktuj się z nami, a znajdziemy rozwiązanie.

**Dlaczego czat wsparcia AI jest taki sam w każdym planie?**
To decyzja produktowa, nie przeoczenie: wsparcie jest wliczone dla wszystkich, nigdy nie jest elementem różnicującym płatne plany. Limit wiadomości (1000/miesiąc) istnieje wyłącznie jako techniczne zabezpieczenie przed nadużyciami, a nie jako realne ograniczenie — żadne uzasadnione użycie nawet się do niego nie zbliża.

**Znalazłem błąd albo coś wygląda nie tak. Komu to zgłosić?**
Napisz na [info@ifgecommerce.com](mailto:info@ifgecommerce.com), opisując co zobaczyłeś oraz, jeśli to możliwe, którego produktu lub strony to dotyczy — zwykle to wystarczy, by szybko namierzyć problem. Możesz też skorzystać z czatu wsparcia AI w aplikacji i poprosić o rozmowę z człowiekiem.

[← Powrót do Centrum pomocy](index.html)
