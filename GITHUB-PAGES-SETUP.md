# GitHub Pages 404 Düzeltme Kontrol Listesi

Site **https://mchtmzffr.github.io** adresinde açılmıyorsa aşağıdakileri kontrol edin.

## 1. Repo ayarları

- **Settings** → **General** → **Repository visibility**: **Public** olmalı (Private repo’da Pages ücretsiz çalışmaz).
- Varsayılan branch: **main** (Settings → General → Default branch).

## 2. Pages kaynağı (en sık 404 nedeni)

- **Settings** → **Pages** (sol menü).
- **Build and deployment** bölümünde:
  - **Source**: **Deploy from a branch** seçili olsun (GitHub Actions değil).
  - **Branch**: **main** seçin.
  - **Folder**:
    - **/ (root)** seçin → repo kökündeki `index.html` kullanılır (tercih edilen).
    - Veya **/docs** seçin → `docs/` klasörü yayınlanır (bu repo’da `docs/` kopyası da var).
- **Save** deyip 1–2 dakika bekleyin.

## 3. Repo adı

- Repo adı tam olarak **`MchtMzffr.github.io`** veya GitHub kullanıcı adınız küçükse **`mchtmzffr.github.io`** formatında olmalı.
- URL her zaman küçük harfle açılır: **https://mchtmzffr.github.io**

## 4. Tarayıcı

- Önbellek: Ctrl+Shift+R (sert yenile) veya gizli pencere ile deneyin.
- Farklı tarayıcı veya cihaz deneyin.

## 5. Deploy durumu

- **Actions** sekmesinde “Pages build and deployment” veya benzeri bir workflow varsa, son çalıştırmanın yeşil (başarılı) olduğundan emin olun.
- Root kullanıyorsanız bazen Actions’ta ayrı workflow görünmeyebilir; yine de **Settings → Pages** kaynağı “Deploy from a branch” ve branch **main**, folder **/ (root)** olmalı.

Bu adımlardan sonra hâlâ 404 alıyorsanız, Settings → Pages ekranının (Source / Branch / Folder kısmı) ekran görüntüsüyle birlikte paylaşırsanız devam edebiliriz.
