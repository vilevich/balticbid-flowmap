# BalticBid — Plūsmu karte (Flow Map)

Interaktīva, draggable node-style wireframe karte BalticBid izsoļu platformai.
Viens pašpietiekams `index.html` — bez build, bez atkarībām.

## Lietošana
- **Velc fonu** — pārvietoties pa karti
- **Ritini** — tuvināt / attālināt
- **Velc kartiņas** — pārkārtot mezglus
- **FIT** poga — atiestatīt skatu

## Publicēšana uz GitHub Pages

```bash
# repo saknē, kur atrodas index.html
git init
git add .
git commit -m "BalticBid flow map"
gh repo create balticbid-flowmap --public --source=. --push

# ieslēdz GitHub Pages (no main branch saknes)
gh api -X POST repos/vilevich/balticbid-flowmap/pages \
  -f "source[branch]=main" -f "source[path]=/" 2>/dev/null || true
```

Links pēc ~1 min: **https://vilevich.github.io/balticbid-flowmap/**

## Saturs
19 ekrāni, sagrupēti: Autentifikācija · Publiskā plūsma · Profils · Admin · Sistēma.
Oranžās līnijas = galvenā lietotāja plūsma; pelēkās = saistītas darbības; pārtrauktās = sekundāras.
