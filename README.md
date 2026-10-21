# solusvoidofficial.github.io

User-site repo untuk **My VR Media Player** (`com.solusvoid.myvrplayer`, by SolusVoid).

## Isi

| File | Fungsi |
|---|---|
| `/app-ads.txt` | Authorized Sellers for Apps (AdMob) — WAJIB ada di root domain |
| `/index.html` | Halaman ringkas + link ke situs resmi |

## Kenapa repo ini ada

AdMob mencari `app-ads.txt` di **root hostname** dari URL *developer website* yang terdaftar di
listing Google Play. Website resmi ada di project-page
(`solusvoidofficial/MyVRMediaPlayer` → `https://solusvoidofficial.github.io/MyVRMediaPlayer/`),
dan project-page **tidak bisa** menyajikan file di root. Karena itu repo user-site ini dibuat
dengan nama persis `solusvoidofficial.github.io`.

## Verifikasi

```powershell
curl -I https://solusvoidofficial.github.io/app-ads.txt   # -> 200, text/plain
curl -s https://solusvoidofficial.github.io/app-ads.txt
# -> google.com, pub-5600327675311414, DIRECT, f08c47fec0942fa0
```

## Deploy

GitHub Pages: Settings → Pages → Source: **Deploy from a branch** → `main` / *(root)*.

## Contact

Developer: SolusVoid — solusvoidofficial@gmail.com
