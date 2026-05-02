# Note — Design sito, SEO locale, Mobile first, Pronto intervento

Riferimento per **Idraulico Sarti** (Torino). Da aggiornare quando cambiano servizi, prezzi o dominio.

---

## 1. Design sito

- **Gerarchia**: sopra la piega — messaggio di urgenza + area (Torino) + **due CTA chiari** (Chiama / WhatsApp). Niente paragrafi lunghi prima del contatto.
- **Contrasto**: CTA ad alto contrasto su sfondo scuro (es. giallo/arancio o verde WhatsApp su blu/grigio scuro). Testo corpo sempre leggibile (grigio scuro su bianco, non grigio chiaro su bianco).
- **Fiducia**: badge brevi (H24, zona, esperienza), **icone o emoji con parsimonia** per non sembrare spam.
- **Brand**: stesso nome, stesso numero, stesso tono in header, footer, barra fissa e (se presente) Google Business.
- **Legale**: Privacy, Cookie, Termini su **pagine dedicate**; in home solo banner cookie all’ingresso + link in footer.
- **Mappa**: iframe responsive, bordo visibile; non spingere le CTA troppo in basso su mobile.
- **Coerenza**: stessi margini, stessi raggi di bordo (border-radius), stessa palette in tutte le pagine (anche legali).

---

## 2. SEO locale (Torino)

- **Parole chiave intent**: idraulico urgente Torino, pronto intervento idraulico, perdite acqua, scarico intasato, caldaia, boiler, disotturazione + **quartieri e comuni** (liste già utili per long-tail).
- **NAP**: Nome — Telefono — Email **identici** ovunque (sito, schema JSON-LD, scheda Google). Nessun indirizzo falso: “area operativa Torino e provincia” va bene se non c’è sede al pubblico.
- **Schema.org**: `LocalBusiness` + `Plumber`, `telephone`, `email`, `vatID`, `areaServed` (città), `openingHoursSpecification`, `hasMap` o link scheda Google in **`sameAs`** quando disponibile.
- **FAQ**: domande in pagina = stesso testo (o coerente) in **FAQPage** JSON-LD.
- **Meta**: `title` e `description` unici per pagina; `canonical` sul dominio definitivo.
- **Google Business Profile**: categoria corretta, servizi, foto, orari, link al sito, **recensioni reali** — il sito supporta la scheda, non la sostituisce.
- **Tecnico**: `sitemap.xml`, `robots.txt`, HTTPS, URL stabili; aggiornare sitemap/robots se cambi dominio (es. da GitHub Pages a dominio proprio).

---

## 3. Mobile first

- **Viewport**: `width=device-width`, `viewport-fit=cover` per iPhone con notch.
- **Safe area**: padding con `env(safe-area-inset-*)` per top bar, footer fisso e pulsante WhatsApp flottante.
- **Touch**: pulsanti **min. ~48px** di altezza; `touch-action: manipulation` per ridurre ritardo al tap.
- **Tipografia**: `clamp()` per titoli leggibili su schermi piccoli; corpo **≥ 16px** dove possibile.
- **Layout**: griglia a una colonna su mobile; CTA full-width; **ordine contenuti**: urgenza → contatto → servizi → perché noi → zone → FAQ → mappa.
- **Prestazioni**: iframe mappa in contenitore con **aspect-ratio** o altezza definita per limitare **CLS** (salti di layout); `loading="lazy"` sull’iframe; evitare troppi script.
- **Accessibilità**: contrasto colori, focus visibile su link, `aria-label` su icone (telefono, WhatsApp).

---

## 4. Pronto intervento (messaggio e conversioni)

- **Chi / dove / quando / cosa**: in poche righe — idraulico urgente, Torino e prima cintura, H24, tipi di intervento (perdite, scarichi, caldaia…).
- **Promesse**: evitare claim assoluti (“sempre 30 minuti”) se non sono verificabili e documentabili; preferire “intervento rapido”, “operativi H24”, “preventivo chiaro”.
- **CTA**: `tel:+39…` e WhatsApp con **messaggio precompilato**; barra fissa in basso su mobile.
- **Dopo il click**: la conversione vera è **risposta al telefono / WhatsApp** — il sito deve solo ridurre attrito verso la chiamata.
- **Fiducia post-contatto**: preventivo prima dell’intervento quando possibile, garanzia su lavori (come da condizioni reali in contratto/preventivo).

---

## Checklist rapida pre-pubblicazione

- [ ] Numero e email uguali ovunque  
- [ ] Nessun indirizzo inventato  
- [ ] Canonical e sitemap sul dominio finale  
- [ ] `sameAs` con URL Google Business (quando c’è)  
- [ ] Banner cookie + pagine Privacy / Cookie / Termini  
- [ ] Test su telefono reale (CTA, mappa, scroll, banner)  
- [ ] Google Search Console + (opzionale) Google Analytics solo dopo consenso cookie se richiesto dalla policy  

---

*Ultimo aggiornamento note: febbraio 2026.*
