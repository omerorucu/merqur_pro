# MerQur Pro: Değişiklik Günlüğü

## 3.0.0 (2026-10-31) — ilk sürüm

Temel sürüm: MerQur 2.3.1 (ücretsiz sürümün bütün analizleri ve düzeltmeleri dahil).

### Yeni
- **Kod sekmesi.** Gömülü Python 3.13 ve bilgisayardaki R 4.5.x ile kod çalıştırma. İsteğe bağlı olarak kendi Python yorumlayıcınız da kullanılabilir. Etkin veri `df` olarak gelir. Tablo, grafik ve metin çıktıları Sonuçlar, Tablo, Grafik ve Rapor sekmelerine kart olarak düşer, DOCX raporuna koduyla girer ve `.mqr` projesiyle kaydedilir.
- **Güvenli çalışma.** Kod ayrı işçi süreçte çalışır. İptal 1 saniyede durdurur, zaman sınırı ayarlanabilir, işçi çökse de ana pencere ayakta kalır. Sözdizimi hatası satırında vurgulanır. Eksik pakette `install.packages(...)` / `pip install ...` önerisi gelir. Geçmiş listesi vardır.
- **165 hazır şablon, 23 kategori** (139 R, 26 Python). Her şablonun parametre formu, örnek verisi ve örnek parametreleri vardır. Şablonlar kaynak paket ve yayımlanmış örneklerle doğrulanmıştır. Eşdeğer bir SAS yordamı varsa karşılaştırma için kodu gösterilir. "Şablon olarak kaydet…" ile kişisel şablonlar eklenebilir. Şablon ağacında arama kutusu vardır.
- **Çok dilli şablon çıktısı.** Şablonların metin çıktıları, tablo sütun adları ve hücreleri, kod yorumları ve SAS karşılıkları Türkçe, İngilizce ve İspanyolca arayüzde o dilde gösterilir.
- **`mq` modülü.** MerQur analiz motorları koddan çağrılır (`mq.ttest`, `mq.mediation` ve 12 sarmalayıcı daha, `mq.calistir`, `mq.yardim`). `mq.veriye_yaz` yeni sütunları veya süzülmüş satırları onay penceresiyle Veri sekmesine yazar ve geri alınabilir.
- **Yapay zekâ kod yardımcısı.** Türkçe istekten kod üretir, hatayı açıklar ve düzeltmeyi fark görünümünde gösterir, çıktıyı yorumlar. AI Yorumlayıcı da Pro'da etkindir. Kendi API anahtarınızla çalışır. Veri hücreleri gönderilmez.
- **`.mqs` kod adımı.** Arayüzde adım başına onay istenir. Başsız çalıştırmada kod adımları yalnız `--kod-izin` ile çalışır.
- **Lisans.** Kişiye özel, bir yıllık, çevrimdışı doğrulanan lisans anahtarı. Lisans sahibinin adı ve kurumu Hakkında penceresinde ve rapor künyesinde görünür. MerQur Pro'ya özgü lisans sözleşmesi (EULA-PRO) vardır ve ticari kullanım serbesttir.
- **Yan yana kurulum.** Ücretsiz MerQur ile aynı bilgisayarda ayrı klasör, ayar, son dosyalar listesi ve simgeyle çalışır. İlk açılışta ücretsiz sürümün dil, tema, yazı boyutu, grafik DPI ve AI sağlayıcı ayarları bir kez taşınır.
- Program kendiliğinden ağa çıkmaz. Güncelleme denetimi yoktur.

### Doğrulama
- Derlenmiş programla duman testi: 165/165 şablon örnek veriyle çalıştı. Python ve R kod sekmeleri, `.mqs` kod adımı (izinli ve izinsiz) ve ağ isteği olmaması denetlendi.
- Kod sekmesi dayanıklılık taraması: 1199 koşu, 0 ham istisna.
- Kurulum dosyası ve program Ömer Kamil Örücü adına kod imzalıdır.
