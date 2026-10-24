# Salah — Yasal Sayfa (GitHub Pages)

`index.html`: Gizlilik Politikası + Kullanım Koşulları (TR/EN/AR; `?lang=ar` ile doğrudan dil seçilir). Uygulama içindeki
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

## Google Play Console

- **App content → Privacy policy**: ana sayfa veya `#privacy` linki.
- **App content → Data deletion → Delete account URL**: `#delete-account` linki
  (gizlilik politikasının "Hesap ve Veri Silme" bölümüne kayar; uygulama içi adımları
  ve uygulamasız e-posta ile silme talebini anlatır).

> İçeriği güncellersen hem bu `index.html`'i hem uygulamadaki
> uygulama içi metinleri de güncelle. Her platformun kendi sürümü var (TR/EN/AR):
> iOS `ios/Shared/mobile/src/constants/legal.ts` (sonra `bun ios/scripts/gen-legal.ts`),
> Android `android/app/src/main/assets/data/legal.json`. Web iki platformu birlikte anlatır.
