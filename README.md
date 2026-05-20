# Hermes İkincil Beyin Kasası

Bu dizin, session'lar arasında kalıcı bilgi tutan organize bir hafıza sistemidir.
Hermes Agent her oturumda burayı okuyup güncelleyerek devamlılığı sağlar.

## Yapı

```
~/hermes-brain/
├── README.md              # Bu dosya — manifesto
├── systems/               # Çalışan sistemler, servisler, cron job'lar
│   └── cron-jobs.md
├── projects/              # Aktif projeler, durumlar, çıktılar
│   └── income-automation.md
├── ideas/                 # Fikirler, beyin fırtınaları, konseptler
├── preferences/           # Kullanıcı tercihleri, profil bilgisi
│   └── komutan-mehmet.md
├── logs/                  # Zamanlı log'lar, özetler
└── failures/              # Başarısız denemeler ve dersler
```

## Kullanım Protokolü

1. **Session başlangıcı**: `preferences/` ve `systems/` altındaki dosyaları oku.
2. **Güncelleme**: Her önemli işlem sonrası ilgili kategoriye yaz.
3. **Loglama**: `logs/` altına tarihli özetler bırak.
4. **Arşiv**: Aylık olarak eski log'ları `logs/archive/` altına taşı.

## Hedef
Session reset'leri, daily truncate'lar veya uzun aralar sonrası bile
Hermes'in kiminle konuştuğunu, ne çalıştırdığını ve neyi hedeflediğini
unutmamasını sağlamak.
