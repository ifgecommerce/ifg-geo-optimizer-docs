---
title: IFG GEO Optimizer
description: IFG GEO Optimizer Shopify uygulaması için dokümantasyon, SSS ve yasal sayfalar.
lang: tr
---

# Gizlilik Politikası

<div class="lang-switcher">
{% include lang-switcher.html current="tr" slug="privacy" %}
</div>

**IFG GEO Optimizer** — Generative Engine Optimization için bir Shopify uygulaması
Son güncelleme: Temmuz 2026

## 1. Veri Sorumlusu

**IFG GEO Optimizer** aracılığıyla işlenen kişisel veriler için veri sorumlusu:

**IFG eCommerce** — Roma, İtalya merkezli
E-posta: [info@ifgecommerce.com](mailto:info@ifgecommerce.com)

## 2. Neleri Topluyoruz

- **Satıcı hesap verileri (Shopify OAuth aracılığıyla)**: mağaza alan adınız, bir API erişim token'ı ve Shopify hesabınızdaki e-posta adresi.
- **Katalog verileri (yalnızca okuma)**: ürün başlıkları, açıklamaları, tedarikçi, fiyatlar, seçenekler ve teknik özellikler — denetimler yapmak, crawler davranışını simüle etmek, içerik çıkarılabilirliğini puanlamak ve SSS veya yeniden yazılmış açıklamalar taslak olarak hazırlamak için kullanılır.
- **Mağaza yapılandırması**: aktif planınız, Ayarlar'da girdiğiniz iade ve kargo politikası detayları ve şirket verileri, kaydedilmiş denetimler, SSS ve içerik yeniden yazma taslakları ve yapay zeka görünürlüğü için takip etmeyi seçtiğiniz istemler.
- **Destek sohbeti mesajları**: uygulama içi yapay zeka asistanı ile değiş tokuş ettiğiniz metin, bir insanla konuşmak için açıkça talepte bulunmanız halinde bize iletilen konuşma dökümü dahil.
- **Anonim mağaza vitrini trafiği (Web Pixel, Grow/Unlimited)**: bir ziyaretçi tanınan bir yapay zeka motorundan (ChatGPT, Perplexity, Claude, Gemini, Copilot) bir ürün sayfasına geldiğinde, motoru, sayfa URL'sini ve bir zaman damgasını kaydederiz — yalnızca ziyaretçi mağazanızın çerez banner'ı aracılığıyla analiz izni verdiyse. Hiçbir ziyaretçi kimliği, çerezi veya oturum verisi toplanmaz.
- **Teknik veriler**: istek zaman damgaları, dahili kayıt tanımlayıcıları ve sistem günlükleri.

> Uygulama **asla kişisel son müşteri verisi talep etmez veya almaz** — ad, e-posta, adres veya sipariş yoktur. Talep edilen Shopify izinleri: `read_products`, `write_products` (katalog ve yapılandırılmış veri), `read_themes` (tema eklentisinin etkin olduğunu kontrol etmek) ve `write_pixels` (yukarıdaki anonim trafik pixel'ini etkinleştirmek).

## 3. Neden İşliyoruz ve Hangi Hukuki Dayanakla

Bu verileri, uygulamayı kurma amacınız olan hizmeti sunmak için işliyoruz — GDPR Madde 6(1)(b) uyarınca, bir sözleşmenin ifası: kataloğunuzun üretken arama motorlarındaki görünürlüğünü analiz etmek ve iyileştirmek, yapay zeka destekli SSS taslağı hazırlama ve içerik yeniden yazma, uygulama içi destek sohbeti, seçtiğiniz istemler üzerinde haftalık yapay zeka görünürlüğü takibi ve anonim yapay zeka yönlendirme trafiği ölçümü dahil — tümü ya satıcı tarafından başlatılır ya da trafik pixel'i için mağaza vitrininizde izne bağlıdır.

## 4. Nasıl Topluyoruz

Hesap verileri, kurulum sırasında Shopify'ın OAuth akışı aracılığıyla bir kez toplanır. Katalog verileri, yalnızca dashboard'dan bir işlem tetiklediğinizde Shopify'ın Admin API'si aracılığıyla okunur. Trafik pixel'i mağaza vitrininizde çalışır ve olayları yalnızca izin verildikten sonra raporlar; siz talep etmeden arka planda başka hiçbir şey çalışmaz.

## 5. Kimlerle Paylaşıyoruz

- **Google Firebase / Cloud Firestore** — yapılandırmanızı, oturumlarınızı ve taslaklarınızı saklar. Google LLC (ABD), AB-ABD Veri Gizliliği Çerçevesi'ne (EU-US Data Privacy Framework) katılmaktadır. Veriler europe-west1 bölgesinde (Belçika) saklanır.
- **Anthropic PBC (ABD)** — SSS taslağı hazırlama, içerik yeniden yazma ve uygulama içi destek sohbeti için kullanılan Claude modelini sağlar, yalnızca sizin açık işleminiz üzerine. Yalnızca sizin sağladığınız ürün özniteliklerini veya sohbet metnini alır — asla müşteri verisi almaz.
- **OpenAI, Inc. (ABD)** ve **Perplexity AI, Inc. (ABD)** — yalnızca izlemek için açıkça seçtiğiniz istemler üzerinde haftalık yapay zeka görünürlüğü takibi için kullanılır. Yalnızca takip edilen istem metnini alır — asla müşteri verisi almaz.
- **Google LLC (ABD)** — görünürlük takibi için yukarıdaki OpenAI/Perplexity ile aynı şekilde kullanılan Gemini modelini sağlar (yalnızca depolama olan Firebase/Firestore'dan farklı bir kullanım).
- **Resend, Inc. (ABD)** — yalnızca destek sohbetinde açıkça bir insanla konuşmak istediğinizde, mağaza adı ve destek sohbeti dökümü ile bize bir bildirim gönderir.
- **Shopify Inc.** — platformun kendisi ve uygulamanın kullandığı Admin API ile Web Pixel altyapısının kaynağı.

Veri satmıyoruz ve pazarlama veya davranışsal profilleme için kullanmıyoruz.

## 6. Ne Kadar Süre Saklıyoruz

- **Oturum token'ları**: Shopify'ın çevrimdışı token yaşam döngüsü tarafından yönetilir, otomatik olarak döndürülür.
- **Yapılandırma, denetimler, taslaklar ve trafik olayları**: uygulama kurulu olduğu sürece saklanır. Kaldırma işlemi, mağazanızın yapılandırmasını ve oturumlarını tamamen silen Shopify'ın `shop/redact` webhook'unu tetikler.
- **Teknik günlükler**: Google Cloud'un standart günlük tutma politikası kapsamında saklanır.

## 7. Haklarınız

GDPR Madde 15–22 uyarınca, verilerinize erişim talep edebilir, yanlış verilerin düzeltilmesini veya silinmesini isteyebilirsiniz — en basit yol uygulamayı kaldırmaktır — ya da işlemeye itiraz edebilirsiniz. Ayrıca yerel veri koruma otoritenize şikayette bulunabilirsiniz. Uygulama asla kişisel son müşteri verisi işlemediğinden, `customers/data_request` ve `customers/redact` uyumluluk webhook'ları, dışa aktarılacak veya silinecek hiçbir şey olmadığını onaylayarak yanıt verir.

## 8. Güvenlik

Tüm trafik HTTPS/TLS 1.2+ üzerinden çalışır. Shopify kimlik doğrulama token'ları asla tarayıcıya açığa çıkarılmaz. Her webhook, işlenmeden önce sabit zamanlı bir HMAC SHA-256 kontrolüyle doğrulanır. Veritabanına yalnızca backend'den, barındırma platformunun kendi hizmet kimliği aracılığıyla kimlik doğrulanarak erişilebilir — kodda statik kimlik bilgisi bulunmaz ve doğrudan istemci erişimi, veritabanının kendi güvenlik kurallarınca reddedilir. Veriler hem beklemede hem de aktarım sırasında şifrelenir.

## 9. Değişiklikler

Bu politikayı zaman zaman güncelleyebiliriz. Önemli değişiklikler burada yansıtılacak ve üstteki tarih güncel tutulacaktır.

---

**Verileriniz hakkında sorularınız mı var?**
[info@ifgecommerce.com](mailto:info@ifgecommerce.com)

[← Yardım Merkezine Dön](index.html)
