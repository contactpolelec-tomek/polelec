# POLELEC — pakiet strony (gotowe pliki)

Masz tu gotowy folder z prostą stroną dwujęzyczną (PL/FR), szablonami faktury i oferty oraz przykładowymi wpisami na bloga.
Folder: `/mnt/data/polelec_site`

## Co jest w środku (ważne):
- `index.html` — strona główna (PL)
- `fr/index.html` — strona główna (FR)
- `about.html`, `services.html`, `blog.html`, `contact.html`
- `styles.css`, `script.js`
- `assets/images/logo.png` — Twoje logo (jeśli przesłane)
- `invoice.html` — szablon faktury (drukowalny, PDF)
- `devis.html` — szablon oferty (devis)
- `content/posts/pl` i `content/posts/fr` — przykładowe wpisy w markdown
- `admin/config.yml` — konfiguracja Netlify CMS (opcjonalnie)
- `README.md` — ten plik

## Krok po kroku — jak uruchomić stronę na twoim komputerze (najprościej)
1. Rozpakuj ZIP (jeśli pobrałeś ZIP). Otwórz folder `polelec_site` i kliknij `index.html` — strona otworzy się w przeglądarce lokalnie. To podgląd — nikt nie zobaczy jej w internecie dopóki nie wrzucisz na hosting.
2. Aby wystawić stronę publicznie: idź na **Netlify** (netlify.com) i zaloguj się. Możesz użyć darmowego konta.
   - Masz 2 proste opcje:
     - **Drag & drop:** w panelu Netlify -> Sites -> "Add new site" -> "Deploy manually" -> przeciągnij cały folder `polelec_site` (upewnij się, że w folderze jest plik `index.html`).
     - **GitHub:** załóż repozytorium na GitHub, wypchnij pliki, a potem na Netlify wybierz "New site from Git" i połącz repozytorium (Netlify będzie automatycznie budować i publikować).
3. Po wrzuceniu Netlify nada Ci adres typu `two-nazwa.netlify.app`. Jeśli chcesz własną domenę (np. twojafirma.fr), możesz ją podłączyć z panelu Netlify (po zakupie domeny u rejestratora).

## Jak edytować treści (proste)
- Edycja ręczna: otwórz pliki `.html` w Notatniku/VSCode, zmień tekst, zapisz. Potem ponownie wrzuć folder na Netlify (drag&drop) lub zrób commit na GitHub i Netlify automatycznie zaktualizuje stronę.
- Blog (ręcznie): dodaj plik .md w `content/posts/pl` lub `content/posts/fr`. Linki w `blog.html` wskazują na pliki w folderze content (możesz je skonwertować lub zostawić jako linki do źródeł markdown).
- Netlify CMS (opcjonalnie): plik `admin/config.yml` jest przygotowany. Aby uruchomić panel CMS trzeba włączyć w Netlify **Identity** i **Git Gateway** (instrukcja w panelu Netlify). Po skonfigurowaniu dostaniesz GUI do dodawania wpisów bez edycji plików.

## Jak wystawić fakturę / ofertę (szybko)
1. Otwórz `invoice.html` w przeglądarce.
2. Podmień dane klienta, numer faktury i kwoty (edytuj w Notatniku).
3. W przeglądarce: Plik -> Drukuj -> wybierz "Zapisz jako PDF" (Save as PDF). Masz gotowy plik PDF faktury.
Analogicznie z `devis.html` (oferta).

## Propozycje na start (co zrobić teraz)
1. Otwórz folder, sprawdź `index.html`, podmień treści (nagłówek, opis, e-mail jeśli chcesz).
2. Wgraj wszystko na Netlify (drag&drop) żeby strona była dostępna publicznie.
3. Przygotuj 2-3 wpisy na blog i dodaj do `content/posts/pl` żeby Google zaczęło indeksować (proste SEO).

---
Jeśli chcesz, mogę:
- Zrobić deploy za Ciebie (potrzebuję dostęp do konta Netlify/GitHub) — wtedy zrobię commity/ustawienia (jednorazowo, w tej rozmowie).
- Przygotować więcej wpisów na blog (PL+FR).
- Dostosować wygląd (kolory, teksty).

Gotowe pliki są też spakowane w ZIP obok — pobierz i otwórz.
