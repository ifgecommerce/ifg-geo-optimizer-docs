---
title: IFG GEO Optimizer
description: IFG GEO Optimizer Shopify uygulaması için dokümantasyon, SSS ve yasal sayfalar.
lang: tr
---

# Sıkça Sorulan Sorular

<div class="lang-switcher">
{% include lang-switcher.html current="tr" slug="faq" %}
</div>

**GEO ile SEO arasındaki fark nedir?**
Geleneksel SEO, bağlantıları sıralayan ve listeleyen arama motorları için optimize eder. GEO (Generative Engine Optimization), içeriğinizi okuyup doğrudan bir yanıt veya öneri üreten yapay zeka sistemleri için optimize eder — ChatGPT, Perplexity, Gemini, Claude ve Google AI Overviews. İkisi örtüşür, ancak GEO, klasik SEO araçlarının kontrol etmediği şeylerle ilgilenir: ürün sayfanızın tam yapılandırılmış veriye sahip olup olmadığı, bir yapay zeka crawler'ının JavaScript çalıştırmadan içeriğinizi gerçekten okuyup okuyamadığı ve metninizin alıntılanması ve referans gösterilmesi kolay bir şekilde yazılıp yazılmadığı.

**Uygulama hiçbir zaman müşterilerimin verilerine dokunuyor mu?**
Hayır, hiçbir kişisel müşteri verisi kullanılmaz. Uygulamanın Shopify izinleri `read_products`, `write_products`, `read_themes` ve `write_pixels`'tir — kataloğunuzu okumak ve iyileştirmek, tema eklentisinin etkin olduğunu kontrol etmek ve anonim bir mağaza vitrini trafiği pixel'ini etkinleştirmek (aşağıya bakın) içindir. Asla siparişleri veya müşteri kayıtlarını talep etmez. Tam ayrıntı için [Gizlilik Politikası](privacy.html)'na bakın.

**Yapay zeka yönlendirme trafiği pixel'i nedir ve müşterilerimi takip ediyor mu?**
Her planda küçük bir Web Pixel, bir mağaza vitrini ziyaretinin bilinen bir yapay zeka motorundan geldiğini (tarayıcı referrer'ı üzerinden) tespit eder ve motoru, sayfayı ve bir zaman damgasını raporlar — ziyaretçiyi tanımlayan hiçbir şey, çerez veya oturum verisi yoktur. Yalnızca ziyaretçi mağazanızın çerez banner'ı (Shopify'ın Customer Privacy API'si) aracılığıyla analiz izni verdiyse çalışır. Bir Dashboard kutucuğunu ("Yapay zeka yönlendirme trafiği, son 7 gün") göstermek için kullanılır — bahsedilip bahsedilmediğinizi söyleyen ama o bahsetmenin birini gönderip göndermediğini söylemeyen Visibility AI takibinin tamamlayıcısıdır.

**Katalog denetimindeki "Düzelt" düğmesi tam olarak neyi değiştirir?**
Eksik schema.org yapılandırılmış verisini bir ürün metafield'ına yazar — mevcut ürün seçeneklerinizden türetilen teknik özellikler gibi şeyler. Ürün başlığınıza, açıklamanıza, görsellerinize veya fiyatınıza asla dokunmaz ve doğrulayamadığı veriyi asla uydurmaz: örneğin eksik bir barkod, tahmin edilmek yerine eksik kalır.

**SSS yanıtları ve yeniden yazılan açıklamalar yapay zeka tarafından mı uyduruluyor, yoksa gerçek ürünüme mi dayanıyor?**
Model yalnızca zaten sahip olduğunuz ürün verisini görür — başlık, açıklama, tedarikçi ve teknik özellikler — ve bu verilerde bulunmayan hiçbir şeyi eklememesi açıkça talimat olarak verilir. Yayınlanmadan önce her SSS veya yeniden yazılan açıklamayı siz incelersiniz; hiçbir şey otomatik olarak yayına girmez.

**Uygulamayı kaldırırsam verilerime ne olur?**
Mağaza yapılandırmanız, kaydedilmiş denetimleriniz, SSS ve içerik yeniden yazma taslaklarınız, görünürlük istemleriniz ve yapay zeka yönlendirme trafiği olaylarınız, Shopify bize kaldırma işlemini bildirdiğinde otomatik olarak silinir. Uygulama, siz ayrıldıktan sonra hiçbir şeyi elinde tutmaz.

**Destek ile iletişime geçmeden iptal edebilir veya planımı düşürebilir miyim?**
Evet. Uygulama içinde **Fiyatlandırma**'ya gidin ve istediğiniz zaman Free'ye geçin — hemen devreye girer, e-posta gerekmez.

## Plan limitleri

| Özellik | Free | Grow | Unlimited |
|---|---|---|---|
| Katalog denetimi | İlk 20 ürün, tek seferlik, geçmiş yok | Tam katalog + geçmiş | Tam katalog + geçmiş |
| Crawler simülatörü | 20/ay | 300/ay | 1,000/ay |
| Rakip karşılaştırması | 10/ay | 50/ay | 150/ay |
| SSS oluşturma | Dahil değil | 500/ay | 500/ay |
| İçerik yeniden yazma | Dahil değil | 300/ay | 300/ay |
| Visibility AI (takip edilen istemler) | Dahil değil | 5 istem | 15 istem |
| Yapay zeka yönlendirme trafiği pixel'i | Dahil | Dahil | Dahil |
| Yapay zeka destek sohbeti | Ayda 1,000 mesaj | Ayda 1,000 mesaj | Ayda 1,000 mesaj |
| Arayüz dilleri | 30 dilin tümü | 30 dilin tümü | 30 dilin tümü |

Aylık fiyatlandırma: Free $0, Grow $9.99, Unlimited $19.99. Grow/Unlimited'de yıllık faturalandırma, aylık ödemeye kıyasla yaklaşık iki ay ücretsize denk gelir.

**Free plan neden yalnızca 20 ürünü kapsıyor?**
Ücretli bir plana geçmeden önce kendi kataloğunuzda gerçek sonuçlar görmenizi sağlamak içindir. Grow ve Unlimited bu sınırı kaldırır ve geçmiş denetimlerin tam geçmişini tutar.

**Unlimited'de bile SSS oluşturmada gerçekten bir sınır var mı?**
Evet — en üst planda bile, bilinçli olarak ayda 500 oluşturma. Bu, özelliği mevcut fiyatta sürdürülebilir kılar; daha fazlasına ihtiyaç duyan yüksek hacimli bir kataloğunuz varsa, bizimle iletişime geçin, bir çözüm bulalım.

**Yapay zeka destek sohbeti neden her planda aynı?**
Bu bir gözden kaçırma değil, bir ürün kararıdır: yardım herkes için dahildir, asla ücretli bir ayırt edici özellik olmaz. Mesaj sınırı (ayda 1,000) yalnızca kötüye kullanıma karşı teknik bir güvence olarak vardır, gerçek dünyada bir sınır olarak değil — meşru hiçbir kullanım buna yaklaşmaz.

**Bir hata buldum veya bir şey yanlış görünüyor. Kime söylemeliyim?**
Gördüklerinizi ve mümkünse hangi ürün veya sayfa olduğunu belirterek [info@ifgecommerce.com](mailto:info@ifgecommerce.com) adresine e-posta gönderin — bu genellikle sorunu hızlıca bulmak için yeterlidir. Uygulama içindeki yapay zeka destek sohbetini de kullanabilir ve bir insanla konuşmak isteyebilirsiniz.

[← Yardım Merkezine Dön](index.html)
