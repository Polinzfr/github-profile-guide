🌍 **Language:** [English](README.md) | [Türkçe](README.tr.md)

# 🎨 GitHub README ve Profil Tasarımı İçin Eksiksiz Rehber

> Güzel ve işlevsel GitHub depo ve profil README'leri hazırlamak için pratik, kapsamlı bir başvuru kaynağı — araçları, teoriyi ve kaçınılması gereken hataları kapsar.

<p align="center">
  <img src="docs/screenshots/header-banner.png" alt="capsule-render ile oluşturulmuş header banner" width="800">
</p>

> [!NOTE]
> Bu rehber, birbiriyle kesişen iki kitle için yazıldı: **depo README**'sini (bir projenin dokümantasyonu) cilalayan geliştiriciler ve **profil README**'sini (GitHub'ın profil sayfanızda gösterdiği özel `kullanıcıadı/kullanıcıadı` deposu) hazırlayan geliştiriciler. Tavsiyelerin ikisi için farklılaştığı yerler açıkça belirtilmiştir.

---

## 📚 İçindekiler

1. [Hızlı Başlangıç](#-hızlı-başlangıç)
2. [Zorluk Göstergesi](#-zorluk-göstergesi)
3. [Araç Kategorileri](#-araç-kategorileri)
4. [Yeni Başlayanlar Yol Haritası](#-yeni-başlayanlar-yol-haritası)
5. [Önerilen Öğrenme Yolu](#-önerilen-öğrenme-yolu)
6. [Temel Araçlar — Detaylı Rehberler](#-temel-araçlar--detaylı-rehberler)
   - [Shields.io](#1-shieldsio)
   - [capsule-render](#2-capsule-render)
   - [Readme Typing SVG](#3-readme-typing-svg)
   - [GitHub Readme Stats](#4-github-readme-stats)
   - [GitHub Readme Streak Stats](#5-github-readme-streak-stats)
   - [Simple Icons](#6-simple-icons)
   - [GitHub Profile README Generator](#7-github-profile-readme-generator)
   - [Contribution Snake / Contribution Painter](#8-contribution-snake--contribution-painter)
7. [README Tasarım Prensipleri](#-readme-tasarım-prensipleri)
8. [Markdown ve GitHub Flavored Markdown Kopya Kâğıdı](#-markdown-ve-github-flavored-markdown-kopya-kâğıdı)
9. [Markdown'da HTML Kullanımı](#-markdownda-html-kullanımı)
10. [README Klasör Yapısı ve Varlık Düzeni](#-readme-klasör-yapısı-ve-varlık-düzeni)
11. [Görsel Optimizasyonu](#-görsel-optimizasyonu)
12. [Erişilebilirlik](#-erişilebilirlik)
13. [Mobil Uyumluluk ve Karanlık Mod](#-mobil-uyumluluk-ve-karanlık-mod)
14. [Rozet, Banner ve İkon Kullanımında Doğru Uygulamalar](#-rozet-banner-ve-ikon-kullanımında-doğru-uygulamalar)
15. [Yerleşim, Tipografi, Renk ve Boşluk](#-yerleşim-tipografi-renk-ve-boşluk)
16. [Sık Yapılan README Hataları](#-sık-yapılan-readme-hataları)
17. [README Kontrol Listesi](#-readme-kontrol-listesi)
18. [Kullanım Senaryosuna Göre Önerilen Araç Kombinasyonları](#-kullanım-senaryosuna-göre-önerilen-araç-kombinasyonları)
19. [Öne Çıkan README Örnekleri ve Koleksiyonlar](#-öne-çıkan-readme-örnekleri-ve-koleksiyonlar)
20. [Kaynaklar](#-kaynaklar)
21. [Sıkça Sorulan Sorular](#-sıkça-sorulan-sorular)

---

## 🚀 Hızlı Başlangıç

Çalışan bir profil README'sine giden en hızlı yol:

1. Adı, GitHub kullanıcı adınızla **birebir aynı** olan yeni bir depo oluşturun (büyük/küçük harf fark etmez ama yine de aynı yazın).
2. **Public** seçeneğini ve **Initialize this repository with a README** kutusunu işaretleyin.
3. GitHub isim eşleşmesini otomatik algılar ve `README.md` dosyasını profil sayfanızda göstermeye başlar.
4. Dosyayı açın, yer tutucu metni silin ve bir başlık, tek satırlık bir biyografi ve bir teknoloji rozeti satırıyla başlayın ([Shields.io](#1-shieldsio) bölümüne bakın).
5. Commit edin. Profil sayfanızı yenileyin — değişiklikler anında görünür, derleme adımı yoktur.

<p align="center">
  <img src="docs/screenshots/create-profile-repo.png" alt="GitHub'da kullanıcı adıyla aynı isimli özel depoyu oluşturma ekranı" width="600">
</p>

> [!TIP]
> Profil README'niz görünmüyorsa en yaygın üç neden şunlardır: depo public değil, depo adı kullanıcı adınızla birebir eşleşmiyor veya README dosyası boş. Tam kontrol listesi için [SSS](#-sıkça-sorulan-sorular) bölümüne bakın.

**Depo README**'si (profil değil, proje dokümantasyonu) için hızlı yol farklıdır: *projenin ne olduğunu*, *nasıl kurulacağını*, *nasıl kullanılacağını* ve *nasıl katkı verileceğini* kapsayan bir şablonla başlayın — bkz. [README Tasarım Prensipleri](#-readme-tasarım-prensipleri).

---

## 📊 Zorluk Göstergesi

Rehber boyunca her aracı ve tekniği derecelendirmek için kullanılır.

| Sembol | Seviye | Anlamı |
|---|---|---|
| 🟢 | Başlangıç | Kurulum olmadan bir Markdown/URL parçasını kopyalayıp yapıştırmak yeterli |
| 🟡 | Orta | Yapılandırma, sorgu parametreleri veya bir hesap gerektirir |
| 🟠 | İleri | Bir workflow dosyası, API token'ı veya kendi sunucunuzda barındırma gerektirir |
| 🔴 | Uzman | Özel kod yazmayı (Actions, script, SVG) gerektirir |

## ⏰ Tahmini Kurulum Süresi

| Araç / Teknik | Süre |
|---|---|
| Shields.io rozeti | 1–2 dakika |
| capsule-render banner'ı | 2–5 dakika |
| Readme Typing SVG | 3–5 dakika |
| GitHub Readme Stats kartı | 2–5 dakika |
| Streak Stats kartı | 2–5 dakika |
| Simple Icons rozet seti | 5–10 dakika |
| Tam profil oluşturucu | 5–15 dakika |
| Contribution snake (GitHub Action) | 15–30 dakika |
| Özel WakaTime / Actions hattı | 30–90 dakika |

---

## 📂 Araç Kategorileri

| Kategori | Neleri kapsar | Rehberdeki araçlar |
|---|---|---|
| **Rozetler** | Küçük durum/metaveri hapları | Shields.io, Simple Icons |
| **Banner'lar ve Başlıklar** | Dekoratif bölüm ayırıcıları | capsule-render |
| **Animasyonlu Metin** | Yazma/silme efektleri | Readme Typing SVG |
| **Canlı İstatistik Widget'ları** | Kendiliğinden güncellenen SVG istatistik kartları | GitHub Readme Stats, Streak Stats |
| **Tam Oluşturucular** | Birkaç aracı birleştiren rehberli oluşturucular | GitHub Profile README Generator |
| **Otomasyon / Actions** | README'nizi yeniden yazan zamanlanmış workflow'lar | Contribution Snake, Contribution Painter |

---

## 🧭 Yeni Başlayanlar Yol Haritası

Daha önce hiç README özelleştirmediyseniz bu sırayı izleyin — her adım bir öncekinin üzerine kurulur ve 15 dakikadan kısa sürer.

1. **Önce gerçek içeriği yazın.** Herhangi bir araca geçmeden önce biyografinizi/proje açıklamanızı düz metin olarak taslak haline getirin. Tasarım sonra gelir.
2. En çok kullandığınız 5–8 teknoloji için [Shields.io](#1-shieldsio) ile bir **rozet satırı** ekleyin.
3. [capsule-render](#2-capsule-render) ile bir **header banner** ekleyin.
4. [GitHub Readme Stats](#4-github-readme-stats) ile **bir istatistik kartı** ekleyin.
5. **GitHub üzerinde önizleyin** (yalnızca yerel bir Markdown görüntüleyicide değil — GitHub'ın render motorunun kendine has tuhaflıkları vardır).
6. **Ancak ondan sonra** animasyonu, streak kartlarını veya Actions tabanlı otomasyonu düşünün.

> [!WARNING]
> 1. adımı atlamak, etkileyici görünen ama hiçbir şey anlatmayan bir README'nin en yaygın nedenidir. Boş bir biyografinin üstündeki rozet duvarı kimseye yardımcı olmaz.

---

## 🎓 Önerilen Öğrenme Yolu

| Aşama | Odak | Sonuç |
|---|---|---|
| 1. Markdown temelleri | Başlıklar, listeler, bağlantılar, görseller, tablolar | Temiz ve yapısal içerik yazabilirsiniz |
| 2. GitHub Flavored Markdown | Callout'lar, görev listeleri, dipnotlar, açılır bölümler | GitHub'a özgü dokümanlar yazabilirsiniz |
| 3. Statik rozetler | Shields.io temelleri | Teknoloji yığını ve durum rozetleri ekleyebilirsiniz |
| 4. Dinamik widget'lar | İstatistik kartları, streak kartları | Kendiliğinden güncellenen içerik ekleyebilirsiniz |
| 5. Markdown içinde HTML | `<details>`, `<picture>`, `<div>` ile hizalama | Yalnızca Markdown'ın sağlayamadığı yerleşimi kontrol edebilirsiniz |
| 6. Otomasyon | README içeriğini yeniden üreten GitHub Actions | Kendini güncelleyen profiller kurabilirsiniz |

---

## 🧰 Temel Araçlar — Detaylı Rehberler

### 1. Shields.io

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 1–2 dakika

#### Kısa Özet
Bir rozet üretme servisi. Bir URL oluşturursunuz, GitHub bunu görsel olarak gösterir ve rozet kendiliğinden güncellenir, çünkü statik bir dosya değil, canlı üretilen bir SVG'dir.

#### Genel Bakış
Shields.io, GitHub'daki rozet standardıdır. Kısa ve tutarlı SVG/PNG rozetler üretir; onlarca paket kayıt servisi, CI sağlayıcısı ve statik veri kaynağıyla çalışır. Derleme durumunu, sürümü, lisansı ve indirme sayısını tek bakışta göstermek için popüler açık kaynak depolarının büyük çoğunluğunda kullanılır.

#### Amaç
Küçük durum veya metaveri bilgilerini (derleme geçti, lisans türü, son sürüm, dil, indirme sayısı) kompakt, kolay taranabilir ve görsel olarak tutarlı bir biçimde iletmek — profil README'lerinde ise teknoloji yığını satırları oluşturmak.

#### Ana Özellikler
- Onlarca desteklenen servis (npm, PyPI, Docker Hub, GitHub Actions, Codecov vb.)
- Keyfi etiket/mesaj/renk kombinasyonları için statik rozetler
- [Simple Icons](#6-simple-icons) slug'ları ile logo desteği
- Birden fazla görsel stil: `flat`, `flat-square`, `plastic`, `for-the-badge`, `social`
- Temel kullanım için hesap veya API anahtarı gerekmez

#### Resmi Web Sitesi
https://shields.io

#### GitHub Deposu
https://github.com/badges/shields

#### Gereksinimler
Yok. Barındırılan bir servistir — yalnızca bir Markdown veya HTML `<img>` etiketine ihtiyacınız var.

#### Kurulum
Kurulacak bir şey yok. Bir URL oluşturup gömün:

```md
![Static Badge](https://img.shields.io/badge/status-active-brightgreen)
```

#### Adım Adım Anlatım

**Adım 1 — Rozetin neyi ileteceğine karar verin.** Durum mu? Sürüm mü? Bir teknoloji yığını öğesi mi? Her birinin URL kalıbı biraz farklıdır.

**Adım 2 — Statik bir rozet için** şu kalıbı kullanın:
```
https://img.shields.io/badge/<ETIKET>-<MESAJ>-<RENK>
```
Örnek:
```md
![License](https://img.shields.io/badge/license-MIT-blue)
```

<p align="center">
  <img src="docs/screenshots/badge-static.png" alt="Statik bir Shields.io rozeti" width="320">
</p>

**Adım 3 — Servise bağlı (kendiliğinden güncellenen) bir rozet için** shields.io rozet oluşturucusunu veya ilgili servisin belgelenmiş uç noktasını kullanın; örneğin npm sürümü:
```md
![npm version](https://img.shields.io/npm/v/react)
```

**Adım 4 — Logo ekleyin.** Bir Simple Icons slug'ı ile `&logo=` ekleyin:
```md
![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)
```

<p align="center">
  <img src="docs/screenshots/badge-logo.png" alt="Logolu bir Shields.io rozeti" width="320">
</p>

**Adım 5 — Tutarlı bir stil seçin.** README boyunca tüm rozetlerde aynı stili kullanın — aynı satırda `flat` ve `for-the-badge` karıştırmak kasıtsız görünür.

**Adım 6 — Rozetleri mantıksal olarak gruplayın** (derleme durumu bir arada, teknoloji yığını bir arada, sosyal medya bir arada) ve gruplar arasına satır boşluğu bırakın.

#### En Uygun Olduğu Durumlar
Teknoloji yığını satırları, proje README'lerinde derleme/lisans/sürüm durumu, profil README'lerinde sosyal/iletişim bağlantı satırları.

#### Avantajlar
- Sıfır kurulum, anında sonuç
- Son derece geniş servis kapsamı
- GitHub genelinde tanınan tutarlı bir görsel dil
- Tek rozetten elli rozete ek araç gerektirmeden ölçeklenir

#### Dezavantajlar
- Aşırı kullanım hızla görsel gürültü yaratır
- Özel renkler hex kodu gerektirir; bu yeni başlayanlar için küçük bir sürtünmedir
- Statik rozetler güncellenmez — eskimelerine izin vermek kolaydır
- Bazı kayıt servisleri yoğun trafikte shields.io'nun proxy'sine hız sınırı uygular

#### Pratik İpuçları
1. Tüm belge boyunca tek bir stil kullanın (`flat-square` en yaygın modern varsayılandır).
2. Tek bir rozet satırını yeni satıra geçmeden önce 6–8 rozetle sınırlayın.
3. Koyu rozet arka planlarında kontrast için `logoColor=white` kullanın.
4. Her rozeti `[![...]](url)` biçiminde ilgili araca veya profile bağlayın.
5. Değişmeyecek şeyler (lisans, "X ile yapıldı") için statik rozet; değişmesi gereken şeyler (sürüm, derleme durumu) için servis rozeti kullanın.
6. Rozet rengini, varsa marka rengiyle eşleştirin (örn. Simple Icons'taki resmi marka hex'i) — daha özenli ve bilinçli bir görünüm verir.
7. Yoğun satırlarda `for-the-badge` stilinden kaçının — büyüktür ve bir iki ana rozet için daha uygundur.
8. Son haline getirmeden önce rozetleri hem GitHub açık hem koyu temasında test edin.
9. Tüm rozet setini tek seferde temalamak için `?style=flat-square&labelColor=...` kullanın.
10. Kimsenin tıklamayacağı şeyi rozetlemeyin — bir rozet ya tek bakışta durum iletmeli ya da işe yarar bir yere bağlanmalı.

#### Sık Yapılan Hatalar
1. Aynı belgede birden fazla rozet stilini karıştırmak.
2. Tutarlı bir palet yerine her şey için varsayılan kırmızı/yeşil/mavi kullanmak.
3. Güncel yığın yerine dokunduğunuz her teknolojiyi rozetlemek.
4. `logoColor`'u unutup logonun koyu rozette görünmez kalması.
5. Dokümantasyon bağlantısı değer katacakken rozetleri bağlantısız bırakmak.
6. Gerçek içeriğin üstünde devasa rozet satırları kullanmak.
7. Rozet markdown'ını kopyalayıp URL'deki kullanıcı adını/depo adını güncellemeyi unutmak.
8. Küçük durum göstergeleri yerine büyük görseller için shields.io kullanmak.
9. GitHub Markdown güncellemelerinden sonra rozetlerin görünümünü kontrol etmemek.
10. 20'den fazla rozeti satırlar halinde gruplamak yerine alt alta dizmek.

#### İlgili Araçlar
[Simple Icons](#6-simple-icons) (logolar için), [capsule-render](#2-capsule-render) (banner'lar için), [shieldcn](https://shieldcn.dev) (shadcn stilinde alternatif rozet/grafik üreticisi).

#### Alternatifler
- **Badgen** — benzer API yapısına sahip, daha hafif ve hızlı bir rozet servisi.
- **shieldcn** — shadcn/ui stilinde rozetler ve grafikler; star-history ve indirme grafikleri dahil, taşınabilir SVG olarak.

#### Karşılaştırma

| Araç | Stil | Hız | Özelleştirme |
|---|---|---|---|
| Shields.io | Flat/plastic/for-the-badge | Hızlı, geniş çapta önbelleğe alınır | Yüksek (renkler, logolar, stiller) |
| Badgen | Minimal flat | Hızlı | Orta |
| shieldcn | shadcn'den esinli | Hızlı | Yüksek, ek olarak grafikler |

#### Gerçek Dünya Kullanım Örnekleri
- Açık kaynak bir kütüphanenin README'sinde derleme/CI durumu.
- Katkıya açık bir depoda "PRs Welcome" rozeti.
- Profil README'sinde teknoloji yığını rozet satırı.
- Benimsenmeyi göstermek için npm/PyPI paketlerinde indirme sayısı rozetleri.

#### Özelleştirme Fikirleri
- Banner'ınızın renk paletine uyan temalı bir rozet satırı oluşturun.
- Eğlenceli, kişisel bir profil dokunuşu için `label=` ile emoji kullanın.
- Ana yığınınızdan ayrı bir "şu an öğreniyorum" rozet satırı oluşturun.

#### SSS

**S: Rozetler README'mi yavaşlatır mı?**
C: Çok az — küçük, önbelleğe alınmış SVG'lerdir; ancak onlarca rozet gerçek HTTP istekleri ekler, o yüzden sayıyı makul tutun.

**S: Shields.io'yu kendi sunucumda barındırabilir miyim?**
C: Evet, depo açık kaynaktır ve kendi sunucuda barındırma talimatlarını içerir; dahili/özel ekosistemler için işe yarar.

**S: Statik bir rozet zamanla eskiyebilir mi?**
C: Evet — statik rozetler siz düzenlemedikçe asla değişmez; bu yüzden gerçeği takip etmesi gereken şeyler (sürüm numaraları gibi) için dinamik/servis rozetleri kullanın.

#### Son Karar
Shields.io, iyi tasarlanmış herhangi bir README için neredeyse zorunludur. Düşük çaba, yüksek getiri ve neredeyse evrensel GitHub desteği sunar. Gereken tek beceri ölçülülüktür.

---

### 2. capsule-render

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 2–5 dakika

#### Kısa Özet
Dalga, dilim, gradyan gibi dekoratif SVG banner'lar üretir; profil README'lerinde header ve footer ayırıcısı olarak kullanılır.

#### Genel Bakış
capsule-render, tamamen URL sorgu parametreleriyle yönetilen, üzerine metninizi yerleştirdiği özelleştirilebilir SVG "kapsül" şekilleri (dalga, yuvarlatılmış dikdörtgen, silindir ve daha fazlası) üreten küçük bir barındırılan API'dir. "Tasarlanmış" bir GitHub profilinin en tanınan görsel imzalarından biri haline gelmiştir.

#### Amaç
Hiçbir görsel düzenleme becerisi gerektirmeden — yalnızca bir sorgu dizesiyle — profil README'sine net bir görsel header ve footer kazandırmak.

#### Ana Özellikler
- Birden fazla şekil: `waving`, `rect`, `slice`, `egg`, `shark`, `cylinder`, `soft`, `venom`, `rounded`, `blur`, `speech`
- Düz veya gradyan renk dolguları
- Yapılandırılabilir metin, yazı boyutu, yükseklik ve animasyon hızı
- Şeklin alt banner için ters çevrilebilmesini sağlayan bölüm konumlandırması (`header` veya `footer`)

#### Resmi Web Sitesi / Depo
https://github.com/kyechan99/capsule-render

#### Gereksinimler
Yok — barındırılan servis, tek bir görsel URL'si.

#### Kurulum
Uygulanamaz. Doğrudan gömün:

```md
![Header](https://capsule-render.vercel.app/api?type=waving&color=gradient&height=200&section=header&text=Hello%2C%20World&fontSize=70)
```

#### Adım Adım Anlatım

**Adım 1 — Bir şekil seçin.** İstediğiniz tona uyanı belirleyin: samimi/rahat için `waving`, minimal/profesyonel için `rect` veya `soft`, cesur ve eğlenceli bir profil için `venom` veya `shark`.

<p align="center">
  <img src="docs/screenshots/capsule-shapes.png" alt="capsule-render şekillerinin karşılaştırması: waving, rect, soft, venom, shark ve slice" width="700">
</p>

**Adım 2 — Rengi ayarlayın.** Adlandırılmış bir renk, hex kodu veya `color=gradient` kullanın (`customColorList` ile özelleştirilebilir); gradyan daha yumuşak bir görünüm verir.

**Adım 3 — Metninizi ekleyin.** `text=` ile yazın (boşlukları `%20` veya `+` olarak URL-encode edin).

**Adım 4 — Yükseklik ve yazı boyutunu ayarlayın.** Metin sıkışmasın diye `height=200` ile `300` arası ve `fontSize=60` ile `80` arası yaygın ve rahat bir aralıktır.

<p align="center">
  <img src="docs/screenshots/header-tuned.png" alt="Ayarları yapılmış bir capsule-render header banner" width="800">
</p>

**Adım 5 — Footer için kopyalayın.** `section=footer` yapın ve çoğu zaman ters çevrilmiş bir şekil kullanın; böylece header ve footer sayfayı görsel olarak iki uçtan çerçeveler.

#### En Uygun Olduğu Durumlar
Profil README header/footer'ları; ara sıra uzun proje README'lerinde bölüm ayırıcı olarak.

#### Avantajlar
- Tasarım aracı gerektirmez
- Tamamen URL ile yönetilir, anında düzenlenebilir
- Geniş şekil/renk çeşitliliği
- GitHub'ın Markdown görsel hattında güvenilir şekilde render edilir

#### Dezavantajlar
- Aşırı kullanılan şekiller (özellikle varsayılan gökkuşağı `waving`) sıradan görünebilir
- Büyük banner'lar profili domine edip asıl içeriği ekranın altına itebilir
- Tasarlanmış bir görsele kıyasla sınırlı tipografi kontrolü
- README'nizin render edilmesine harici bir HTTP bağımlılığı ekler

#### Pratik İpuçları
1. Uyumlu bir görünüm için banner rengini rozet paletinizle eşleştirin.
2. Header yüksekliğini ölçülü tutun — aşırı büyük banner'lar içeriği mobilde ekranın altına iter.
3. `animation=twinkling` ve benzerlerini idareli kullanın; fazla hareket etkileyici değil, dikkat dağıtıcıdır.
4. Eşleşen, ters çevrilmiş bir footer banner'ı sayfaya tasarlanmış ve bilinçli bir kapanış verir.
5. Bilinçli bir marka tercihi değilse varsayılan gökkuşağı gradyanlarından kaçının — en tanınabilir "varsayılan" görünümdür.
6. Banner'ı yalnızca ham görsel olarak değil, gerçek GitHub profil genişliğinde test edin.
7. Header metnini kısa tutun — uzun metinler tahmin edilemez biçimde küçülür veya garip yerden satır atlar.
8. Metin kaymış görünüyorsa dikey ortalamayı ince ayarlamak için `fontAlignY` kullanın.
9. Daha kurumsal/profesyonel bir profil için `soft` veya `rounded` türlerini düşünün.
10. Düzenleme sırasında GitHub eski bir görsel gösteriyorsa bir parametreyi hafifçe değiştirerek önbelleği aşın.

#### Sık Yapılan Hatalar
1. Biyografinizi ve sabitlenmiş projelerinizi ekran dışına iten aşırı büyük bir banner kullanmak.
2. Minimal bir profille çelişen şekil/animasyon kombinasyonu seçmek.
3. Boşluk veya özel karakter içeren metni URL-encode etmeyi unutmak.
4. GitHub'ın koyu temasında çakışan gradyan renkleri kullanmak.
5. Eşleşen bir footer eklememek ve sayfayı yarım bırakmak.
6. Metin uzunluğuna göre fazla büyük yazı boyutu seçip metnin kırpılmasına yol açmak.
7. Typing SVG'yi yoğun bir banner'ın hemen üstüne bindirip ikisini de okunmaz hale getirmek.

#### İlgili Araçlar
[Readme Typing SVG](#3-readme-typing-svg) (genellikle header banner'ın hemen altına yerleştirilir), [Simple Icons](#6-simple-icons).

#### Alternatifler
- Tam yaratıcı kontrol için Figma veya Canva ile hazırlanmış özel statik PNG/SVG banner'lar.
- Daha sade bir alternatif olarak shadcn/ui'den esinlenen **shieldcn** header/banner üreticisi.

#### Karşılaştırma

| Araç | Kontrol | Çaba | Görsel Ağırlık |
|---|---|---|---|
| capsule-render | Sorgu parametresi tabanlı | Düşük | Orta–Yüksek |
| Özel PNG/SVG banner | Tam tasarım kontrolü | Yüksek | Tamamen özel |

#### Gerçek Dünya Kullanım Örnekleri
- Ad/rolü tanıtan profil README header'ı.
- Uzun profillerde "Hakkımda", "İstatistikler" ve "Projeler" blokları arasında bölüm ayırıcılar.
- Kişisel/portfolyo projelerinin depo README header'ları (ciddi açık kaynak kütüphanelerde daha az yaygın).

#### Özelleştirme Fikirleri
- Marka tutarlılığı için ana rozet vurgu renginizi banner'ın düz dolgu rengi olarak kullanın.
- Tekrara düşmeden simetri için aynı renkte `soft` bir header ile `rect` bir footer eşleştirin.

#### SSS

**S: capsule-render yalnızca profillerde mi, depo README'lerinde de çalışır mı?**
C: Evet, sadece bir görsel URL'sidir — Markdown görsellerinin render edildiği her yerde çalışır, ancak en çok profil README'lerinde kullanılır.

**S: Kendi sunucumda barındırabilir miyim?**
C: Proje açık kaynaktır, yani evet; ancak neredeyse herkes barındırılan Vercel uç noktasını kullanır.

#### Son Karar
Bir profil README'sini varsayılan değil, tasarlanmış göstermenin en hızlı yolu. Ölçülü kullanın: sayfaya dağılmış banner'lardan çok, tek ve net bir header (isteğe bağlı olarak eşleşen bir footer) daha iyidir.

---

### 3. Readme Typing SVG

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 3–5 dakika

#### Kısa Özet
Bir dizi satırı yazıp silen animasyonlu bir SVG üretir; genellikle profil header'ının altında kişisel bir slogan olarak kullanılır.

#### Genel Bakış
DenverCoder1 tarafından geliştirilen bu araç, bir metin listesinde daktilo efektiyle dolaşan, kendi içinde tam bir animasyonlu SVG üretir (sizin tarafınızda JavaScript gerekmez). Profil README'lerinde en yaygın benimsenen kişiselleştirme widget'larından biridir.

#### Amaç
Bir ad/header'ın hemen altına dinamik, dikkat çeken bir satır (dönüşümlü sloganlar, roller veya ilgi alanları) eklemek.

#### Ana Özellikler
- Otomatik olarak dönen birden fazla satır
- Yapılandırılabilir yazı tipi, boyut, renk ve arka plan
- Ayarlanabilir yazma/silme/bekleme hızı
- Ortalama hizalama ve genişlik/yükseklik kontrolü
- Tamamen URL parametreleriyle yönetilir, hesap gerekmez

#### Resmi Web Sitesi / Depo
https://github.com/DenverCoder1/readme-typing-svg

#### Gereksinimler
Yok.

#### Kurulum
Görsel olarak gömün:

```md
[![Typing SVG](https://readme-typing-svg.demolab.com/?lines=Hello%2C+I'm+a+developer;I+build+things+for+the+web)](https://git.io/typing-svg)
```

#### Adım Adım Anlatım

**Adım 1 — 2–4 kısa satır yazın.** Her biri kendi başına doğal okunmalı — paragraf değil, dönüşümlü bir alt başlık gibi düşünün.

**Adım 2 — `lines=` parametresini ayarlayın.** Satırlar `;` ile ayrılır ve URL-encode edilir.

<p align="center">
  <img src="docs/screenshots/typing-mid.png" alt="Yazma animasyonunun ortasından bir kare" width="540">
</p>

**Adım 3 — `font`, `size` ve `color` değerlerini** header banner'ınızın paletine uyacak şekilde ayarlayın.

**Adım 4 — header düzeniniz ortalıysa** (HTML `<div align="center">` kullanan profil README'lerinde yaygındır) `center=true` ayarlayın.

**Adım 5 — `pause` ve `duration` değerlerini** okuma temposu doğal hissettirecek biçimde ayarlayın — çok hızlı okunmaz, çok yavaş ağır gelir.

<p align="center">
  <img src="docs/screenshots/typing-final.png" alt="Header banner altına yerleştirilmiş typing SVG" width="700">
</p>

#### En Uygun Olduğu Durumlar
Profil header banner'ının hemen altındaki satır — ad, rol veya dönüşümlü ilgi alanları.

#### Avantajlar
- Kod yazmadan hareket ve kişilik katar
- Tamamen kendi içinde bir SVG, GitHub Action gerekmez
- Yüksek oranda yapılandırılabilir tipografi
- Küçük dosya boyutu, hızlı render

#### Dezavantajlar
- Animasyonlu GIF/SVG'ler metin ağırlıklı bir README'de dikkat dağıtabilir
- Bazı üçüncü taraf Markdown görüntüleyicilerde (README toplayıcılar, bazı IDE'ler) render edilmez
- Ekran okuyucular animasyonlu içeriğin alt metnini garip biçimde okuyabilir
- Aşırı kullanım (bir sayfada birden fazla typing SVG) karmaşık görünür

#### Pratik İpuçları
1. Sayfa başına tek bir typing SVG kullanın — tekil bir odak noktası olarak tasarlanmıştır.
2. `color` değerini rastgele bir varsayılana değil, banner'ınızın vurgu rengine uydurun.
3. Kısa ve vurucu satırlar kullanın — ~40 karakterin altı en iyi okunur.
4. GitHub temasıyla uyum için eşleşen bir `background` ayarlayın (veya saydam bırakın).
5. Cilalı bir hero bölümü için `center=true` ile HTML `<div align="center">` sarmalayıcısını birlikte kullanın.
6. Satır listesini uzatmayın — 3–4 dönüşümlü satır tatlı noktadır.
7. Metin rengi otomatik uyum sağlamadığı için hem GitHub açık hem koyu temasında önizleyin.
8. Kritik bilgiyi yalnızca typing SVG'ye koymayın — bazı izleyicilerin animasyonu görmeyeceğini varsayın.
9. Satırlar daha uzun ifadeler içeriyorsa `pause` değerini biraz yavaşlatın.
10. Sık değişen veriler için değil, kişilik için (roller, ilgi alanları) kullanın — statik metindir, canlı bir akış değildir.

#### Sık Yapılan Hatalar
1. GitHub açık veya koyu arka planında görünmez olan bir renk kullanmak.
2. Mesaj yerine ulaşmasın diye çok fazla dönüşümlü satır doldurmak.
3. Sayfadaki geri kalan her şey ortalıyken `center=true` ayarını unutmak.
4. Özel karakterleri URL-encode etmeyip sorgu dizesini bozmak.
5. Aynı sayfaya iki veya daha fazla typing SVG koymak.
6. Hemen taranabilir olması gereken bilgiler için (örn. e-posta) kullanmak.

#### İlgili Araçlar
[capsule-render](#2-capsule-render) (genellikle hemen üstüne yerleştirilir).

#### Alternatifler
- Statik, kalın bir slogan metni (daha erişilebilir, daha az gösterişli).
- Tam yaratıcı kontrol için elle hazırlanmış özel animasyonlu SVG.

#### Karşılaştırma

| Yaklaşım | Hareket | Erişilebilirlik | Çaba |
|---|---|---|---|
| Readme Typing SVG | Var | Orta | Çok düşük |
| Statik slogan | Yok | Yüksek | Önemsiz |

#### Gerçek Dünya Kullanım Örnekleri
- Bir ad header'ının altında dönen "Full-stack geliştirici \| Açık kaynak tutkunu \| Şu an Rust öğreniyor".
- Portfolyo tarzı bir profilde dönen güncel odak alanları listesi.

#### Özelleştirme Fikirleri
- Konuştuğunuz dilleri dönüşümlü göstererek eğlenceli, kişisel bir dokunuş katın.
- Rengi, istatistik kartlarınızın kullandığı temaya (dracula, tokyonight vb.) eşitleyin.

#### SSS

**S: Ücretli mi?**
C: Hayır, açık kaynaklı bir depo tarafından desteklenen ücretsiz bir barındırılan servistir.

**S: Özel bir yazı tipi kullanabilir miyim?**
C: Evet, `font` parametresinin sunduğu desteklenen Google Fonts kümesi içinde.

#### Son Karar
Profil header'ına gözle görülür bir kişilik katan küçük, düşük çabalı bir ekleme. Tam olarak bir tane kullanın, kısa tutun ve paletini sayfanın geri kalanıyla eşleştirin.

---

### 4. GitHub Readme Stats

**Zorluk:** 🟡 Orta · **Kurulum Süresi:** 2–5 dakika (kendi sunucunuzda barındırırsanız daha uzun)

#### Kısa Özet
GitHub istatistiklerini — yıldızlar, commit'ler, PR'lar, issue'lar ve bir "en çok kullanılan diller" dökümü — gösteren, kart her görüntülendiğinde kendiliğinden güncellenen dinamik SVG kartlar üretir.

#### Genel Bakış
Anuraghazra tarafından geliştirilen bu araç, kendi deposunda on binlerce yıldızı olan, en yaygın kullanılan GitHub istatistik kartı üreticisidir. GitHub'ın API'sini sunucu tarafında sorgular ve bir SVG kart render eder; böylece profilinizdeki rakamlar sizin hiçbir bakım yapmanıza gerek kalmadan her zaman günceldir.

#### Amaç
Elle yazılmış bir iddia yerine gerçek, canlı etkinlik verisini doğrudan profil README'sinde göstermek; hesaba güvenilirlik ve aktiflik hissi katmak.

#### Ana Özellikler
- Stats kartı: yıldızlar, commit'ler, PR'lar, issue'lar, katkıda bulunulan depo sayısı ve hesaplanmış bir sıralama
- Top Languages kartı: depolar genelinde bayt cinsinden dil kullanımı dökümü
- Repo pin kartları: belirli bir sabitlenmiş depoyu öne çıkaran kompakt kart
- Yerleşik temalar (dracula, tokyonight, radical, gruvbox ve daha fazlası)
- Kapsamlı sorgu parametresi özelleştirmesi (belirli istatistikleri gizleme, özel renkler, kenar yarıçapı, ikonlar)

#### Resmi Web Sitesi / Depo
https://github.com/anuraghazra/github-readme-stats

#### Zorluk Notları
Temel gömme 🟢 başlangıç seviyesindedir (tek satır Markdown). Kendi örneğinizi barındırmak (özel depo istatistikleri için veya paylaşılan örneğin hız sınırlarından kaçınmak için gerekir) 🟠 ileri seviyedir.

#### Gereksinimler
Genel barındırılan örnek için yok. Kendi sunucunuzda barındırırsanız kişisel bir GitHub token'ı ve kendi Vercel dağıtımınız gerekir.

#### Kurulum

Temel (barındırılan örnek):
```md
![Your GitHub stats](https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true)
```

Kendi sunucunuzda barındırma (isteğe bağlı, ileri seviye): depoyu fork'layın, Vercel'e dağıtın, kişisel erişim token'ınızla bir `PAT_1` ortam değişkeni ekleyin, ardından görsel URL'sini kendi dağıtım alan adınıza yönlendirin.

#### Adım Adım Anlatım

**Adım 1 — Temel stats kartını gömün.** Kullanıcı adınızı yazın ve daha cilalı bir düzen için `show_icons=true` ayarlayın.

<p align="center">
  <img src="docs/screenshots/stats-default.png" alt="Varsayılan GitHub Readme Stats kartı" width="450">
</p>

**Adım 2 — Bir tema seçin.** Paletinize uyanı seçin, örn. `&theme=tokyonight`.

**Adım 3 — İstemediğiniz istatistikleri `&hide=` ile gizleyin** (örn. henüz hoşunuza gitmiyorsa `stars`'ı gizleyin; ancak şeffaflık genellikle daha doğru tercihtir).

**Adım 4 — İkinci satıra Top Languages kartını ekleyin:**
```md
![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=YOUR_USERNAME&layout=compact&theme=tokyonight)
```

<p align="center">
  <img src="docs/screenshots/top-langs-compact.png" alt="Compact düzende En Çok Kullanılan Diller kartı" width="360">
</p>

**Adım 5 — (İsteğe bağlı) Belirli bir depoyu sabitleyin.** Bir projeyi öne çıkarmak için `/api/pin` uç noktasını kullanın.

**Adım 6 — (İsteğe bağlı, ileri seviye) Kendi sunucunuzda barındırın.** Özel depo katkılarının sayılmasını istiyorsanız veya paylaşılan örnek yoğun saatlerde hız sınırına takılıyorsa.

<p align="center">
  <img src="docs/screenshots/stats-side-by-side.png" alt="Stats kartı ve En Çok Kullanılan Diller kartı yan yana" width="700">
</p>

#### En Uygun Olduğu Durumlar
Elle yazılmış bir iddia yerine, etkinliğin güvenilir ve kendiliğinden güncellenen bir özetini görmek istediğiniz profil README'leri.

#### Avantajlar
- Her zaman güncel — gömüldükten sonra sıfır bakım
- Çoğu profil renk şemasıyla uyuşan geniş tema desteği
- Gerçekten aktif hesaplar için güçlü sosyal kanıt
- İyi belgelenmiş, büyük bir topluluğu olan, aktif olarak bakımı yapılan bir araç

#### Dezavantajlar
- Paylaşılan genel örnek, yoğun yük altında yavaş olabilir veya hız sınırına takılabilir
- Kendi sunucunuzda barındırmadıkça özel katkıları saymaz
- Düşük rakamlı yeni hesaplar için cesaret kırıcı olabilir — görünür metrikler her zaman olumlu değildir
- Gözle görülür görsel ağırlık ekler; sonuna eklemek yerine bilinçli yerleştirme gerektirir

#### Pratik İpuçları
1. Çok dil kullandığınızda Top Languages için `layout=compact` kullanın — varsayılan düzen çok uzayabilir.
2. GitHub temanız zaten `<div>` stiliyle bir kenarlık sağlıyorsa, daha minimal bir görünüm için `hide_border=true` ayarlayın.
3. Tutarlı bir görsel kimlik için stats kartı, streak kartı ve typing SVG arasında `theme=` değerini eşleştirin.
4. Bir ekipteyseniz ve birden fazla profil aynı genel örneğe yoğun yük bindiriyorsa kendi sunucunuzda barındırmayı düşünün.
5. `include_all_commits=true` kullanırken dikkatli olun — commit sayısının temelini değiştirir ve yalnızca bazı izleyiciler ne anlama geldiğini biliyorsa tutarsız görünebilir.
6. Stats kartını biyografinizden önce değil sonra yerleştirin — bir rakamla değil, kim olduğunuzla başlayın.
7. Belirli bir "rank" harfinin peşinden koşmayın; kaba bir sezgiseldir, anlamlı bir yeterlilik belgesi değildir.
8. `count_private=true` değerini yalnızca kendi token'ınızla kendi sunucunuzda barındırırken kullanın, aksi halde sessizce etkisiz kalır.
9. Daha temiz bir yerleşim için stats ve top-languages kartlarını bir HTML tablosu veya flex `<div>` ile yan yana hizalayın.
10. Çakışmaları önlemek için GitHub yeni açık/koyu tema varyantları yayımladığında tema seçiminizi yeniden gözden geçirin.

#### Sık Yapılan Hatalar
1. Beş veya daha fazla istatistik/yardımcı kartı görsel gruplama olmadan alt alta dizmek.
2. Açık modu kullanan izleyiciler için GitHub'ın varsayılan açık moduyla çakışan bir tema kullanmak.
3. Neyi değiştirdiğini anlamadan `include_all_commits=true` ayarlamak.
4. Özel katkıların genel örnekte sayıldığını varsaymak (sayılmaz).
5. Profildeki geri kalan her şey özel renklendirilmişken varsayılan temayı bırakmak.
6. Kartı biyografinin üstüne yerleştirip ziyaretçinin bağlamdan önce rakamları görmesine yol açmak.
7. Mobil görünümü kontrol etmemek — geniş yan yana kart düzenleri küçük ekranlarda taşabilir.

#### İlgili Araçlar
[GitHub Readme Streak Stats](#5-github-readme-streak-stats) (sık birlikte kullanılır), çerçeveleme için [capsule-render](#2-capsule-render).

#### Alternatifler
- SVG/Markdown/PDF/JSON çıktısı veren, 30'dan fazla eklentiye sahip **readme-generator** infografik araçları.
- Hiç metrik göstermek istemeyen geliştiriciler için elle yazılmış "Şu an üzerinde çalıştığım" bölümleri.

#### Karşılaştırma

| Araç | Canlı Veri | Kurulum | Özelleştirme |
|---|---|---|---|
| GitHub Readme Stats | Evet | 🟡 | Yüksek |
| Elle yazılmış "Şimdi" bölümü | Hayır | 🟢 | Tam (sadece metindir) |

#### Gerçek Dünya Kullanım Örnekleri
- Profile göz atan işe alımcılara aktif açık kaynak katkı geçmişini göstermek.
- Bir yığın odağını (örn. çoğunlukla Python ve Go) hızla iletmek için en çok kullanılan dilleri göstermek.
- Pin kartıyla, aksi halde minimal bir profilde tek bir ana projeyi öne çıkarmak.

#### Özelleştirme Fikirleri
- Solda stats kartı, sağda top-languages kartı olacak şekilde iki sütunlu bir HTML tablosu oluşturun.
- Görsel süreklilik için kartın temasını capsule-render header'ınızın rengiyle birebir eşleştirin.

#### SSS

**S: Özel katkılarım neden görünmüyor?**
C: Paylaşılan genel örnek özel katkıları asla saymaz; kendi token'ınızla ve `count_private=true` ile kendi sunucunuzda barındırmanız gerekir.

**S: Kart neden bazen yavaş yükleniyor?**
C: Genel örnek çok sayıda profile hizmet verir ve yoğun saatlerde hız sınırına takılabilir veya kısa süre aşırı yüklenebilir — kendi sunucunuzda barındırmak bunu önler.

#### Son Karar
Bir profil README'sine yapılabilecek en etkili "dinamik" ekleme. Özellikle diğer widget'larla eşleşen bir temayla kullanıldığında, küçük kurulum çabasına değer.

---

### 5. GitHub Readme Streak Stats

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 2–5 dakika

#### Kısa Özet
Mevcut katkı serinizi, en uzun serinizi ve toplam katkılarınızı temalandırılabilir bir SVG kart olarak gösterir.

#### Genel Bakış
Yine DenverCoder1 tarafından geliştirilen bu araç, ham toplamlardan çok katkı düzenliliğine odaklanarak GitHub Readme Stats'ı tamamlar — farklı ve çoğu zaman daha motive edici bir sinyal.

#### Amaç
Birçok geliştiricinin ham yıldız/commit sayılarından daha anlamlı (ve sürdürmesi daha teşvik edici) bulduğu katkı düzenliliğini görsel olarak ödüllendirmek ve göstermek.

#### Ana Özellikler
- Mevcut seri, en uzun seri ve toplam katkılar tek kartta
- Tutarlılık için GitHub Readme Stats'ın tema adlarıyla eşleşen temalandırma
- Özel tarih aralığı desteği
- Kenar yarıçapı, arka plan ve yazı tipi özelleştirmesi

#### Resmi Web Sitesi / Depo
https://github.com/DenverCoder1/github-readme-streak-stats

#### Gereksinimler
Temel kullanım için yok.

#### Kurulum
```md
![GitHub Streak](https://streak-stats.demolab.com/?user=YOUR_USERNAME&theme=tokyonight)
```

#### Adım Adım Anlatım

**Adım 1 — Kartı kullanıcı adınızla gömün.**

<p align="center">
  <img src="docs/screenshots/streak-default.png" alt="Açık ve koyu temada varsayılan Streak Stats kartı" width="450">
</p>

**Adım 2 — Görsel tutarlılık için temayı** GitHub Readme Stats kartınızla eşleştirin.

**Adım 3 — (İsteğe bağlı) Özel bir tarih aralığı ayarlayın.** Seriyi belirli bir pencereye göre hesaplamak istiyorsanız `&date_format=` kullanın.

<p align="center">
  <img src="docs/screenshots/streak-themed.png" alt="Stats kartının yanında temalı Streak Stats kartı" width="800">
</p>

**Adım 4 — Ana stats kartının hemen yanına veya altına yerleştirin**, sayfada başka bir yere dağıtmayın.

#### En Uygun Olduğu Durumlar
Ham hacim yerine tutarlılığı ve alışkanlığı vurgulamak isteyen profiller — özellikle günlük kodlama alışkanlığı kazanan geliştiriciler için motive edici.

#### Avantajlar
- Gerçekten iyi bir alışkanlığı (düzenli katkı) teşvik eder
- Stats kartından görsel olarak farklıdır, tekrara düşmez
- GitHub Readme Stats ile aynı tema kütüphanesini kullanır

#### Dezavantajlar
- "Seriyi canlı tut" baskısı yaratıp düşük değerli commit'lere yol açabilir
- Vercel'de barındırılan diğer widget'larla aynı paylaşılan örnek hız sınırı çekinceleri
- Seriler kaliteyi değil sıklığı ödüllendirir — gerçek etkiyi yanlış yansıtabilir

#### Pratik İpuçları
1. Görsel süreklilik için stats kartınızla aynı `theme=` değerini kullanın.
2. Bir seri sayacı sizi seriyi bozmamak için anlamsız commit'lere itmesin — kart gerçek işi yansıtmalı.
3. Ana stats kartının altına değil, hemen yanına iki sütunlu bir düzende yerleştirin.
4. Katkı düzeniniz bilinçli olarak günlük değilse (örn. işleri toplu yapıyorsanız) bu kartı atlamayı düşünün — olduğundan kötü görünebilir.
5. Düzeniniz kartları zaten özel bir `<div>` kenarlığıyla çerçeveliyorsa `hide_border=true` kullanın.

#### Sık Yapılan Hatalar
1. Streak kartı ile ana stats kartı arasında tema uyumsuzluğu.
2. Uzun süredir kırık bir seriniz varken kartı öne çıkarıp dikkati yanlış şeye çekmek.
3. Destekleyici bir ayrıntı yerine ana metrik olarak ele almak.

#### İlgili Araçlar
[GitHub Readme Stats](#4-github-readme-stats).

#### Alternatifler
Görünür bir seri sayacının yarattığı baskıdan kaçınan, yazılı bir "nasıl çalışıyorum" notu.

#### Karşılaştırma

| Araç | Sinyal Verdiği Şey | Risk |
|---|---|---|
| Streak Stats | Tutarlılık | Düşük değerli commit'leri teşvik edebilir |
| Readme Stats | Hacim ve etkinlik | Kaliteden çok niceliği öne çıkarabilir |

#### Gerçek Dünya Kullanım Örnekleri
"100 günde kod" tarzı kişisel bir meydan okumayı belgeleyen geliştiriciler; tutarlı günlük öğrenme üzerine kurulu profiller.

#### Özelleştirme Fikirleri
Kartın tek başına tüm hikâyeyi anlatmak yerine bağlam içinde okunması için çalışma ritminizi anlatan yazılı bir notla birleştirin (örn. "Commit'leri haftalık toplu yapıyorum").

#### SSS

**S: Özel katkıları sayar mı?**
C: Yalnızca uygun kendi sunucunuzda barındırma/token kurulumuyla; GitHub Readme Stats ile aynı çekince.

#### Son Karar
Ana stats kartına güzel, isteğe bağlı bir tamamlayıcı — seri baskısı sizin için sağlıklı bir motivasyon kaynağı değilse atlayın.

---

### 6. Simple Icons

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 5–10 dakika (tam bir rozet seti için)

#### Kısa Özet
Marka ve teknolojiler için 3.000'den fazla ücretsiz SVG ikondan oluşan bir kütüphane; Shields.io rozetlerinin `logo=` kaynağı olarak ve bağımsız ikon gömmeleri için kullanılır.

#### Genel Bakış
Simple Icons, marka ikonlarını (React, Python, Docker, PostgreSQL ve binlercesi) tutarlı slug'lar ve resmi marka renkleriyle standartlaştırır; bu da onu GitHub genelinde teknoloji yığını rozetlerinin fiili ikon kaynağı yapar.

#### Amaç
Rozetlere ve ikon satırlarına, genel veya uyumsuz ikonlar yerine tanınabilir, tutarlı ve markaya uygun bir görünüm kazandırmak.

#### Ana Özellikler
- Her biri resmi hex rengine sahip binlerce marka/teknoloji ikonu
- Kolay arama için tutarlı slug adlandırması
- CDN'de barındırılan, doğrudan veya Shields.io'nun `logo=` parametresiyle kullanılabilen SVG'ler
- Aranabilir ikon dizini içeren web sitesi

#### Resmi Web Sitesi
https://simpleicons.org

#### GitHub Deposu
https://github.com/simple-icons/simple-icons

#### Gereksinimler
Yok.

#### Kurulum
Rozet kullanımı için kurulum gerekmez — slug'a doğrudan başvurun:
```md
![React](https://img.shields.io/badge/React-61DAFB?logo=react&logoColor=black)
```

#### Adım Adım Anlatım

**Adım 1 — Teknolojinizin slug'ını bulun.** simpleicons.org'da arayın (genellikle küçük harfli addır, örn. `postgresql`, `nextdotjs`).

**Adım 2 — Resmi marka hex rengini not edin.** İkonun ayrıntı sayfasında gösterilir.

<p align="center">
  <img src="docs/screenshots/simple-icons-search.png" alt="Slug ve marka renklerini gösteren Simple Icons arama sayfası" width="800">
</p>

**Adım 3 — Bir Shields.io rozeti oluşturun.** `logo=<slug>` kullanın ve rozet arka planı olarak resmi hex'i verin.

**Adım 4 — `logoColor` seçin.** O arka plana karşı kontrast için genellikle beyaz veya siyah.

**Adım 5 — Tüm yığınınız için tekrarlayın.** Rozet stilini hepsinde aynı tutun.

<p align="center">
  <img src="docs/screenshots/stack-row.png" alt="Simple Icons ile hazırlanmış eksiksiz teknoloji yığını rozet satırı" width="660">
</p>

#### En Uygun Olduğu Durumlar
Tutarlı, markaya uygun bir teknoloji yığını rozet satırı oluşturmak.

#### Avantajlar
- Resmi, doğru marka renkleri — hex kodu tahmin etmeye gerek yok
- Modern araç ve dilleri çok geniş kapsar
- Ücretsiz, açık kaynak, MIT lisanslı
- Shields.io ile sorunsuz çalışır

#### Dezavantajlar
- Bazı çok yeni veya niş araçların henüz ikonu olmayabilir
- Slug adları her zaman sezgisel değildir (küçük arama sürtünmesi)
- Dokunduğunuz her araç için mevcut her ikonu kullanmak netlik değil kalabalık yaratır

#### Pratik İpuçları
1. Yaklaşık bir renk yerine her zaman ikon sayfasındaki resmi marka hex'ini kullanın.
2. İkon stilini tutarlı tutun — ya tüm rozetler ya tüm bağımsız ikonlar; biçimleri karıştırmayın.
3. Yığın satırınızı dokunduğunuz her araç değil, 8–12 temel teknolojiyle sınırlayın.
4. İkonları kategoriye göre (diller, framework'ler, araçlar, bulut) ince başlıklarla gruplayın.
5. Güncellenmiş/yeniden markalanmış logoları periyodik olarak kontrol edin — marka renkleri zamanla değişir.

#### Sık Yapılan Hatalar
1. Resmi rengi kullanmak yerine hex rengi tahmin edip markaya uymayan bir görünüm elde etmek.
2. Bir proje adını değiştirdikten sonra eski slug adını kullanmak.
3. Güncel ve ilgili yığın yerine kullandığınız her teknolojiyi eklemek.
4. Uyumsuz `logoColor` yüzünden ikonun görünmez olması.

#### İlgili Araçlar
[Shields.io](#1-shieldsio) (Simple Icons'ın başlıca kullanıcısı).

#### Alternatifler
Devicon (bazı sunum stilleri için daha animasyon dostu, bir diğer popüler teknoloji ikon seti).

#### Karşılaştırma

| Araç | Kapsam | Renk Doğruluğu | Format |
|---|---|---|---|
| Simple Icons | Çok geniş | Resmi marka hex'i | SVG |
| Devicon | Geniş, geliştirici araçlarına odaklı | Yaklaşık | SVG/Yazı tipi |

#### Gerçek Dünya Kullanım Örnekleri
Teknoloji yığını rozet satırları, "kullandığım araçlar" bölümleri ve sosyal/iletişim ikon satırları (birçok sosyal platform da dahildir).

#### Özelleştirme Fikirleri
Her rozetin aynı arka plan tonunu paylaştığı ama her birinin marka renkli ikonunu koruduğu temalı bir satır oluşturun; daha ölçülü ve profesyonel bir görünüm için.

#### SSS

**S: Simple Icons ticari/profesyonel profiller için ücretsiz mi?**
C: Evet, serbest bir lisansla açık kaynaktır.

#### Son Karar
Shields.io rozetlerini genel değil bilinçli gösteren eksik parça. Tahmin edilen renkler yerine her zaman onu tercih edin.

---

### 7. GitHub Profile README Generator

**Zorluk:** 🟢 Başlangıç · **Kurulum Süresi:** 5–15 dakika

#### Kısa Özet
Yukarıdaki widget'ların birkaçını (rozetler, istatistikler, yazan metin, sosyal bağlantılar) elle Markdown yazmadan tek bir oluşturulmuş README'de birleştiren, form tabanlı bir web aracı.

#### Genel Bakış
Topluluk tarafından geliştirilmiş birkaç oluşturucu var; en bilineni Rahul Jain'in `gh-profile-readme-generator` aracı. Ad, biyografi, beceriler, sosyal bağlantılar gibi alanları doldurursunuz; araç eksiksiz, yapıştırmaya hazır Markdown üretir.

#### Amaç
Rozet URL'lerini ve widget parametrelerini tek tek elle birleştirmek istemeyen geliştiriciler için cilalı bir profil README'sinin giriş engelini düşürmek.

#### Ana Özellikler
- Biyografi, beceriler, sosyal bağlantılar ve destek bağlantılarını kapsayan rehberli form
- Üretilen Markdown'ı kopyalamadan önce canlı önizleme
- Shields.io, GitHub Readme Stats ve sosyal rozetleri otomatik birleştirir
- Hesap gerekmez

#### Resmi Web Sitesi
https://rahuldkjain.github.io/gh-profile-readme-generator/

#### Gereksinimler
Yok — tarayıcı tabanlı araç.

#### Kurulum
Kurulum yok — bir web uygulamasıdır; çıktıyı README'nize kopyalarsınız.

#### Adım Adım Anlatım

**Adım 1 — Oluşturucuyu açın** ve adınızı ve kısa bir biyografiyi doldurun.

<p align="center">
  <img src="docs/screenshots/generator-form.png" alt="GitHub Profile README Generator formu, biyografi bölümü" width="800">
</p>

**Adım 2 — Becerilerinizi seçin.** Verilen ikon listesinden seçin.

**Adım 3 — Sosyal bağlantıları ekleyin** (Twitter/X, LinkedIn, kişisel site vb.).

**Adım 4 — İsteğe bağlı widget'ları etkinleştirin.** GitHub istatistikleri veya bir destek/bağış rozeti gibi.

<p align="center">
  <img src="docs/screenshots/generator-preview.png" alt="GitHub Profile README Generator canlı önizleme" width="800">
</p>

**Adım 5 — Üretilen Markdown'ı kopyalayın** ve profil deponuzun README'sine yapıştırın.

**Adım 6 — Sonrasında elle düzenleyin.** Çıktıyı nihai ürün değil, güçlü bir taslak olarak görün; ifadeleri kişiselleştirin ve genel kalan her şeyi kırpın.

#### En Uygun Olduğu Durumlar
Önce rozet söz dizimini öğrenmeden dakikalar içinde eksiksiz, çalışan bir profil README'si isteyen mutlak yeni başlayanlar.

#### Avantajlar
- "Bitmiş" bir profile son derece hızlı bir yol
- Birden fazla aracı kutudan çıktığı gibi doğru birleştirir
- Örnek üzerinden altta yatan Markdown kalıplarını öğrenmek için iyi

#### Dezavantajlar
- Düzenlenmeden bırakılırsa üretilen çıktı şablon gibi görünebilir
- Seçim yapmak yerine her isteğe bağlı alanı doldurmaya teşvik eder
- Varsayılanları aştığınızda elle oluşturmaktan daha az esnek

#### Pratik İpuçları
1. Üretilen biyografiyi her zaman düzenleyin — varsayılan ifade deneyimli göz için genel görünür.
2. Gerçek içeriğiniz olmayan bölümleri kaldırın (boş "şu an öğreniyorum" yer tutucuları, bölümü hiç koymamaktan daha kötü görünür).
3. Üretilen stats kartlarını varsayılanlarda bırakmak yerine kendi renk seçimlerinize göre yeniden temalayın.
4. Çıktıyı rozet/widget söz dizimi için öğrenme referansı olarak kullanın, sonra elle düzenlemeye geçin.
5. Sunulan her isteğe bağlı rozeti etkinleştirmeyin — seçici davranın.

#### Sık Yapılan Hatalar
1. Üretilen çıktıyı hiç düzenlemeden yayımlamak.
2. Varsayılan biyografi ifadesi gibi yer tutucu metinleri yerinde bırakmak.
3. Sizinle ilgili olanlar yerine sunulan her widget'ı etkinleştirmek.
4. Sosyal bağlantıların oluşturucunun örneğine değil, gerçekten kendi hesaplarınıza işaret ettiğini doğrulamamak.

#### İlgili Araçlar
Yukarıdaki her şey — bu araç Shields.io, Simple Icons ve GitHub Readme Stats'ın bir sarmalayıcısıdır.

#### Alternatifler
Baştan tam kontrol için bu rehberin tekil araç bölümlerini kullanarak README'yi elle oluşturmak.

#### Karşılaştırma

| Yaklaşım | Hız | Özgünlük | Öğrenme Değeri |
|---|---|---|---|
| Oluşturucu | En hızlı | Daha düşük (düzenlenmezse) | Orta |
| Elle oluşturma | Daha yavaş | Yüksek | Yüksek |

#### Gerçek Dünya Kullanım Örnekleri
İlk kez profil README'si hazırlayan bir geliştiricinin, örn. iş arayışı veya hackathon öncesinde hızlı, saygın bir profil oluşturması.

#### Özelleştirme Fikirleri
İskeleyi oluşturucuyla çıkarın, ardından elle özel bir capsule-render banner'ı ve seçilmiş bir Simple Icons rozet satırı ekleyin.

#### SSS

**S: Oluşturulmuş README "hile" veya özgün olmayan bir şey sayılır mı?**
C: Hayır — saygın profillerin çoğu bir oluşturucuyla başlayıp sonra kişiselleştirildi. Önemli olan onu size özgü bir şeye dönüştürmek.

#### Son Karar
Mükemmel bir giriş rampası, son durak değil. Kalıpları öğrenmek için kullanın, sonra en çok önemsediğiniz bölümleri elle oluşturmaya geçin.

---

### 8. Contribution Snake / Contribution Painter

**Zorluk:** 🔴 Uzman (Snake) / 🟠 İleri (Painter) · **Kurulum Süresi:** 15–30 dakika

#### Kısa Özet
Otomasyonla çalışan iki farklı görsel efekt: **contribution snake**, zamanlanmış bir GitHub Action ile katkı grafiğinizin içinden "yiyerek" geçen bir "yılan" animasyonu oluşturur; **Contribution Painter** ise piksel sanatı tasarlamanızı ve onu katkı grafiğinize "boyayan" geçmişe dönük commit'ler üretmesini sağlar.

#### Genel Bakış
Her ikisi de GitHub Actions'a ve Contribution Painter örneğinde commit geçmişi/tarihlerinin doğrudan manipülasyonuna dayanır — yukarıdaki herhangi bir "URL'yi gömün" aracından belirgin biçimde daha ileri seviyedir.

#### Amaç
Snake: gerçek katkı grafiğinizin üzerinde tamamen dekoratif, düzenli güncellenen bir animasyon. Painter: katkı grafiğinizde organik olarak oluşan değil, bilinçli olarak tasarladığınız bir desen elde etmenin yolu.

#### Ana Özellikler

**Contribution Snake:**
- Zamanlanmış çalışan bir GitHub Action (örn. günlük)
- Katkı karelerinizi yiyen animasyonlu bir SVG "yılan" üretir
- Hem açık hem koyu tema varyantlarını otomatik çıkarır

**Contribution Painter:**
- Piksel sanatı tasarlamak için etkileşimli tuval
- Bu sanatı katkı grafiğinizde görünür kılmak için gereken geçmişe dönük commit'leri üretir
- Yoğunluk seviyeleri ve commit çarpanlarını, çok dilli arayüzle destekler

#### Gereksinimler
- GitHub Actions'ın etkin olduğu bir depo (ücretsiz katmanda çalışır)
- YAML workflow dosyalarını düzenleme konusunda rahatlık
- Painter için: ayrı, özel bir depo — bu teknik katkı grafiğini sentetik commit'lerle doldurur ve gerçek bir proje deposunda asla yapılmamalıdır

#### Kurulum (Contribution Snake)

**Adım 1 — Bir workflow dosyası ekleyin** (`.github/workflows/snake.yml`). Yılan üretim action'ını zamanlanmış olarak çalıştırır ve çıktı SVG'sini bir `output` branch'ine commit eder.

**Adım 2 — Üretilen SVG'ye README'nizde başvurun.** Açık/koyu varyantlarıyla bir `<picture>` etiketi kullanın:
```md
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-contribution-grid-snake-dark.svg">
  <img alt="snake" src="https://raw.githubusercontent.com/USERNAME/USERNAME/output/github-contribution-grid-snake.svg">
</picture>
```

<p align="center">
  <img src="docs/screenshots/snake.png" alt="Katkı grafiği üzerinde contribution snake animasyonu" width="700">
</p>

**Adım 3 — Commit edin ve Action'ın zamanlamasına göre çalışmasına izin verin.** SVG bundan sonra otomatik güncellenir.

#### Adım Adım Anlatım (Contribution Painter)

> [!CAUTION]
> Bu teknik, gerçek bir zaman çizelgesinde yapay commit geçmişi oluşturur. Bunun için ayrı, açıkça etiketlenmiş bir depo kullanın — asla ana proje geçmişinizde kullanmayın — ve boyanmış bir grafiğin bazı izleyiciler tarafından etkinliği yanlış gösterme biçimi sayıldığını unutmayın. Dekoratif olduğu konusunda şeffaf olmanız şiddetle tavsiye edilir.

**Adım 1 — Desenizi** aracın etkileşimli tuvalinde tasarlayın.

**Adım 2 — Yoğunluk ve commit çarpanlarını yapılandırın.** Her boyanmış karenin ne kadar "koyu" görüneceğini kontrol edin.

**Adım 3 — Kimlik doğrulayın ve aracın geçmişe dönük commit'leri** GitHub REST API üzerinden ayrı bir depoya göndermesine izin verin.

**Adım 4 — Desenin doğru render edildiğini doğrulayın.** Herkese açık profil grafiğinizde görünmesi kısa bir süre alabilir.

#### En Uygun Olduğu Durumlar
Gerçekten dikkat çekici, "bunu nasıl yapmışlar" dedirten bir profil öğesi isteyen ve GitHub Actions/YAML ile rahat olan geliştiriciler.

#### Avantajlar
- Çok yüksek görsel yenilik — anında öne çıkar
- Snake varyantı kurulduktan sonra tamamen otomatiktir (sıfır süregelen bakım)
- Gerçek GitHub Actions yetkinliğini gösterir; bu kendi başına olumlu bir sinyaldir

#### Dezavantajlar
- Bu rehberdeki diğer araçların hepsinden belirgin biçimde daha zor kurulur
- Contribution Painter, açıkça dekoratif olarak çerçevelenmezse etkinlik düzeyini yanlış gösterebilir
- Bozuk bir workflow (YAML hatası, izin sorunu) sessizce güncellemeyi durdurabilir
- Diğer README araçlarında olmayan bir bakım yüzeyi ekler

#### Pratik İpuçları
1. Workflow'u herkese açık profil deponuzda etkinleştirmeden önce özel bir fork'ta test edin.
2. Hem açık hem koyu SVG varyantıyla `<picture>` kullanın — tek temalı bir yılan diğer modda bozuk görünür.
3. Workflow zamanlamasını günlük yapın, daha sık değil — daha sık çalıştırmanın faydası yoktur.
4. Contribution Painter için her zaman ayrı, açıkça etiketlenmiş bir depo kullanın.
5. Workflow'a yalnızca ihtiyaç duyduğu en az izni verin (output branch'inde `contents: write`).
6. GitHub Actions söz dizimi değişirse sıfırlamanız gerekebileceği için çalışan YAML'ın bir kopyasını başka yerde saklayın.
7. Kurulumdan sonra ilk zamanlanmış çalışmanın gerçekten başarılı olduğunu doğrulamak için Actions sekmesini izleyin.
8. Aynı depoya karşı çok fazla zamanlanmış Action zincirlemeyin — hatalar ayıklaması daha zor hale gelir.
9. Contribution Painter kullanıyorsanız, özellikle profesyonel bağlamlarda boyanmış grafiğin dekoratif olduğunu belirtin.
10. Bakımı yapılmayan topluluk Action'ları platform değişiklikleriyle ara sıra bozulduğundan Action'ı periyodik olarak gözden geçirip güncelleyin.

#### Sık Yapılan Hatalar
1. Koyu mod SVG varyantını unutup yılanın koyu tema izleyicileri için kaybolmasına yol açmak.
2. Contribution Painter'ı ayrı bir depo yerine gerçek bir proje deposunda çalıştırmak.
3. Workflow'lara aşırı geniş izinler vermek.
4. İlk Action çalışmasının gerçekten başarılı olduğunu doğrulamadan işin bittiğini varsaymak.
5. Bozuk bir workflow'un aylarca sessizce güncellemeyi durdurmasına izin vermek.
6. Boyanmış bir katkı grafiğini inceleyenlere veya işverenlere organik etkinlikmiş gibi göstermek.

#### İlgili Araçlar
[GitHub Readme Stats](#4-github-readme-stats), genel GitHub Actions ekosistemi.

#### Alternatifler
Otomasyonu tamamen atlayıp GitHub'ın her profilde zaten gösterdiği organik katkı grafiğine güvenmek — profesyonel bağlamlarda çoğu zaman daha güvenilir tercih.

#### Karşılaştırma

| Araç | Otomasyon | Risk | Getiri |
|---|---|---|---|
| Contribution Snake | Tam (zamanlanmış Action) | Düşük (tamamen dekoratif) | Yüksek görsel yenilik |
| Contribution Painter | Elle tetikleme + Action | Orta (yanlış gösterim riski) | Çok yüksek yenilik |

#### Gerçek Dünya Kullanım Örnekleri
Görsel yeniliğin kişisel markanın parçası olduğu geliştirici ilişkileri ve hackathon odaklı profiller; muhafazakâr/kurumsal profesyonel bağlamlar için daha az uygun.

#### Özelleştirme Fikirleri
Sayfa genelinde tam görsel tutarlılık için yılanın renklerini diğer kartlarınızın tema adıyla eşleştirin.

#### SSS

**S: Bu, gerçek katkı grafiğimi veya diğer depolardaki commit geçmişimi etkiler mi?**
C: Snake yalnızca grafiğinizi okur, değiştirmez. Contribution Painter ise sentetik commit'ler yazar — onu ayrı bir depoyla sınırlayın.

**S: Bozuk bir snake workflow'u profilime zarar verir mi?**
C: Yalnızca görsel olarak — eski kalmış bir görsel — ama uzun süre sessizce güncellemeyi durdurmaması için izlemeye değer.

#### Son Karar
Bu rehberdeki en ileri seviye ve görsel olarak en çarpıcı araçlar; GitHub Actions ile rahat olduğunuzda uygundur. Bir yeni başlayanın ilk adımı değildir — önceki araçlarda ustalaştıktan sonra buraya dönün.

---

## 📐 README Tasarım Prensipleri

> [!IMPORTANT]
> Bu rehberdeki her araç iletişime hizmet eder. Bir README'nin işi, ziyaretçinin sorularını mümkün olan en hızlı şekilde yanıtlamaktır — tasarım sürtünmeyi azaltmalı, asla kendi başına süs olarak eklenmemelidir.

**Depo README'leri için** tutarlı biçimde işe yarayan temel yapı:

1. **Proje adı + tek satırlık açıklama** — ne olduğu, hemen.
2. **Rozetler** — derleme durumu, sürüm, lisans (yalnızca anlamlı olanlar).
3. **Kısa demo** — proje görselse, ekranın üst kısmında bir ekran görüntüsü veya GIF.
4. **Kurulum** — kopyalanıp yapıştırılabilir komutlar.
5. **Kullanım** — minimal çalışan bir örnek.
6. **Yapılandırma/API referansı** — gerektiği kadar, çoğu zaman tam dokümana bağlanarak.
7. **Katkıda bulunma** — nasıl dahil olunur.
8. **Lisans**.

**Profil README'leri için** tutarlı biçimde işe yarayan temel yapı:

1. **Header banner** (isteğe bağlı ama yaygın).
2. **Ad ve tek satırlık kimlik** — rol, odak veya ilgi alanı.
3. **Kısa biyografi** — 2–4 cümle, gerçek içerik, sadece rozet değil.
4. **Teknoloji yığını rozetleri**.
5. **İstatistik/streak kartları** (isteğe bağlı).
6. **Sabitlenmiş/öne çıkan projeler** — tam açıklamaları tekrarlamak yerine bağlantı verin.
7. **İletişim/sosyal bağlantılar**.

Her ikisinde de aynı prensipler geçerlidir:

- **Önce öz, sonra süs.** Ziyaretçi tek bir rozet görmeden önce projeyi veya kişiyi anlamalıdır.
- **Tutarlılık çeşitliliği yener.** Tek rozet stili, tek tema, tek renk paleti bilinçli görünür; stil karışıklığı bitmemiş görünür.
- **Her öğe bir soruyu yanıtlamalı.** Bir rozet, kart veya bölüm birinin projeyi/profili anlamasına veya kullanmasına yardımcı olmuyorsa çıkarın.
- **Göz gezdirmeye göre tasarlayın.** Başlıklar, kısa paragraflar ve madde işaretleri ziyaretçinin ihtiyacı olanı saniyeler içinde bulmasını sağlar.

---

## 📝 Markdown ve GitHub Flavored Markdown Kopya Kâğıdı

| Öğe | Sözdizimi |
|---|---|
| Başlık | `# H1` ile `###### H6` arası |
| Kalın | `**kalın**` |
| İtalik | `*italik*` |
| Üstü çizili | `~~metin~~` |
| Bağlantı | `[metin](url)` |
| Görsel | `![alt](url)` |
| Satır içi kod | `` `kod` `` |
| Kod bloğu | ```` ```dil ... ``` ```` |
| Alıntı | `> alıntı` |
| Sırasız liste | `- öğe` |
| Sıralı liste | `1. öğe` |
| Görev listesi | `- [ ] yapılacak` / `- [x] yapıldı` |
| Tablo | `\| sütun \| sütun \|` ve bir `---` ayırıcı satırı |
| Yatay çizgi | `---` |
| Dipnot | `Metin[^1]` sonra `[^1]: not` |

**GitHub'a özgü eklentiler:**

| Özellik | Sözdizimi |
|---|---|
| Callout'lar | `> [!NOTE]`, `> [!TIP]`, `> [!IMPORTANT]`, `> [!WARNING]`, `> [!CAUTION]` |
| Anmalar | `@kullanıcıadı` |
| Issue/PR referansı | `#123` |
| Emoji kısa kodları | `:rocket:` → 🚀 |
| Açılır bölüm | `<details><summary>Başlık</summary>Gövde</details>` |
| Mermaid diyagramları | ```` ```mermaid ... ``` ```` |
| Bağlantı çapaları | Başlıklar otomatik `#anchor-links` alır |

> [!TIP]
> Callout'lar (`> [!NOTE]` vb.) GitHub Markdown'ının en değerli ve en az kullanılan özelliklerindendir — renkli bir ikon ve etiketle render edilirler ve özel HTML olmadan uyarılara, ipuçlarına veya önemli duyurulara anında dikkat çekerler.

---

## 🧩 Markdown'da HTML Kullanımı

GitHub'ın Markdown render motoru, yalnızca Markdown'ın sağlayamadığı yerleşim kontrolü için işe yarayan, güvenli bir HTML alt kümesini destekler:

```html
<div align="center">
  <img src="banner.png" width="100%">
  <h1>Proje Adı</h1>
</div>
```

Yaygın, güvenli kalıplar:

- **Ortalama:** `<div align="center">...</div>`
- **Yan yana kartlar:** kenarlıksız bir HTML `<table>`, her hücrede bir widget
- **Açılır içerik:** `<details><summary>Genişletmek için tıklayın</summary>...</details>`
- **Temaya duyarlı görseller:** `<source media="(prefers-color-scheme: dark)">` içeren `<picture>`
- **Görsel boyutlandırma:** `<img src="..." width="400">` (Markdown görsel söz diziminde boyut kontrolü yoktur)

> [!WARNING]
> Script'ler, formlar ve birçok etkileşimli HTML öğesi güvenlik nedeniyle GitHub'ın temizleyicisi tarafından kaldırılır. Yapısal/yerleşim etiketlerine bağlı kalın — çalıştırılması gereken hiçbir şey için HTML'e güvenmeyin.

---

## 📁 README Klasör Yapısı ve Varlık Düzeni

Anlamlı görsel varlıkları olan depolar için temiz bir kalıp:

```
your-repo/
├── README.md
├── docs/
│   └── screenshots/
│       ├── demo.png
│       └── architecture.png
├── .github/
│   └── workflows/
└── assets/
    └── logo.svg
```

- Görselleri depo kök dizininden uzak tutun — ayrılmış bir `docs/` veya `assets/` klasörü üst düzeyi taranabilir tutar.
- Mümkün olduğunda mutlak GitHub URL'leri yerine göreli yollarla (`docs/screenshots/demo.png`) başvurun — göreli yollar fork'larda ve yeniden adlandırılan branch'lerde çalışmaya devam eder.
- Profil README'leri için, profil depoları genellikle başka açıdan minimal olduğundan, özel/gizli bir varlık barındırıcısı (veya deponun kendi `assets/` klasörü) standarttır.

---

## 🌄 Görsel Optimizasyonu

- **Commit'lemeden önce sıkıştırın.** PNG'ler ve GIF'ler depo boyutunu hızla şişirir; eklemeden önce bir sıkıştırıcıdan (örn. `pngquant`, `gifsicle` veya çevrimiçi bir araç) geçirin.
- **Vektör tabanlı her şey için SVG tercih edin** (rozetler, ikonlar, diyagramlar) — sonsuz ölçeklenir, dosya boyutu küçüktür.
- **SVG'nin uygun olmadığı ekran görüntülerinde WebP veya optimize edilmiş PNG tercih edin.**
- **GIF'leri kısa ve döngüsel tutun**; daha uzun demolar için desteklenen yerlerde HTML5 video ile MP4/WebM düşünün.
- **Aşırı büyük görsellerin sayfaya hâkim olmasını önlemek için** HTML `<img width="...">` ile açık bir genişlik belirleyin.
- **Büyük medyayı harici olarak barındırın** (veya Git LFS kullanın); ana deponun geçmişini ikili varlıklarla şişirmeyin.

---

## ♿ Erişilebilirlik

- **Her görsele anlamlı `alt` metni yazın** — `![image](...)` değil, `![Haftalık analitikleri gösteren uygulama panosu](...)`.
- **Durumu iletmek için yalnızca renge güvenmeyin** (örn. kırmızı rozeti sadece kırmızı bırakmak yerine "failing" kelimesiyle eşleştirin).
- **Animasyonlu içeriği isteğe bağlı hissettirin** — bir typing SVG veya snake animasyonu, düz metinde başka yerde bulunmayan bilgi taşımamalıdır.
- **Başlık hiyerarşisini koruyun** (`#` → `##` → `###` sırayla) ki ekran okuyucular belgede yapısal olarak gezinebilsin.
- **Rozet/banner metni ile arka planı arasında yeterli kontrastı sağlayın**, özellikle özel hex renklerle.
- **Açıklayıcı bağlantı metni kullanın** ("Kurulum rehberini görüntüle", "buraya tıkla" değil).

---

## 📱 Mobil Uyumluluk ve Karanlık Mod

- **Dar genişliklerde test edin.** Yan yana HTML tablo içindeki stats kartları mobilde kötü taşabilir — gerçek bir telefonda veya dar bir tarayıcı penceresinde doğrulayın.
- **Her iki GitHub temasında da okunaklı olmayan banner veya diyagramlar için** `prefers-color-scheme` ile `<picture>` kullanın.
- **Tipik bir masaüstü görüntü alanının %100'üne yakın sabit piksel genişliklerden kaçının**; yüzde tabanlı genişlikler daha zarif küçülür.
- **Rozet/banner metin kontrastını her iki temada da kontrol edin** — yalnızca koyu moda göre tasarlanmış bir banner açık modda okunmaz hale gelebilir ve tersi de geçerlidir.
- **Kritik içeriği yalnızca görsellerin içinde değil, metin olarak tutun**; çünkü bazı mobil istemciler Markdown görsellerini tutarsız render eder.

---

## 🔖 Rozet, Banner ve İkon Kullanımında Doğru Uygulamalar

- Belge başına bir rozet **stili** (flat-square, flat veya for-the-badge seçin ve ona bağlı kalın).
- Bir banner **şekil ailesi** — `waving` header ile `venom` footer'ı karıştırmayın.
- Rozetleri **amaca** göre gruplayın (durum, yığın, sosyal) ve gruplar arasında görsel ayrım bırakın.
- Yaklaşık hex değerleri yerine Simple Icons'tan **resmi marka renklerini** kullanın.
- Banner'ları **orantılı** tutun — okunacak kadar yüksek, sayfaya hâkim olmayacak kadar kısa.
- İkonlar, kullandığınız her aracın tarihsel bir kaydı değil, **güncel olarak ilgili** olmalıdır.

---

## 🎨 Yerleşim, Tipografi, Renk ve Boşluk

**Yerleşim:** İçeriği, en önemli bilginin kaydırmadan görülebileceği şekilde yapılandırın — ad/proje, tek satırlık açıklama ve birincil eylem çağrısı (kurulum komutu veya biyografi) ekranın üst kısmında olsun.

**Tipografi:** Markdown sınırlı tipografik kontrol sunar (başlıklar, kalın, italik). Başlık seviyelerini keyfi boyut değişiklikleri için değil, taranabilir bir hiyerarşi oluşturmak için bilinçli kullanın.

**Renk:** 2–3 temel renk (bir vurgu ve nötrler) seçin ve bunları rozetlerde, banner'larda ve stat-kart temalarında tutarlı biçimde uygulayın. Tutarlı, sınırlı bir palet, geniş ve birbiriyle ilgisiz bir renk yelpazesinden daha profesyonel okunur.

**Boşluk:** Bölümleri ayırmak için bölümler arasında boş satırlar bırakın ve uzun belgeleri bölmek için yatay çizgileri (`---`) idareli kullanın. Yoğun, kesintisiz metin, uzun README'lerde okunabilirliğin en büyük katilidir.

---

## 🚨 Sık Yapılan README Hataları

1. Projenin ya da kişinin gerçek bir açıklaması yerine rozetlerle başlamak.
2. Kurulum talimatı olmaması veya belgelenmemiş ön koşulları varsayan talimatlar.
3. Başlık, liste veya boşluk içermeyen bir metin duvarı.
4. Güncel arayüzle uyuşmayan eski ekran görüntüleri.
5. Kırık görsel bağlantıları (branch yeniden adlandırıldıktan veya varlıklar taşındıktan sonra yaygın).
6. Aynı belgede birden fazla rozet stilini karıştırmak.
7. Açık kaynak projede lisans bölümü olmaması.
8. Gerçek bir yönlendirme olmadan sadece "PR'lar hoş geldi" diyen bir "Katkıda Bulunma" bölümü.
9. Açıkça özelleştirilmemiş, kopyala-yapıştır şablon metni (geride kalan yer tutucu kuruluş/depo adları).
10. Kullanım örneğinin olmaması — aracın gerçekten çalıştığını gösteren hiçbir şey olmadan kurulum talimatları.
11. İçindekiler tablosu olmayan aşırı uzun README.
12. Kişisel siteye, eski Twitter hesabına veya kullanımdan kalkmış dokümantasyona ölü bağlantılar.
13. Görsellerde alt metin olmaması; erişilebilirliğe ve SEO'ya zarar verir.
14. Profesyonel tonu zayıflatan aşırı emoji kullanımı (bağlama bağlı, ama kontrol etmeye değer).
15. Tamamen rozet ve kartlardan oluşan, kişisel tek bir cümlesi olmayan profil README'si.
16. Belge boyunca tutarsız başlık büyük harf kullanımı veya biçimlendirme stili.
17. Tüm gerçek içeriği ekranın altına iten aşırı büyük banner görselleri.
18. Sayfa yüklemesini fark edilir biçimde yavaşlatacak kadar büyük GIF'ler.
19. Projenin gerçek dokümantasyon sitesinde de (ve orada daha güncel) bulunan bilgilerin tekrarı.
20. Bir portfolyo projesinde teknoloji yığınından hiç söz edilmemesi; ziyaretçiyi kodu karıştırmaya zorlar.
21. Yalnızca koyu modda test edildiği için GitHub'ın açık temasıyla ağır biçimde çakışan bir stats kartı teması.
22. Depo boyutunu şişiren sıkıştırılmamış ekran görüntülerini commit'lemek.
23. Büyük bir sürüm veya kırıcı API değişikliğinden sonra README'yi güncellemeyi unutmak.
24. Net bir eylem çağrısı olmaması (depoyu yıldızla, demoyu dene, dokümanı oku) — sonda.
25. Teknoloji yığını değiştikten sonra temizlenmemiş, artık kullanılmayan framework'leri gösteren rozet satırları.
26. Deponun en çok görüntülenen belgesinde yazım ve dilbilgisi hataları.
27. "Bunu nasıl kullanırım" sorusunu daha az önemli bilgilerin altına gömen bölüm sırası.
28. Somut teknik ayrıntısı olmayan, pazarlama metni gibi okunan bir README.
29. Belirgin olmayan araçlar için "bu proje neden var" açıklamasının eksikliği.
30. Proje durumuna dair bir belirti olmaması (aktif bakımda mı, arşivlenmiş mi, deneysel mi).

---

## ✅ README Kontrol Listesi

**İçerik**
- [ ] Proje adı ve tek satırlık açıklama görünen ilk şey
- [ ] Projenin çözdüğü amaç/problem açıklanmış
- [ ] Kurulum talimatları kopyalanıp yapıştırılabilir ve test edilmiş
- [ ] Minimal çalışan bir kullanım örneği eklenmiş
- [ ] Yapılandırma/seçenekler belgelenmiş veya bağlantı verilmiş
- [ ] Katkı yönergeleri mevcut (kısa bile olsa)
- [ ] Lisans belirtilmiş ve bir `LICENSE` dosyası mevcut
- [ ] Proje durumu (aktif/bakımda/arşivlenmiş) net
- [ ] İletişim veya destek kanalı listelenmiş

**Görsel Tasarım**
- [ ] Baştan sona tek ve tutarlı bir rozet stili kullanılmış
- [ ] Rozetler mantıksal olarak gruplanmış (durum / yığın / sosyal)
- [ ] Banner (varsa) orantılı, sayfaya hâkim değil
- [ ] Renk paleti sınırlı ve widget'lar arasında tutarlı
- [ ] Başlıklar mantıksal, sıralı bir hiyerarşi izliyor
- [ ] Bölümleri ayırmak için boşluk kullanılmış
- [ ] Uzun belgeler için içindekiler tablosu mevcut

**Teknik Doğruluk**
- [ ] Tüm bağlantılar çalışıyor (404 yok)
- [ ] Tüm görseller render ediliyor (kırık yol yok)
- [ ] Kod örnekleri yazıldığı gibi gerçekten çalışıyor
- [ ] Rozet URL'leri yer tutucu değerlere değil doğru kullanıcı adına/depoya işaret ediyor
- [ ] Ekran görüntüleri güncel arayüzü/sürümü yansıtıyor

**Erişilebilirlik ve Uyumluluk**
- [ ] Her görselde açıklayıcı alt metin var
- [ ] İçerik hem GitHub açık hem koyu temasında okunaklı
- [ ] Yerleşim mobil genişliklerde bozulmuyor
- [ ] Durum yalnızca renkle iletilmiyor
- [ ] Kritik bilgi yalnızca görsellerde/animasyonlarda değil, düz metinde de mevcut

**Performans ve Düzen**
- [ ] Görseller sıkıştırılmış
- [ ] Büyük medya uygun şekilde barındırılıyor (depo geçmişini şişirmiyor)
- [ ] Dinamik widget'lar (stats/streak kartları) test edilmiş ve düzgün yükleniyor
- [ ] Şablondan veya oluşturucudan kalma yer tutucu metin yok
- [ ] Yazım ve dilbilgisi kontrol edilmiş

**Profil README'sine Özel**
- [ ] Depo adı GitHub kullanıcı adıyla birebir eşleşiyor
- [ ] Depo public
- [ ] Biyografi yalnızca rozet değil, gerçek ve kişisel içerik barındırıyor
- [ ] Sosyal/iletişim bağlantıları doğru ve güncel
- [ ] Öne çıkan/sabitlenmiş projeler gerçekten en iyi temsil eden işler

**Bakım**
- [ ] Büyük değişikliklerden sonra README'yi yeniden gözden geçirmek için bir plan (gayriresmi bile olsa) var
- [ ] Zamanlanmış Action'lar (snake, WakaTime vb.) çalıştığı doğrulanmış

---

## 🧩 Kullanım Senaryosuna Göre Önerilen Araç Kombinasyonları

**Yeni Başlayanlar**
Shields.io rozetleri + capsule-render header. *Neden işe yarar:* ikisi de sıfır kurulumlu kopyala-yapıştır URL araçlarıdır; öğrenilecek yeni bir kavram olmadan hızlı ve gerçek bir iyileştirme sağlar.

**Öğrenciler**
capsule-render header + Shields.io yığın rozetleri + kısa bir "şu an öğreniyorum" bölümü. *Neden işe yarar:* köklü hesapları kayıran stats kartlarından çok, işe alımcılara gelişimi ve güncel odak alanlarını daha dürüstçe gösterir.

**Açık Kaynak Bakımcıları**
Shields.io derleme/sürüm/lisans rozetleri + net bir kurulum/kullanım bölümü. *Neden işe yarar:* bir proje README'sinin kitlesi önce işlevsel durum bilgisine ihtiyaç duyar — süs burada ikincildir.

**Portfolyo Profilleri**
capsule-render header + Readme Typing SVG sloganı + seçilmiş Simple Icons yığın satırı + 3–4 sabitlenmiş proje. *Neden işe yarar:* kimlikle ve dönüşümlü bir sloganla başlar, ardından dikkati istatistiklerin altına gömmek yerine doğrudan en güçlü işlere yönlendirir.

**Python Geliştiricileri**
Shields.io PyPI sürüm/indirme rozetleri + GitHub Readme Stats Top Languages (compact düzen). *Neden işe yarar:* PyPI'ye özgü rozetler, genel bir yığın rozetinin veremeyeceği gerçek ve anlamlı paket metrikleri verir.

**JavaScript/Node Geliştiricileri**
Shields.io npm sürüm/indirme rozetleri + Simple Icons yığın satırı (React/Node vb.). *Neden işe yarar:* npm rozetleri kendiliğinden güncellenir ve JS ekosisteminin kitlesi için hemen anlamlıdır.

**AI/ML Projeleri**
Model/veri seti lisansı, framework sürümü için Shields.io rozetleri + net bir "çıkarım nasıl çalıştırılır" kullanım bölümü. *Neden işe yarar:* AI projelerinin kurulum sürtünmesi alışılmadık derecede yüksektir; README'nin en değerli işi süsleme değil, bu sürtünmeyi en aza indirmektir.

**Web Geliştiricileri**
capsule-render header + erken bir demo GIF'i/ekran görüntüsü + canlı site rozeti/bağlantısı. *Neden işe yarar:* web işi doğası gereği görseldir — göstermek anlatmaktan iyidir.

**Oyun Geliştiricileri**
Özel banner (veya capsule-render) + gömülü oyun içi GIF + platform/motor rozetleri. *Neden işe yarar:* benzer şekilde görseldir; durağan bir ekran görüntüsü, kısa bir GIF'in verdiği oynanış hissini nadiren aktarır.

**Minimalistler**
Düz başlıklar, tek rozet satırı, banner yok, stats kartı yok. *Neden işe yarar:* ölçülülük kendi başına bir tasarım tercihidir ve temiz, metin öncelikli bir README bitmemiş değil, kendinden emin okunur.

**Gösterişli/Maksimalist Profiller**
capsule-render header + footer + Readme Typing SVG + GitHub Readme Stats + Streak Stats + seçilmiş ikon satırları, hepsi tek bir eşleşen temada. *Neden işe yarar:* etki yalnızca her öğe tek ve tutarlı bir temayı paylaştığında işe yarar — risk dağınıklıktır ve temaları eşleştirmek bunu önler.

---

## 🌟 Öne Çıkan README Örnekleri ve Koleksiyonlar

> [!NOTE]
> Uydurma bir liste vermek yerine, bu bölüm öne çıkan profil README'lerinin özenle derlenmiş, aktif olarak bakımı yapılan topluluk koleksiyonlarına işaret eder — "etkileyici" profiller trendler geliştikçe sürekli değiştiği için gerçekten güncel örneklere göz atmanın en iyi yolu budur.

| Kaynak | Bağlantı | Neden faydalı |
|---|---|---|
| awesome-github-profile-readme | https://github.com/abhisheknaiidu/awesome-github-profile-readme | Öne çıkan profil README'lerinin ve arkasındaki araçların geniş, aktif olarak derlenen bir listesi |
| awesome-github-profile-readme-templates | https://github.com/durgeshsamariya/awesome-github-profile-readme-templates | Birçok görsel stili kapsayan, uyarlamaya hazır şablonlar |
| creative-profile-readme | https://github.com/coderjojo/creative-profile-readme | Doğrudan ilham için bireysel geliştirici profillerinin dizini |
| awesome-github-profiles (EddieHub Community) | https://github.com/EddieHubCommunity/awesome-github-profiles | Pull request'lerle büyüyen, topluluğun gönderdiği profil vitrini |
| github-readme-stats | https://github.com/anuraghazra/github-readme-stats | Bakımcının kendi README'si, belgelediği widget'ın canlı örneği olarak da işler |
| readme-typing-svg | https://github.com/DenverCoder1/readme-typing-svg | Yazma efektini kendi dokümantasyonunda doğrudan gösterir |
| shields (rozetler) | https://github.com/badges/shields | Projenin kendi README'si rozet dokümantasyonu stili için güçlü bir referans |

Bireysel öne çıkan **profil** örnekleri için, yukarıdaki widget depolarının bakımcılarına ve en çok katkı verenlere göz atmak (kendi profilleri çoğu zaman geliştirdikleri araçları sergiler), kaçınılmaz olarak eskiyecek statik bir listeden ziyade gerçek, güncel ve yüksek kaliteli örnekleri görmenin en güvenilir yollarından biridir.

---

## 📦 Kaynaklar

**Resmi Dokümantasyon**
- GitHub Docs — Profil README'nizi yönetme: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- GitHub Flavored Markdown Spesifikasyonu: https://github.github.com/gfm/
- GitHub Docs — Temel yazma ve biçimlendirme söz dizimi: https://docs.github.com/en/get-started/writing-on-github

**Rozetler ve İkonlar**
- Shields.io: https://shields.io
- Simple Icons: https://simpleicons.org
- shieldcn (shadcn stilinde rozetler ve grafikler): https://shieldcn.dev

**Banner'lar ve Görsel Widget'lar**
- capsule-render: https://github.com/kyechan99/capsule-render
- Readme Typing SVG: https://github.com/DenverCoder1/readme-typing-svg

**İstatistik ve Etkinlik**
- GitHub Readme Stats: https://github.com/anuraghazra/github-readme-stats
- GitHub Readme Streak Stats: https://github.com/DenverCoder1/github-readme-streak-stats

**Oluşturucular ve Derlenmiş Listeler**
- GitHub Profile README Generator: https://rahuldkjain.github.io/gh-profile-readme-generator/
- awesome-github-profile-readme: https://github.com/abhisheknaiidu/awesome-github-profile-readme
- awesome-github-profile-readme-templates: https://github.com/durgeshsamariya/awesome-github-profile-readme-templates

**Markdown Editörleri ve Araçları**
- GitHub'ın yerleşik web editörü (canlı önizlemeyle)
- Commit'lemeden önce daha hızlı yineleme için kod editörünüzdeki herhangi bir yerel Markdown önizleme eklentisi

**Topluluklar**
- GitHub Community Discussions: https://github.com/orgs/community/discussions
- DEV Community (`#github`, `#markdown` etiketleri): https://dev.to

---

## ❓ Sıkça Sorulan Sorular

**S: Profil README'm profil sayfamda görünmüyor. Sorun ne?**
C: Sırayla kontrol edin: (1) depo adı kullanıcı adınızla birebir eşleşiyor mu, (2) depo public mi, (3) README dosyası var mı ve boş değil mi, (4) birden fazla hesabınız varsa doğru hesaba mı bakıyorsunuz.

**S: İyi bir README hazırlamak için HTML bilmem gerekir mi?**
C: Hayır — iyi README tasarımının büyük çoğunluğunu yalnızca Markdown kapsar. Az miktarda HTML (başlıca `<div align>`, `<details>` ve `<picture>`) geri kalanının kilidini açar.

**S: Çok sayıda rozet ve widget README'mi yavaşlatır veya performansa zarar verir mi?**
C: Her biri küçük, önbelleğe alınmış bir SVG isteğidir; makul bir sayı (bir düzine kadar) ihmal edilebilir etki yaratır. Aşırı fazlalık (onlarca büyük kart) özellikle mobilde gerçek yükleme süresi ekler.

**S: Depo README'si ve profil README'si aynı görünmeli mi?**
C: Hayır — depo README'sinin işi dokümantasyondur (kur, kullan, katkıda bulun); profil README'sinin işi kişisel tanıtımdır. Tasarım dilini yeniden kullanın (örneğin tutarlı rozet stili) ama yapıyı değil.

**S: README'mi ne sıklıkla güncellemeliyim?**
C: Depo README'leri her önemli özellikte veya kırıcı değişiklikte güncellenmelidir. Profil README'leri daha düşük riskli, ancak yığınınız veya odağınız değiştikçe birkaç ayda bir gözden geçirmeye değer.

**S: Dinamik istatistik kartları uzun vadede güvenilir mi?**
C: GitHub Readme Stats gibi iyi bakımlı topluluk projeleri için genellikle evet, ancak barındırılan her üçüncü taraf servis kesinti yaşayabilir — sıfır bakımlı, her zaman güncel veri karşılığında yapılan takas budur.

**S: Mevcut bir README'de yapabileceğim tek en etkili değişiklik nedir?**
C: Neredeyse her zaman: en üste net bir tek satırlık açıklama ve çalışan bir kullanım örneği eklemek. Görsel cila, bir ziyaretçinin projeyi ilk on saniyede anlayabilmesinden çok daha az önemlidir.

---

<div align="center">

<p align="center">
  <img src="docs/screenshots/footer-banner.png" alt="capsule-render ile oluşturulmuş footer banner" width="800">
</p>

README'leri sadece meşgul göstermek değil, gerçekten işe yarasın isteyen geliştiriciler için özenle hazırlandı.

</div>
