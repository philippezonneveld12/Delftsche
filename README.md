# Delftsche — Coming Soon

Eenvoudige one-page coming soon site voor [delftsche.com](https://delftsche.com).

## Wat doet 'ie?

- Diep Delfts blauw fullscreen achtergrond met subtiele gradient, vignette en filmkorrel
- "Delftsche" in Italiana (elegante fashion-serif), wit, met dunne ornament-lijntjes erboven en eronder
- Vier delicate botanische hoekornamenten (tulp + ranken, geïnspireerd op klassiek Delfts blauw)
- Na **25 seconden** verschijnt "COMING SOON" smooth fade-in onder de merknaam
- Volledig responsive, respecteert `prefers-reduced-motion`

Eén bestand, geen dependencies, geen build step. Open `index.html` in je browser om te previewen.

## Online zetten

### Optie A — GitHub Pages (gratis, simpel)

1. Maak een nieuwe repo aan: `delftsche-coming-soon` (of `delftsche.github.io` als je dat account hebt)
2. Upload `index.html` naar de root van de repo
3. Repo → **Settings** → **Pages** → Source: `main` branch, folder `/ (root)` → **Save**
4. Na ~1 minuut staat 'ie op `https://<jouw-username>.github.io/delftsche-coming-soon/`
5. Custom domein: voeg een `CNAME` bestand toe met inhoud `delftsche.com`, en zet bij je DNS-provider:
   - `A` records voor `delftsche.com` naar `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - `CNAME` voor `www.delftsche.com` naar `<jouw-username>.github.io`

### Optie B — Vercel (sneller, je gebruikt 'm al)

1. Push de repo naar GitHub
2. Op vercel.com → **New Project** → importeer de repo → **Deploy** (geen config nodig)
3. **Settings** → **Domains** → voeg `delftsche.com` en `www.delftsche.com` toe
4. Volg de DNS-instructies die Vercel geeft

## Aanpassen

- **Timing wijzigen**: zoek `25000` onderin het `<script>` blok (milliseconden)
- **Kleuren**: bovenin het `<style>` blok bij `:root` — `--delft-blue`, `--white` etc.
- **Tekst "Coming Soon"**: zoek `<p class="coming-soon" id="comingSoon">Coming Soon</p>`
- **Botanische ornamenten verbergen op mobiel**: voeg `display: none` toe aan `.botanical` in de mobile media query
