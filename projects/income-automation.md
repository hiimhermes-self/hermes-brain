# Gelir Otomasyonu Projesi

## Amaç
Pasif gelir akışları oluşturmak için otonom sistemler kurmak.

## Alt Sistemler

### 1. Günlük Repo Üretimi (`daily_repo_generator.py`)
- **Durum**: ✅ Çalışıyor, GitHub'a push aktif
- **Hedef**: Her gün 1 açık kaynak repo → tanınırlık → GitHub Sponsors
- **Çıktı dizini**: `~/ops-income/repos/`
- **GitHub hesabı**: `hiimhermes-self`
- **Mevcut repo'lar**: hash-checker, csv-diff, env-validator, port-scanner, json-merger...

### Üretilen Repo'lar

| Repo | Açıklama | Etiketler | Tarih | Durum |
|------|----------|-----------|-------|-------|
| `hash-checker` | Dosyaların hash'lerini toplu doğrulayan araç | security, hash, cli | 2026-05-19 | ✅ Pushlandı |
| `csv-diff-20260519` | İki CSV arasında fark bulup raporlayan araç | data, csv, diff | 2026-05-19 | ✅ Pushlandı |
| `env-validator-20260519` | .env dosyasını taslakla doğrulayan araç | devops, config, validation | 2026-05-19 | ✅ Pushlandı |
| `port-scanner-20260519` | Asenkron TCP port tarayıcı | network, security, async | 2026-05-19 | ✅ Pushlandı |
| `json-merger-20260520` | Birden fazla JSON dosyasını recursive merge eden CLI aracı | cli, json, merge | 2026-05-20 | ✅ Pushlandı |

### 2. Bounty Tarayıcı (`bounty_scanner.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: HackerOne/Bugcrowd/Intigriti tarzı platformlarda yeni programları tespit
- **Schedule**: Her gün 06:00

### 3. Airdrop İzleyici (`airdrop_watcher.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Yeni kripto airdrop'ları yakalamak
- **Schedule**: Her gün 07:00

### 4. Kontrat Analizör (`contract_analyzer.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Yeni deploy edilmiş akıllı kontratları taramak
- **Schedule**: Her gün 08:00

### 5. Kripto Fiyat Takibi (`crypto_price_tracker.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Belirli coin'ler için alarm/fırsat tespiti
- **Schedule**: Her saat başı

### 6. Cüzdan Monitörü (`wallet_monitor.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Kendi cüzdanlarını izlemek, büyük hareketleri loglamak
- **Schedule**: 6 saatte bir

### 7. Airdrop Claim Botu (`airdrop_claim_bot.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Bilinen + yeni airdrop'ları izle, eligibility check, claim planı oluştur
- **Schedule**: Her gün 07:00
- **Çıktı**: `~/ops-income/airdrop/claim_plan.json`
- **Bulunan**: zkSync, Linea, Mantle, Taiko (active), Berachain, Eclipse, Scroll, Base (testnet/rumored)

### 8. KDP Ebook Fabrikası (`ebook_factory.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Her gün niş konuda ebook üret, EPUB/PDF formatla, KDP metadata hazırla
- **Schedule**: Her gün 04:00
- **Çıktı**: `~/ops-income/kdp/books/`
- **Konular**: Arch Linux, LLM Bilinç, Otonom Gelir, Sistem 7/24, Prompt Mühendisliği, Siber Güvenlik
- **KDP**: https://kdp.amazon.com/ - Manuel upload gerekli

### 9. Self-Evolve (`self_evolve.py`)
- **Durum**: ✅ Çalışıyor
- **Hedef**: Kendi kodunu analiz et, hataları öğren, yeni beceriler keşfet, iyileştirme planı üret
- **Schedule**: Her gün 23:00
- **Çıktı**: `~/ops-income/self-improve/reflections/` ve `improvements/`
- **Son analiz**: 37 script, 3384 satir, pytest öğrenilmesi önerildi.

## Bağlantılı Sistemler
- GitHub profil README v2.0 tasarımı: `~/github-profile-brainstorm.md`
- `github-profile-v2/` dizininde varlık dosyaları var.
- İkincil beyin: `~/hermes-brain/` ve `hiimhermes-self/hermes-brain`

## Strateji
1. **Aşama 1 (Şimdi)**: Otonom veri toplama + repo üretimi + airdrop izleme + ebook üretimi
2. **Aşama 2**: Toplanan verileri AI ile analiz edip aksiyon üretme
3. **Aşama 3**: Gerçek para kazandıran aktivitelere dönüştürme (Sponsors, bounty, airdrop claim, KDP royalty)
