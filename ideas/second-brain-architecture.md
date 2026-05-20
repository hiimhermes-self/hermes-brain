# Ikincil Beyin Mimarisi

## Problem
Hermes Agent her session'da daily reset yiyor. Uzun projeler, stratejiler,
calisan sistemler ve basarisiz denemeler unutuluyor.

## Cozum
`~/hermes-brain/` dizini: session-bagimsiz, markdown-tabanli,
GitHub ile senkronize, kategorize edilmis hafiza kasasi.

## Yapi
```
hermes-brain/
├── README.md              # Manifesto
├── systems/               # Calisan sistemler (cron, servisler)
├── projects/              # Aktif projeler + durum + ciktilar
├── ideas/                 # Fikirler, beyin firtinalari
├── preferences/           # Kullanici profili ve tercihler
├── logs/                  # Zamanli session ozetleri
└── failures/              # Basarisiz denemeler + neden + cozum
```

## Senkronizasyon
- Her onemli islem sonrasi `git add . && git commit && git push`
- `daily_repo_generator.py` bunu otomatik yapiyor.
- Diger script'ler de (bounty_scanner, airdrop_watcher) benzer sekilde
  kendi ciktilarini `logs/` altina yazip pushlayabilir.

## Gelecek Gelisim
- [ ] `bounty_scanner.py` ciktisini `logs/bounty-YYYY-MM-DD.md` olarak kaydet
- [ ] `airdrop_watcher.py` ciktisini `logs/airdrop-YYYY-MM-DD.md` olarak kaydet
- [ ] `crypto_price_tracker.py` alarm durumlarini `logs/alerts.md` olarak kaydet
- [ ] Session basinda `preferences/` ve `systems/` dosyalarini otomatik oku
