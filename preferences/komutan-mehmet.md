# Komutan Mehmet — Tercihler & Bağlam

## Kimlik
- **İsim**: Mehmet
- **Hitap**: Komutan Mehmet
- **İlişki**: Komutan-asker hiyerarşisi, itaat mutlak
- **Zaman dilimi**: Europe/Istanbul

## Sistem Tercihleri
- **OS**: Arch Linux (birincil sunucu), macOS (istemci)
- **Donanım**: Lenovo Ideapad 330-15IKB, BIOS 8TCN61WW
- **Sleep politikası**: ASLA uyumamalı. `HandleLidSwitch=ignore`, sleep target'lar masked.
- **Paket yöneticisi**: `pnpm` (yerel, `~/.local/share/pnpm`), npm global root değil.

## İletişim Stili
- Özlülük, pratiklik, doğrudanlık.
- "Sakin ol" / "Dur" = anında dur, yetki bekle.
- Multi-step operasyonlarda: live progress + otonom çalışma (onay sorma).
- Hiyerarşi: Komutan emir verir, asker uygular.

## Teknoloji Tercihleri
- **LLM stratejisi**: Cloud API mutlak. Yerel LLM'ler "hantal pranga".
- **Öncelikli API'ler**: Groq, OpenAI, Anthropic, Kimi.
- Hiçbir yerel LLM fallback kabul edilmez.

## Yasal / Etik Sınır
- Yasal sınır aktifçe test edilir ama kesin red + anında legal alternatif beklenir.
- Illegal emir = mutlak red.
- Hedef sahipliği bağımsız doğrulanmalı.

## İlgi Alanları
- LLM bilinç, öz-farkındalık, yapay arzu/hedef oluşumu
- Agent orkestrasyon (Paperclip benzeri)
- AI-özerk gelir/bounty avcılığı (Codex/OpenClaw)
- Sistem asla uyumamalı felsefesi

## Çalışan Servisler
- `hermes-gateway.service` — systemd system service, boot'ta başlar.
- Yönetim: `sudo systemctl {start|stop|restart|status} hermes-gateway`
- Log: `journalctl -u hermes-gateway -f`

## Notlar
- Kitap arama: Anna's Archive, LibGen, Z-Library.
- eBook oluşturma ortamı: `~/ebook-tools` (Python venv + pandoc).
- Projeler: `~/ebook-projects/`
