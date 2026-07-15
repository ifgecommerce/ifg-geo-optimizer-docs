---
title: IFG GEO Optimizer
description: IFG GEO Optimizer Shopify uygulaması için dokümantasyon, SSS ve yasal sayfalar.
lang: tr
---

# Başlarken

<div class="lang-switcher">
{% include lang-switcher.html current="tr" slug="getting-started" %}
</div>

IFG GEO Optimizer'ın, kurulum tamamlandıktan sonra üst gezinme menüsünden erişilebilen dokuz alanı vardır: **Dashboard**, **Katalog denetimi**, **Crawler AI**, **Ürün SSS**, **Link Coach**, **Visibility AI**, **Fiyatlandırma**, **Ayarlar** ve **Destek**. Bu rehber, çoğu satıcının kullandığı sırayla hepsini ele alır.

## 1. Kurulumu yapın ve kurulum sihirbazını tamamlayın

İlk açılışta, kısa bir rehberli kurulum (yaklaşık 2 dakika) temel bilgileri toplar: arayüz dili, iade ve kargo politikanızın detayları, şirket bilgileriniz ve — teknik olarak gerçekten önemli olan tek adım — tema düzenleyicinizde **GEO Schema** uygulama eklentisini (app embed) etkinleştirmek. Bu eklenti etkinleştirilene kadar uygulamanın sonrasında yaptığı hiçbir şey mağaza vitrininize ulaşmaz, bu yüzden bu adımı atlamamakta fayda var. Bu yanıtların herhangi birini daha sonra her zaman **Ayarlar**'dan değiştirebilirsiniz.

## 2. Dashboard

Ana üssünüz. Güncel GEO puanınızı (son denetiminizden), tek bakışta sekiz sinyal içeren bir **Hazırlık Matrisi**'ni — içerik çıkarılabilirliği, Organization şeması, `llms.txt`, `agents.md`, crawler erişimi, MCP hazırlığı, Link Coach bağlantısı ve yapay zeka yönlendirme trafiği — ayrıca öncelik sıralı bir "önce bunu düzelt" listesini ve planınızın kullanım sayaçlarını (SSS oluşturmaları, katalog boyutu) gösterir. Buradaki her şey, üzerinde işlem yapabileceğiniz sayfaya doğrudan bağlantı verir.

## 3. Katalog denetimi

Arama motorlarının aradığı dokuz yapılandırılmış veri alanına göre her ürünü kontrol etmek için **Kataloğu yeniden tara**'ya tıklayın: görsel, açıklama, marka, SKU, GTIN, fiyat, teknik özellikler, iade politikası ve kargo politikası. 80/100'ün altındaki ürünler tam olarak nelerin eksik olduğunu gösterir.

- **Tek tıkla düzeltme**: uygulamanın eksik veriyi güvenle türetebildiği durumlarda (genellikle mevcut ürün seçeneklerinden teknik özellikler), ürünün yapılandırılmış verisine doğrudan yazan bir **Düzelt** düğmesi görürsünüz. Uygulamanın doğrulayamadığı alanlar için hiçbir şey tahmin edilmez — örneğin eksik bir barkod, uydurulmak yerine eksik kalır.
- **Content chunking skoru**: yapılandırılmış veri kontrolünün yanı sıra, her ürün ayrı bir çıkarılabilirlik puanı alır — "alan mevcut mu" değil, "bir AI/RAG sistemi bu açıklamadan gerçekten temiz bir gerçek çıkarabiliyor mu." Zayıf, sıfat ağırlıklı metinler, mükemmel schema.org işaretlemesiyle bile daha düşük puan alır.
- **`llms.txt`**: mağazanızı yapay zeka sistemleri için özetleyen, standartlara uygun gerçek bir `llms.txt` dosyası oluşturur; mağazanızın gerçek kök dizininde (`/llms.txt`) sunulur, crawler'ların bulamayacağı bir app proxy yolunun altına gizlenmez.
- **`agents.md`**: mağazanızı otonom alışveriş ajanlarına anlatan bir dosya oluşturur — varyantlar, arama, ödeme — yalnızca mağazanızın zaten sunduğu gerçek verilerden oluşturulur, hiçbir şey uydurulmaz.
- **Organization şeması**: şirket bilgilerinizi (yasal unvan, vergi/KDV numarası, adres) yapılandırılmış veri olarak yayınlar, böylece yapay zeka motorları sizi önermeden önce gerçek, hesap verebilir bir işletme olduğunuzu doğrulayabilir.

Free planda denetimler ilk 20 ürününüzü, tek seferlik olarak kapsar ve geçmiş tutulmaz. Grow ve Unlimited tüm kataloğunuzu tarar ve trend karşılaştırması için geçmiş her taramayı saklar.

## 4. Crawler AI

Bir ürün seçin, uygulama sayfasını tam olarak bir yapay zeka crawler'ının yaptığı gibi getirir — JavaScript çalıştırmadan, GPTBot, ClaudeBot veya PerplexityBot ile aynı şekilde — böylece bu motorlara tam olarak neyin görünür olduğunu görürsünüz: `robots.txt`'nizin onları engelleyip engellemediği (genel bir izin/red yerine bot bazında kontrol edilir) ve yapılandırılmış verinizin bu botların okuduğu ham HTML içinde gerçekten hayatta kalıp kalmadığı.

**Rakip karşılaştırması** (bu sayfadaki ayrı bir sekme): bir rakibin ürün URL'sini yapıştırın ve aynı GEO sinyallerinin sizinkilerle yan yana karşılaştırmasını alın — rakibin kendi araçlarına kaydolmanıza gerek kalmadan, manuel bir denetimden alacağınız türden aynı farkı.

## 5. Ürün SSS

Grow veya Unlimited'de bir ürün seçin ve yalnızca o ürünün gerçek başlığından, açıklamasından, tedarikçisinden ve özelliklerinden hazırlanan üç ila beş soru-cevap çifti için **SSS Oluştur**'a tıklayın — modele, verilerinizde zaten bulunmayan bir ayrıntıyı asla eklememesi açıkça talimat olarak verilir. Her taslağı inceleyin; siz açıkça **Onayla**madan hiçbir şey yayınlanmaz. Onaylanan SSS'ler canlı ürün sayfasında görünür ve `FAQPage` yapılandırılmış verisi olarak işaretlenir, böylece hem insan tarafından okunabilir hem de makine tarafından alıntılanabilir olurlar.

**İçerik yeniden yazma** (bu sayfadaki ayrı bir sekme): uygulama, bir ürün açıklamasını doğrulanabilir gerçekler açısından daha yoğun ve üretken bir motorun alıntılaması için daha kolay hale getirecek şekilde yeniden yazabilir — ürüne herhangi bir şey geri yazılmadan önce her zaman bir öncesi/sonrası karşılaştırması görür ve onaylarsınız.

## 6. Link Coach

Ürünlerinizin paylaşılan koleksiyonlar, tedarikçiler ve etiketler aracılığıyla birbirine ne kadar iyi bağlı olduğunu analiz eder — iç bağlantı, yapay zeka sistemlerinin kataloğunuzun bir bütün olarak neyi kapsadığını anlamak için kullandığı bir sinyaldir, sadece tek seferde bir sayfa değil. Anlamlı bağlantısı olmayan yalnız kalmış ürünleri ve bunu düzeltmek için açıklanabilir önerileri gösterir.

## 7. Visibility AI

Bir müşterinin gerçekçi olarak bir yapay zeka asistanına sorabileceğini düşündüğünüz birkaç istem ekleyin (limit planınıza bağlıdır — aşağıdaki Fiyatlandırma'ya bakın) ve uygulama her hafta Claude, ChatGPT, Gemini ve Perplexity'nin yanıtta mağazanızdan bahsedip bahsetmediğini kontrol eder, her motor için zaman içinde takip edilir. Grow ve Unlimited'de bu, aynı istemlerde adı belirtilen rakiplerle nasıl karşılaştığınızı da gösterir.

**Yapay zeka yönlendirme trafiği** (Grow ve Unlimited): hafif, gizliliğe saygılı bir pixel, bir mağaza vitrini ziyaretinin gerçekten bu yapay zeka motorlarından birinden geldiğini tespit eder (referrer üzerinden, yalnızca ziyaretçi mağazanızın çerez banner'ı aracılığıyla analiz izni verdikten sonra) ve son 7 günde kaç böyle ziyaret aldığınızı raporlar — yalnızca görünürlük takibinin gösteremediği döngünün ikinci yarısı: sadece "bahsediliyor muyuz" değil, "o bahsetme birini gönderiyor mu."

## 8. Destek

GEO, denetim sonuçlarınız veya belirli bir özelliğin nasıl çalıştığı hakkındaki sorularınız için uygulama içinde bir yapay zeka sohbet asistanı bulunur (sağ alt köşedeki simge). Yardımcı olamazsa, bir insanla konuşmak isteyebilirsiniz ve konuşma doğrudan IFG eCommerce'e iletilir.

## 9. Ayarlar

Kurulum sihirbazı yanıtlarınızı (politikalar, şirket verileri, arayüz dili — yeniden yükleme gecikmesi olmadan 30 dil arasında anında geçiş yapın) yönettiğiniz, tema eklentisi etkinleştirmesini yeniden kontrol ettiğiniz ve hesabınızın Shopify scope'larını gördüğünüz yer.

## 10. Fiyatlandırma

**Fiyatlandırma**, Free, Grow ve Unlimited'i yan yana, aylık veya yıllık olarak gösterir (yıllık ödeme, her iki ücretli katmanda da yaklaşık 2 ay ücretsize denk gelir). Doğrudan uygulama üzerinden istediğiniz zaman planınızı yükseltebilir, düşürebilir veya Free'ye geri dönerek iptal edebilirsiniz — e-posta gerekmez. Kesin plan limitleri için [SSS](faq.html) sayfasına bakın.

İşte döngünün tamamı bu. Çoğu satıcı yeni ürün eklediklerinde denetimi yeniden çalıştırır, bir açıklamayı her güncellediklerinde crawler simülatörünü kontrol eder ve haftalık olarak Dashboard'daki Hazırlık Matrisi'ne göz atar.

[← Yardım Merkezine Dön](index.html)
