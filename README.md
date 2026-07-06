# Sınıf Atlası

Sınıf Atlası, emek mücadeleleri, grevler, direnişler, adalet nöbetleri, ekoloji mücadeleleri ve benzeri toplumsal mücadele başlıklarını harita, canlı tarama ve medya akışıyla izlemek için hazırlanmış tek sayfa web uygulamasıdır.

Bu depo, umutsen.org sitesine entegrasyon için hazırlanmıştır.

## Dosyalar

- `index.html` ana yayın dosyasıdır.
- `sinif-atlasi.html` geliştirme ve doğrudan açılabilir tam sürümdür.
- `direnisscope.template.html` şablon sürümdür.
- `data/direnis-listesi.tsv` mevcut takip listesinin kaynak veri dosyasıdır.
- `docs/umutsen-entegrasyon.md` WordPress ve web sitesi entegrasyon notlarını içerir.
- `Sinif-Atlasi-Baslat.bat` yerelde hızlı test için kullanılabilir.

## Hızlı kullanım

Projeyi doğrudan açmak için `index.html` dosyasını tarayıcıda açabilirsiniz.

Yerelde test için Windows üzerinde `Sinif-Atlasi-Baslat.bat` dosyasını çalıştırabilirsiniz.

## Umut-Sen sitesine entegrasyon

En güvenli entegrasyon yöntemi iframe ile ayrı bir sayfaya gömmektir. Ayrıntılı yönerge için `docs/umutsen-entegrasyon.md` dosyasına bakın.

## Not

Canlı tarama ve medya bölümü API anahtarı gerektirmeden, açık kaynaklardan alınan sonuçları seçili direniş bağlamına göre filtreleyecek şekilde yapılandırılmıştır. İlgili görsel bulunamadığında alakasız görsel göstermek yerine boş durum mesajı gösterir.
