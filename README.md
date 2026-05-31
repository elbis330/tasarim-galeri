# Tasarım Galerisi

UI tasarım asset'lerinin tek bir yerde toplandığı galeri. Her tasarım canlı önizlemeyle listelenir; bir karta tıklayınca tasarımın tam sürümü açılır (etkileşimler ve animasyonlar dahil).

## Canlı

GitHub Pages: `https://elbis330.github.io/<repo>/`

## Yapı

```
index.html              # Galeri ana sayfası
_manifest.json          # Tasarım listesi (slug, başlık, kategori)
designs/<slug>/index.html   # Her tasarımın kendi sayfası
```

## Uyumluluk

Tüm tasarımlar Safari / WebKit / macOS Quick Look / WhatsApp önizleme / iPhone ve Chrome'da düzgün görünecek şekilde uyarlandı:

- İkonlar dış CDN (Font Awesome) yerine satır-içi SVG — internet veya JS gerektirmez.
- Sabit piksel boyutlar ekrana sığacak şekilde responsive yapıldı.
- WebKit'e özgü CSS fallback'leri eklendi (`backdrop-filter`, `background-clip:text`, `mask` vb.).
- Görsel tasarım birebir korundu; sadece dayanıklılık eklendi.

Kum saati tasarımları zaten her ortamda düzgün çalışıyordu, olduğu gibi dahil edildi.
