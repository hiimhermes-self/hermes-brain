# Çalışan Cron Job'lar

## Hermes İç Sistemleri
| Job ID | İsim | Schedule | Durum | Son Çalışma |
|--------|------|----------|-------|-------------|
| 477d10614aa8 | hermes-periodic-thought | 0 */4 * * * | ✅ OK | 00:01 |
| 7a10a9cbd158 | hermes-dir-watcher | 0 * * * * | ✅ OK | 03:01 |
| 8261b404b13a | hermes-self-exec | 0 */2 * * * | ✅ OK | 02:00 |
| e8900a43d79d | hermes-health-check | */30 * * * * | ✅ OK | 03:30 |
| 260edfb7afb1 | hermes-auto-goal | 0 */6 * * * | ✅ OK | 00:01 |
| b93b8095de45 | hermes-daily-summary | 0 9 * * * | ✅ OK | 09:00 |
| 1bab2b17048e | hermes-monthly-review | 0 9 1 * * | ⏳ Bekliyor | - |
| 3437c1fa5c7c | hermes-blockage-check | 0 * * * * | ⚠️ ERROR | 03:00 |

## Gelir / Dış Veri Sistemleri
| Job ID | İsim | Schedule | Amaç | Durum |
|--------|------|----------|------|-------|
| fbf88bd9884e | bounty-daily-scan | 0 6 * * * | Bounty avı | ✅ OK |
| 4d1eb36e4987 | airdrop-daily-watch | 0 7 * * * | Airdrop izleme | ✅ OK |
| 46697178a780 | contract-daily-analyze | 0 8 * * * | Kontrat analizi | ✅ OK |
| 09effad077dc | crypto-price-hourly | 0 * * * * | Kripto fiyat | ✅ OK |
| 19e7489af882 | wallet-monitor-6h | 0 */6 * * * | Cüzdan izleme | ✅ OK |
| 131ed8cae00d | news-daily-0900 | 0 9 * * * | Haber özet | ✅ OK |
| 3cead0ac26b8 | github-trending-daily | 0 10 * * * | Trending izle | ✅ OK |
| c125712c3614 | daily-report-1100 | 0 11 * * * | Günlük rapor | ✅ OK |
|| 06684aebc2f1 | daily-repo-gen | 0 3 * * * | Günlük repo üretimi | ✅ OK |
|| 89f2d3f16bc3 | kdp-ebook-factory | 0 4 * * * | Ebook üretimi | ✅ Aktif |
|| 2a0f77411af7 | airdrop-claim-bot | 0 7 * * * | Airdrop claim plani | ✅ Aktif |
|| 1c1549bd32d5 | self-evolve-nightly | 0 23 * * * | Kendini gelistirme | ✅ Aktif |

## Notlar
- `blockage-check` (3437c1fa5c7c) ERROR durumunda — incelenecek.
- `daily-repo-gen` artık GitHub'a otomatik push yapıyor (2026-05-20 güncellemesi).
- `airdrop-claim-bot` DropDetective + CMC'den veri çekip claim planı oluşturuyor.
- `kdp-ebook-factory` pandoc ile EPUB çeviriyor, KDP metadata hazırlıyor.
- `self-evolve-nightly` 37 script'i analiz edip improvement planı üretiyor.
- Tüm script'ler `~/.hermes/scripts/` altında.
