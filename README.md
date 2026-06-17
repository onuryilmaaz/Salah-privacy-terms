# Salah — Yasal Sayfa (GitHub Pages)

`index.html`: Gizlilik Politikası + Kullanım Koşulları (TR/EN). Uygulama içindeki
`LegalModal` ile aynı içerik. App Store Connect zorunlu **Privacy Policy URL** alanı için.

## GitHub Pages ile yayınlama

1. GitHub'da yeni bir public repo oluştur (örn. `salah-legal`).
2. Bu klasördeki `index.html`'i repo köküne yükle (commit + push).
3. Repo → **Settings → Pages** → *Build and deployment* → Source: **Deploy from a branch**.
4. Branch: `main`, klasör: `/ (root)` → **Save**.
5. 1-2 dk sonra yayınlanır:
   - Ana sayfa: `https://<kullanıcı-adı>.github.io/salah-legal/`
   - Gizlilik (doğrudan): `https://<kullanıcı-adı>.github.io/salah-legal/#privacy`
   - Koşullar (doğrudan): `https://<kullanıcı-adı>.github.io/salah-legal/#terms`

## App Store Connect

- **App Privacy → Privacy Policy URL**: ana sayfa veya `#privacy` linkini gir.
- İstersen "Terms of Use (EULA)" alanına da `#terms` linkini ekleyebilirsin
  (zorunlu değil; abonelik eklersen önerilir).

> İçeriği güncellersen hem bu `index.html`'i hem uygulamadaki
> `mobile/src/constants/legal.ts` dosyasını birlikte güncelle (ikisi aynı metin).
