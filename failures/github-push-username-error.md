# Hata: `could not read Username for 'https://github.com'`

## Zaman
2026-05-20

## Senaryo
`hash-checker-20260519` lokal reposunu GitHub'a pushlamaya calisirken:
```
Unable to add remote "origin"
fatal: could not read Username for 'https://github.com': No such device or address
```

## Kok Neden
`gh` CLI aktif olmasina ragmen (`gh auth status` OK), git'in kendi HTTPS
credential helper'i `gh`'nin token'ini bilmiyordu. `gh auth setup-git`
calistirilmamisti.

## Cozum
```bash
gh auth setup-git
```
Bu komut git config'e `credential.helper` olarak gh'yi ekler.
Ardindan `gh repo create --source=. --push --remote=origin` duzgun calisti.

## Ders
- `gh auth login` yeterli degil, `gh auth setup-git` da gerekli.
- GitHub CLI ve git credential helper arasinda baglanti elle kurulmali.
