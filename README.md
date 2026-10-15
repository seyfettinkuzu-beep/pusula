# Proje Komuta Merkezi (telefon uygulaması)

Ana ekrana eklenen bir web uygulaması (PWA). Projelerini, yol haritalarını ve sıradaki adımları gösterir;
Gemini ile konuşarak güncellemeni sağlar. Veri telefonunda kalır.

## Dosyalar
- index.html : uygulamanın tamamı
- manifest.webmanifest, sw.js, icon-*.png : kurulum ve çevrimdışı çalışma için

Projelerin bu klasörde YOK. Onlar ayrı verilen `projelerim.json` dosyasında.
O dosyayı barındırmaya yükleme; sadece telefonuna indirip uygulamadan içe aktar.

## 1. Barındır (bir kez)
Uygulamanın telefondan açılabilmesi için internette bir adrese (https) koyman gerekir.
Ücretsiz seçenekler: GitHub Pages, Netlify, Cloudflare Pages. Bu klasördeki dosyaları olduğu gibi yükle.
Sitenin adresi herkese açık olabilir; uygulama kodunda senin verin ve anahtarın yoktur.

## 2. Telefona kur
- Android (Chrome): adresi aç, menüden "Uygulamayı yükle" ya da "Ana ekrana ekle".
- iPhone (Safari): adresi aç, Paylaş düğmesi, "Ana Ekrana Ekle".

## 3. Gemini bağlantısı
1. https://aistudio.google.com/apikey adresinden API anahtarı al.
2. Uygulamada Ayarlar bölümüne yapıştır, "Kaydet ve dene" de.
Anahtar yalnızca telefonda saklanır, sadece Gemini'ye gönderilir.
Ücretsiz katmanda Google gönderdiğin metni ürün geliştirmede kullanabilir; gizli bilgileri ücretli katmanda kullanmayı düşün.

## 4. Projelerini yükle
Telefonuna `projelerim.json` dosyasını indir, Ayarlar > "Dosyadan içe aktar" ile seç.

## Nasıl çalışır
- Gemini sekmesinde konuşursun. Gemini, projelerini görür ve "şunu tamamla, şunu ekle" gibi güncellemeler önerir.
  Sen "Uygula" demeden hiçbir şey değişmez.
- "Başka sohbetten aktar": Claude'dan ya da başka bir yapay zekadan kopyaladığın metni yapıştırırsın, projeleri ayıklar.
- Gecikmiş, karar bekleyen ve yakın tarihli işler Projeler ekranında üstte görünür.

## Sınırlar
- Uygulama kapalıyken bildirim göndermez; hatırlatmalar uygulamayı açtığında görünür.
- Sohbet geçmişini Gemini ya da Claude uygulamasından kendi başına okumaz; konuşmayı bu uygulamada yaparsın ya da metni yapıştırırsın.
- Veri tarayıcı deposundadır. Ayarlar > "Yedeği indir" ile düzenli yedek al.
- Model adı değişirse Ayarlar'daki Model alanını güncelle (varsayılan: gemini-3.8-flash).
