# MerQur Pro: Değişiklik Günlüğü

## 3.4.0 (2026-11) — Doğruluk ve doğrulama; MerQur 2.5.0 tabanı

> "Çalışmadan, yorulmadan, üretmeden rahat yaşamak isteyen toplumlar; önce haysiyetlerini sonra hürriyetlerini ve daha sonra da istiklal ve istikballerini kaybetmeye mahkûmdurlar."
> — Mustafa Kemal Atatürk

- MerQur Pro 3.4.0, ücretsiz MerQur 2.5.0'ın doğruluk ve doğrulama iyileştirmelerini getirir: sonuç değerleri tam duyarlıkla saklanır, çok küçük değerler anlamlı basamakla yazılır.
- Veri yükleme, probit (doğal yanıt), GLMM/GEE, eşbütünleşme ve Cox regresyonunda belirli veri durumlarında sonucu etkileyen hatalar giderildi.
- Panel regresyonu, karma modeller, MANOVA, ARIMA, Cox ve sağlam regresyon, Dunn testi, makine öğrenmesi ve çoklu atamaya yeni seçenekler eklendi (varsayılan olarak kapalı); çok gruplu doğrulayıcı faktör analizi ve ölçme değişmezliği hızlandı.
- Şablon kütüphanesi değişmedi (211 şablon); metinlerde ve kararlılıkta küçük iyileştirmeler yapıldı.

## 3.3.0 (2026-11) — 16 yeni şablon: orman ağacı ıslahı ve nicel genetik, kalite, zaman serisi; MerQur 2.4.1 tabanı

> "Çalışmadan, yorulmadan, üretmeden rahat yaşamak isteyen toplumlar; önce haysiyetlerini sonra hürriyetlerini ve daha sonra da istiklal ve istikballerini kaybetmeye mahkûmdurlar."
> — Mustafa Kemal Atatürk

- 16 yeni şablon (toplam 211), her biri yayımlanmış kaynakla ve eşdeğeri varsa SAS ile karşılaştırıldı:
  - Orman ağacı ıslahı ve nicel genetik:
    - orijin–döl denemesi: varyans bileşenleri; birey ve aile ortalaması kalıtım dereceleri ile standart hataları; değişkenlik katsayıları; iki değişkenli REML ile genetik korelasyon ve standart hatası; farklı bireylerde ölçülen özellikler için B tipi korelasyon; tekrarsız denemeler için model;
    - seleksiyon kazancı ve seleksiyon indeksleri (Smith–Hazel, kısıtlı indeks, Pesek–Baker istenen kazanç indeksi);
    - QST–FST karşılaştırması;
    - tohum bahçesi ve ıslah populasyonunda genetik çeşitlilik (doğurganlık değişkenliği, etkili ebeveyn sayısı, statü sayısı, dış polen katkısı, seyreltmenin etkisi);
    - klon denemesi ve çok lokasyonlu döl denemesi (geniş anlamda kalıtım derecesi, B tipi genetik korelasyon, yaş–yaş korelasyonu).
  - Kalite: çok değişkenli kontrol kartı (Hotelling T², temel bileşen tabanlı T² ve SPE izleme, katkı ayrıştırması); normal olmayan süreç yeterliliği (yüzdelik/Clements, Weibull, lognormal, gama, Johnson, Box-Cox).
  - Zaman serisi ve ekonometri: yapısal VAR (A/B kısıtları, Blanchard–Quah uzun dönem tanımlaması, yapısal etki-tepki, FEVD); genişletilmiş GARCH (GARCH-M, IGARCH, GJR/TGARCH, APARCH, EGARCH, NAGARCH; normal, t, GED); panel sayım modelleri (sabit ve rastgele etkili Poisson ve negatif binom, Hausman testi).
  - Karma model ve sağkalım: faktör analitik kovaryans yapılı karma model (çok çevreli denemeler, genotip × çevre); sıralı ve nominal yanıtlı GEE; kesikli zaman sağkalım modeli (kişi-dönem verisi, lojit/cloglog).
  - Çok değişkenli ve nedensel: yeniden örneklemeli çoklu test düzeltmesi (Westfall–Young maxT ve minP); sosyal ağ analizi (merkezilik, yoğunluk, topluluk bulma); nedensel çizge (DAG) çözümlemesi (ayarlama kümeleri, araç değişkenler, sınanabilir koşullu bağımsızlıklar).
- Grup ardışık tasarım şablonuna yararsızlık sınırı seçeneği (bağlayıcı ve bağlayıcı olmayan β harcaması).
- Genetik örnek verileri: beş genetik şablonun örnek verisi açık lisanslı (CC0) Toros göknarı (Abies cilicica) mikrosatellit verisiyle değiştirildi; şablonlar bu veride yayımlanmış değerlerle yeniden doğrulandı.
- Düzeltme: normal olmayan süreç yeterliliğinde Johnson SB dağılımı, dağılımın tanım aralığı dışındaki gözlemlerde hata vermek yerine birikimli olasılığı 0 ya da 1 alır.
- Ücretsiz MerQur 2.4.0 ve 2.4.1 ile gelen bütün analizler ve düzeltmeler: altı yeni analiz (Gamma/Ters Gauss/Tweedie GLM, göreli risk ve prevalans oranı, karmaşık örneklem sıralı ve çok terimli lojistik regresyon, tolerans aralıkları, ANOM), Rastgeleleştirme Planı aracı, ondalık virgüllü ve metin olarak saklanmış sayıların okunması; Varyans Bileşenleri ile boş hücreli iki yönlü ANOVA, ANCOVA ve çapraz karma model düzeltmeleri.

## 3.2.0 (2026-11) — STM, tohum tescili şablonları, MerQur 2.3.2 tabanı

> "Çalışmadan, yorulmadan, üretmeden rahat yaşamak isteyen toplumlar; önce haysiyetlerini sonra hürriyetlerini ve daha sonra da istiklal ve istikballerini kaybetmeye mahkûmdurlar."
> — Mustafa Kemal Atatürk

- Yeni şablon: yapısal konu modeli (STM); metin sütunundan konular, ortak değişkenlerle konu yaygınlığı ve içeriği, K seçimi, temsilî belgeler, etki grafikleri, konu ağı.
- Yeni: tohum tescili (DUS ve VCU/TDÖ) için beş şablon: yıllar üzerinden birleşik farklılık (COYD; uzun dönem, MJRA, 2×%1, karar şemaları), yıllar üzerinden birleşik yeknesaklık (COYU; göreli varyans), off-type ile yeknesaklık (tek ve iki aşamalı test, OC eğrisi), GAIA fenotipik uzaklık ve Lokasyon × Yıl birleşik tesadüf blokları (TTSM tablosu, sabit/rastgele etki, Satterthwaite ve REML, EMM, AÖF, harf grupları). UPOV TGP/8/5 çözümlü örnekleri ve SAS ile doğrulandı (toplam 195 şablon).
- Şablon çıktılarında dile duyarlı ondalık ayırıcı; şablon hata düzeltmeleri; 14 şablona SAS karşılığı.
- Ücretsiz MerQur 2.3.2 düzeltmeleri: uygulanamayan seçenekler artık sonuçta gerekçesiyle gösterilir, yakınsama uyarıları görünür.
- Açımlayıcı faktör analizi, eğik döndürme: döndürme kareler toplamı sütunu diag(ΦP′P) olarak etiketlenir, yanına yapı matrisinin kareler toplamı (ΣS²) eklenir; "toplanamaz" notu yalnız eğik döndürmede basılır. Sayılar değişmedi.
- MANOVA (çapraz desen): hesap yapılamadığında gerçek neden (boş hücre, tekil tasarım matrisi, yetersiz hata serbestlik derecesi) açıkça yazılır.

## 3.1.0 (2026-11) — 24 yeni şablon, parametre penceresi, atıflar

### Yeni

- **24 yeni doğrulanmış şablon (toplam 189).**

  - Ekonometri: ARDL/NARDL sınır testi, kırılmalı birim kök (Zivot–Andrews, Lee–Strazicich) ve Toda–Yamamoto, ikinci kuşak panel (Pesaran CD, CIPS, Pedroni, Kao, Dumitrescu–Hurlin, CCE/AMG), stokastik sınır analizi, veri zarflama analizi ve Malmquist endeksi, kesikli seçim (karma, iç içe ve gizil sınıf lojit, ödeme isteği).

  - Klinik: klinik tahmin modeli (kısıtlı kübik spline, bootstrap doğrulama, kalibrasyon, karar eğrisi, nomogram), cezalı Cox, RMST regresyonu, çapraz geçiş denemeleri, biyoeşdeğerlik ve kompartımansız analiz, joinpoint ve kesintili zaman serisi.

  - Meta-analiz, YEM ve tasarım: oran meta-analizi (varsayılan GLMM), RI-CLPM ve gizil değişim puanı, dağılım uydurma, sağlam ANOVA, karışım deneyleri, dialel/çizgi × test/artırılmış blok/Latin kare.

  - Genetik, ekoloji ve uzamsal: dizi verisiyle AMOVA ve ikili ΦST, MrBayes ile Bayesçi filogeni, DNA barkodlama ve tür sınırlandırma, dizi hizalama (isteğe bağlı GenBank), doluluk ve yakala-yeniden yakala modelleri, uzay-zaman krigingi.

  - Her biri yayımlanmış kaynakla, eşdeğeri varsa SAS ile karşılaştırıldı.

- **Parametre ayarları penceresi.** Şablonun bütün değişken ve seçenekleri Değişkenler, Model, Seçenekler, Gelişmiş ve Çıktı sekmelerinde ayarlanır; **Tamam ve çalıştır** analizi bu ayarlarla çalıştırır. Yan bölmede kısa özet kalır; şablona çift tıklamak pencereyi açar.

- **Bütün şablonlarda tüm parametreler.** Mevcut 165 şablona alttaki yöntemin anlamlı seçenekleri eklendi (şablon başına ortalama 8 → 13,5 parametre). Varsayılan ayarlarla sonuçlar öncekiyle birebir aynıdır.

- **MrBayes 3.2.9 birlikte gelir** (GNU GPL v3, ayrı program; lisans ve kaynak kodu kurulum klasöründe). Şablon özetleri MrBayes'in kendi sump/sumt çıktısıyla karşılaştırıldı.

- **Yazılım ve atıflar.** Her kod ve şablon koşusunda MerQur Pro, R/Python ve kullanılan paketler sürümleri ve resmî atıflarıyla listelenir; bölüm kod eki kapalıyken de raporda kalır. `.mqs` betiği farklı paket sürümleriyle yeniden çalıştırılırsa uyarı verilir.

- **Yardım → Güncellemeleri Denetle.** Yalnız tıklanınca çalışır; açılışta ağ isteği yoktur.

### Değişen

- Yapay zekâ **kod yardımcısı kaldırıldı.** Sonuç ve rapor yorumu yapan AI Yorumlayıcı sürer. Eski `.mqs` betiklerindeki "yapay zekâ ile üretildi" işareti okunmaya devam eder.

- Lisans sözleşmesi PRO-1.1.0: kod yardımcısı maddeleri çıkarıldı, güncelleme denetimi ve MrBayes bildirimi eklendi. İlk açılışta bir kez yeniden onaylanır.

- `uzay_zaman_kriging` artık gerçek uzay-zaman krigingidir; eski eş-kriging şablonunun adı `es_kriging` oldu (sonuçları değişmedi).

### Düzeltilen

- Şablon formunda 1e-14 gibi çok küçük ondalık değerler 0'a yuvarlanıyordu.

- Bazı şablon seçenekleri ham hata veriyordu ya da İngilizce arayüzde Türkçe sütun adı gösteriyordu (her seçenek tek tek denetlendi). `cift_engel` modelinde paket hatası nedeniyle bc ve ihs dağılımları kaldırıldı.

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

