# umutsen.org entegrasyon notu

Bu proje umutsen.org içinde ayrı bir sayfa olarak yayınlanmaya uygundur.

## Önerilen yöntem

En temiz yöntem projeyi statik dosya olarak yayınlayıp WordPress tarafında iframe ile göstermektir.

Önerilen sayfa yolu

`https://umutsen.org/sinif-atlasi/`

Önerilen gömme kodu

```html
<iframe
  src="https://sermedol.github.io/direni-g-ncel-tarama/"
  title="Sınıf Atlası"
  style="width:100%; min-height:90vh; border:0; display:block;"
  loading="lazy"
  referrerpolicy="no-referrer-when-downgrade">
</iframe>
```

## WordPress tarafında yapılacaklar

1. Yönetim panelinde yeni bir sayfa açın.
2. Başlığı `Sınıf Atlası` yapın.
3. Özel HTML bloğu ekleyin.
4. Yukarıdaki iframe kodunu yapıştırın.
5. Sayfa genişliğini tam genişlik olarak seçin.
6. Önbellek eklentisi varsa bu sayfada agresif JS/CSS küçültmeyi kapatın.

## Doğrudan tema içine ekleme

Tema dosyalarına doğrudan gömülecekse `index.html` içeriği ayrı bir şablon sayfasına taşınabilir. Harita ve canlı medya fonksiyonları tek HTML içinde tutulduğu için bağımlılık yönetimi düşüktür.

## Medya ve canlı tarama davranışı

- Teknik tarama sayaçları arayüzde gösterilmez.
- Haberler en yeniden en eskiye sıralanır.
- Haber kartları görselli gösterilir.
- İlgili gerçek görsel bulunamazsa alakasız logo yerine ilgili kayıtla ilişkili nötr görsel alanı gösterilir.
- Logo, favicon, site header görseli, reklam ve stok görsel filtrelenir.

## Yayına almadan önce kontrol

- Mobil görünümde panel açılıp kapanıyor mu
- Harita tam genişlikte yükleniyor mu
- Medya sekmesinde teknik filtre kutusu görünmüyor mu
- Haberler yeni tarihten eski tarihe doğru mu
- Haber kartlarının tamamı görselli mi
- Alakasız logo veya banner galeriye düşüyor mu
