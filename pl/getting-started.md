---
title: IFG GEO Optimizer
description: Dokumentacja, FAQ i strony prawne aplikacji Shopify IFG GEO Optimizer.
lang: pl
---

# Pierwsze kroki

<div class="lang-switcher">
{% include lang-switcher.html current="pl" slug="getting-started" %}
</div>

IFG GEO Optimizer ma dziewięć sekcji, dostępnych z górnego menu nawigacji po zakończeniu konfiguracji: **Dashboard**, **Audyt katalogu**, **Crawler AI**, **FAQ produktu**, **Link Coach**, **Widoczność AI**, **Cennik**, **Ustawienia** i **Wsparcie**. Ten poradnik przechodzi przez wszystkie z nich, w kolejności, w jakiej zwykle korzystają z nich sprzedawcy.

## 1. Instalacja i ukończenie kreatora konfiguracji

Przy pierwszym otwarciu krótki, prowadzony kreator konfiguracji (około 2 minuty) zbiera podstawowe informacje: język interfejsu, szczegóły polityki zwrotów i wysyłki, dane Twojej firmy oraz — jedyny krok, który ma realne znaczenie techniczne — aktywację osadzenia aplikacji **GEO Schema** w edytorze motywu. Nic, co aplikacja robi później, nie dotrze do Twojego sklepu, dopóki to osadzenie nie zostanie włączone, więc warto go nie pomijać. Każdą z tych odpowiedzi możesz później zmienić w **Ustawieniach**.

## 2. Dashboard

Twoja baza operacyjna. Pokazuje aktualny wynik GEO (z ostatniego audytu), **Macierz gotowości** z ośmioma sygnałami widocznymi na pierwszy rzut oka — możliwość ekstrakcji treści, schemat Organization, `llms.txt`, `agents.md`, dostęp crawlerów, gotowość MCP, połączenie z Link Coach oraz ruch polecany przez AI — a także priorytetową listę „napraw to najpierw" i liczniki wykorzystania Twojego planu (generacje FAQ, wielkość katalogu). Wszystko tutaj prowadzi bezpośrednio do strony, na której możesz podjąć działanie.

## 3. Audyt katalogu

Kliknij **Skanuj ponownie katalog**, aby sprawdzić każdy produkt pod kątem dziewięciu pól danych strukturalnych, których szukają wyszukiwarki: zdjęcie, opis, marka, SKU, GTIN, cena, specyfikacje techniczne, polityka zwrotów i polityka wysyłki. Produkty poniżej 80/100 pokazują dokładnie, czego brakuje.

- **Poprawka jednym kliknięciem**: tam, gdzie aplikacja może bezpiecznie wyprowadzić brakujące dane (zwykle specyfikacje techniczne z istniejących już opcji produktu), zobaczysz przycisk **Napraw**, który zapisuje je bezpośrednio w danych strukturalnych produktu. Nic nie jest zgadywane dla pól, których aplikacja nie może zweryfikować — brakujący kod kreskowy, na przykład, pozostaje brakujący zamiast być wymyślony.
- **Wskaźnik chunkingu treści**: obok kontroli danych strukturalnych każdy produkt otrzymuje osobny wynik ekstrahowalności — nie „czy pole jest obecne", ale „czy system AI/RAG może faktycznie wyciągnąć czysty fakt z tego opisu". Ubogi, przymiotnikowy tekst uzyskuje niższy wynik nawet przy idealnym markupie schema.org.
- **`llms.txt`**: generuje prawdziwy, zgodny ze standardem plik `llms.txt`, podsumowujący Twój katalog dla systemów AI, udostępniany w prawdziwym katalogu głównym Twojego sklepu (`/llms.txt`), a nie ukryty pod ścieżką app proxy, gdzie crawlery go nie znajdą.
- **`agents.md`**: generuje plik opisujący Twój sklep dla autonomicznych agentów zakupowych — warianty, wyszukiwanie, kasę — zbudowany wyłącznie z prawdziwych danych, które Twój sklep już udostępnia, bez niczego zmyślonego.
- **Schemat Organization**: publikuje dane Twojej firmy (nazwa prawna, NIP/numer VAT, adres) jako dane strukturalne, aby silniki AI mogły zweryfikować, że jesteś realną, wiarygodną firmą, zanim Cię polecą.

W planie Free audyty obejmują pierwsze 20 produktów, jednorazowo, bez zachowywania historii. Grow i Unlimited skanują cały katalog i zachowują każdy poprzedni skan do porównania trendów.

## 4. Crawler AI

Wybierz produkt, a aplikacja pobierze jego stronę dokładnie tak, jak robi to crawler AI — bez wykonywania JavaScriptu, tak samo jak GPTBot, ClaudeBot czy PerplexityBot — dzięki czemu widzisz dokładnie to, co jest widoczne dla tych silników: czy Twój `robots.txt` je blokuje (sprawdzane dla każdego bota z osobna, a nie tylko ogólne zezwól/zablokuj), oraz czy Twoje dane strukturalne faktycznie przetrwają w surowym HTML-u odczytywanym przez te boty.

**Porównanie z konkurencją** (osobna zakładka na tej stronie): wklej adres URL produktu konkurenta i otrzymaj te same sygnały GEO zestawione obok siebie z Twoimi — ten sam rodzaj różnicy, jaki dałby ręczny audyt, bez potrzeby rejestracji we własnych narzędziach konkurenta.

## 5. FAQ produktu

W planie Grow lub Unlimited wybierz produkt i kliknij **Generuj FAQ**, aby otrzymać od trzech do pięciu par pytanie-odpowiedź, opracowanych wyłącznie na podstawie prawdziwego tytułu, opisu, dostawcy i specyfikacji tego produktu — model ma wyraźne polecenie, by nigdy nie dodawać szczegółu, którego nie ma już w Twoich danych. Przejrzyj każdą wersję roboczą; nic nie zostanie opublikowane bez Twojego wyraźnego **Zatwierdzenia**. Zatwierdzone FAQ pojawiają się na żywej stronie produktu i są oznaczone jako dane strukturalne `FAQPage`, więc są czytelne zarówno dla ludzi, jak i możliwe do zacytowania przez maszyny.

**Przepisywanie treści** (osobna zakładka na tej stronie): aplikacja może przepisać opis produktu tak, by był gęstszy w weryfikowalne fakty i łatwiejszy do zacytowania przez silnik generatywny — zawsze widzisz porównanie przed/po i zatwierdzasz zmianę, zanim cokolwiek zostanie zapisane w produkcie.

## 6. Link Coach

Analizuje, jak dobrze Twoje produkty są ze sobą powiązane poprzez wspólne kolekcje, dostawców i tagi — linkowanie wewnętrzne to sygnał, którego systemy AI używają, by zrozumieć, co obejmuje cały Twój katalog, a nie tylko pojedynczą stronę. Pokazuje osierocone produkty bez sensownych powiązań oraz zrozumiałe sugestie, jak to naprawić.

## 7. Widoczność AI

Dodaj kilka zapytań, o które realistycznie mógłby zapytać klient asystenta AI (limit zależy od Twojego planu — patrz Cennik poniżej), a co tydzień aplikacja sprawdza, czy Claude, ChatGPT, Gemini i Perplexity wspominają o Twoim sklepie w odpowiedzi, śledząc to w czasie dla każdego silnika osobno. W planach Grow i Unlimited pokazuje to również, jak wypadasz na tle wskazanych konkurentów przy tych samych zapytaniach.

**Ruch polecany przez AI** (Grow i Unlimited): lekki, dbający o prywatność pixel wykrywa, kiedy odwiedziny sklepu faktycznie pochodzą z jednego z tych silników AI (poprzez referrer, tylko po tym, jak odwiedzający wyraził zgodę na analitykę przez baner cookie Twojego sklepu) i raportuje, ile takich odwiedzin miałeś w ostatnich 7 dniach — druga połowa pętli, której samo śledzenie widoczności nie może pokazać: nie tylko „czy jesteśmy wspominani", ale „czy ta wzmianka kogoś do nas wysyła".

## 8. Wsparcie

W aplikacji działa asystent czatu AI (ikona w prawym dolnym rogu) do pytań o GEO, wyniki Twojego audytu lub sposób działania konkretnej funkcji. Jeśli nie potrafi pomóc, możesz poprosić o rozmowę z człowiekiem, a rozmowa zostanie przekazana bezpośrednio do IFG eCommerce.

## 9. Ustawienia

Tutaj zarządzasz odpowiedziami z kreatora konfiguracji (polityki, dane firmy, język interfejsu — przełączaj natychmiast między 30 językami, bez opóźnienia przeładowania), ponownie sprawdzasz aktywację osadzenia motywu i widzisz uprawnienia Shopify przypisane do Twojego konta.

## 10. Cennik

**Cennik** pokazuje plany Free, Grow i Unlimited obok siebie, miesięcznie lub rocznie (rozliczenie roczne to w przybliżeniu 2 miesiące gratis w obu płatnych planach). Możesz w każdej chwili uaktualnić, obniżyć plan lub wrócić do Free bezpośrednio w aplikacji — bez konieczności wysyłania e-maila. Dokładne limity planów znajdziesz w [FAQ](faq.html).

To cała pętla. Większość sprzedawców ponownie uruchamia audyt po dodaniu nowych produktów, sprawdza symulator crawlera za każdym razem, gdy aktualizuje opis, i co tydzień rzuca okiem na Macierz gotowości na Dashboardzie.

[← Powrót do Centrum pomocy](index.html)
