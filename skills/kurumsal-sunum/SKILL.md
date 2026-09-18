---
name: kurumsal-sunum
description: Türk kurumsal dünyasında üst yönetime, yönetim kuruluna, direktöre veya müdüre sunulacak sonuç odaklı yönetim sunumları hazırlar. Kullanıcı "yönetici sunumu", "yönetime sunum", "yönetim kurulu sunumu", "proje sunumu", "durum sunumu", "bütçe/yatırım sunumu", "sunum hazırla", "slayt hazırla", "PowerPoint", "pptx" dediğinde veya bir doküman, rapor, analiz ya da notu yönetime sunulacak hale getirmek istediğinde bu skill'i mutlaka kullan; kullanıcı "sunum" kelimesini kullanmasa bile içeriğin bir yöneticiye anlatılacağı belliyse yine kullan. Bu skill içeriği, slayt akışını ve üslubu belirler; pptx dosyasını üretmek için resmi pptx skill'ini kullanır.
---

# Kurumsal Sunum

## Bu skill neden var

Claude'a "yönetici sunumu yap" dendiğinde çıkan sunum genellikle iki hata yapar:

1. Genel geçer olur. Şirket adını değiştirsen aynı sunum başka bir şirkete de gider. Yöneticiler bunu ilk bakışta fark eder ve sunumu ciddiye almaz.
2. Sonucu sona saklar. Önce arka plan, sonra yöntem, en sonda bulgu. Türkiye'deki yöneticiler tam tersini ister: önce sonuç, sonra isterse gerekçe.

Bu skill'in tek amacı bu iki hatayı yaptırmamak. Sunum "sonuç önce, somut, kısa" olur.

## Adım 1: Eksik bilgiyi tamamla

Kullanıcı vermediyse aşağıdakileri sor. Vermişse sorma, doğrudan devam et. Sorular tek mesajda, kısa olsun.

- **Kime sunulacak?** (genel müdür, direktör, yönetim kurulu, birim müdürü, müşteri). Kitle yükseldikçe slayt azalır, rakam büyür.
- **Sunumun sonunda yöneticiden ne bekleniyor?** (onay, bütçe, karar, sadece bilgilendirme). Bu cevap ikinci slaytı belirler.
- **Kaç dakika?** 10 dakika için en fazla 6-8 slayt, 20 dakika için 10-12. Fazlası ek bölümüne gider.
- **Kurumsal renk / şablon var mı?** Varsa onu kullan. Yoksa nötr, açık zeminli bir palet seç. Mavi veya lacivert varsayılan zemin kullanma; bu "hazır şablon" görüntüsü verir.

Kullanıcı elinde doküman, rapor, Excel veya not verdiyse sunumu o kaynaktan çıkar; kaynakta olmayan rakam veya iddia uydurma.

**Şirkete özgü rakam iste.** Genel bir konu (mevzuat, sektör trendi, yeni teknoloji) sunuluyorsa, sunumu bu şirkete bağlayacak 2-3 iç rakam veya olgu iste: "portföyünüzde kaç proje var", "geçen yıl bu kalemde ne harcandı", "hangi birim etkileniyor". Kullanıcı vermezse ilgili yere köşeli parantezle yer tutucu koy ("[tamamlanmış proje sayısı]") ve teslimde bunu söyle. Uydurma rakam koyma.

## Adım 2: Önce slayt planı, sonra dosya

Dosyayı üretmeden önce slayt planını göster: her slayt için tek satır, "slayt başlığı (bulgu cümlesi) + görsel türü". Kullanıcı onaylayınca üret. Bu adım kullanıcıya 30 saniyeye mal olur ama yanlış sunumu baştan yapmaktan kurtarır.

Plan formatı:

```
1. Kapak: [Sunum adı, tarih, sunan]
2. Sonuç: [Tek cümle sonuç + istenen karar]
3. [Bulgu cümlesi] - [grafik / tek rakam / tablo / akış]
...
N. Talep ve sonraki adımlar
Ek: [varsa]
```

## Adım 3: Sunum akışı

Sıra sabittir; slayt sayısı süreye göre değişir.

1. **Kapak** (isteğe bağlı). Kullanıcı istemezse atla, sunum doğrudan sonuçla başlasın.
2. **Sonuç ve talep.** Tek cümle sonuç, altında yöneticiden istenen şey. Yönetici sadece bu slaytı görse sunumu anlamış olmalı. Bu slayt asla atlanmaz.
3. **Neden şimdi.** Durum, sorun veya fırsat. Bir slayt, en fazla iki.
4. **Ne yaptık / ne öneriyoruz.** Yöntem değil, yapılan iş ve öneri. Süreç ayrıntısı ek'e gider.
5. **Rakamlar ve etki.** Maliyet, tasarruf, süre, oran. Her rakamın kaynağı ve tarihi slaytta küçük yazıyla bulunur.
6. **Riskler ve önlemler.** En fazla 3 risk, her birinin karşısında önlem.
7. **Talep ve sonraki adımlar.** Kim, ne, ne zamana kadar. Son slayt "Teşekkürler" değildir; yöneticinin karar vereceği slayttır.
8. **Ekler.** Ayrıntılı tablolar, yöntem, varsayımlar. Sunumda anlatılmaz, soru gelirse açılır.

## Slayt kuralları

Görünüm ve yerleşim kuralları [referans/tasarim-kurallari.md](referans/tasarim-kurallari.md) dosyasında; dosyayı üretmeden önce oku. Aşağıdakiler içerik kurallarıdır.

- **Slayt başına tek mesaj.** İki şey anlatacaksan iki slayt yap.
- **Başlık bir bulgu cümlesidir, konu başlığı değil.** "Kayıp kaçak oranı" değil, "Kayıp kaçak oranı 3 yılda 2 puan düştü".
- **Metin sınırı: slayt başına en fazla 30 kelime.** Aşıyorsan slayt yanlış kurulmuştur; grafik, tek büyük rakam, tablo veya akış şemasına çevir. Slaytta paragraf olmaz.
- **Görsel önce.** Rakam varsa grafik, karşılaştırma varsa tablo, süreç varsa akış. Süs görsel (stok fotoğraf, dekoratif ikon) kullanma.
- **Ölçüsüz ifade yok.** "Önemli ölçüde", "ciddi artış", "yaklaşık" yerine rakam. Rakam yoksa cümle de yok.
- **Renk:** kullanıcının verdiği kurumsal renk ana vurgu rengidir, zemin açık ve sade. Mavi/lacivert varsayılana düşme.

## Genel geçer testi

Dosyayı üretmeden önce her slayta şu soruyu sor: **"Şirket adını değiştirsem bu slayt başka bir şirkete de gider mi?"** Cevap evetse slayt genel geçerdir; içine bu şirkete, bu projeye, bu döneme özgü bir rakam, isim, tarih veya karar koy ya da slaytı sil.

Genel geçer slayt örnekleri (yapma):
- "Dijital dönüşüm günümüzde kaçınılmazdır"
- "Verimlilik artışı hedefliyoruz"
- Sektör tanımı yapan giriş slaytları

Somut slayt örnekleri (yap):
- "Pilot bölgede arıza süresi 47 dakikadan 31 dakikaya indi (Ocak-Haziran 2026)"
- "Yatırım 3,2 milyon TL, geri dönüş 22 ay"

## Dil ve üslup

Yapay zeka kokan ifadeleri temizleme kalıpları [referans/yazim-kurallari.md](referans/yazim-kurallari.md) dosyasında; slayt planı onaylandıktan sonra, dosya üretilmeden önce tüm metinleri o dosyadaki kalıplara karşı tara. Temel kurallar:

- Sade Türkçe. İngilizce kurumsal jargon yerine Türkçe karşılığı ("roadmap" değil "yol haritası", "KPI" yerine "performans göstergesi"; ancak kurumda yerleşik kısaltmalar varsa onları koru).
- Uzun çizgi (em dash) kullanma, normal kısa çizgi veya virgül kullan.
- Şapkalı a kullanma ("hala", "zeka" şeklinde yaz).
- Edilgen ve dolambaçlı cümle yerine özneli, kısa cümle: "Tasarruf sağlanmıştır" değil, "Ekip 1,1 milyon TL tasarruf sağladı".
- Yöneticiye ders verme, öneri sun. "Yapılmalıdır" yerine "öneriyoruz".

## Dosya üretimi

İçerik planı onaylanıp metinler yazım kurallarından geçtikten sonra pptx dosyasını resmi pptx skill'i ile üret; görünümü referans/tasarim-kurallari.md belirler (renk, yazı boyutu, altı slayt tipi, yapma listesi). Bu skill dosya üretme mantığı içermez; sadece ne yazılacağını, nasıl sıralanacağını ve nasıl görüneceğini belirler. Slayt notlarına (speaker notes) her slayt için 2-3 cümlelik konuşma metni ekle; kullanıcı sunarken oradan bakar.

## Teslim öncesi kontrol listesi

Dosyayı vermeden önce kontrol et; bir madde tutmuyorsa düzelt.

- [ ] İkinci slayt (veya kapak yoksa ilk slayt) tek cümlede sonuç ve talebi veriyor
- [ ] Her slayt başlığı bir bulgu cümlesi
- [ ] Hiçbir slaytta 30 kelimeden fazla metin yok
- [ ] Her rakamın kaynağı ve tarihi var
- [ ] "Genel geçer testi"nden geçmeyen slayt yok
- [ ] Son slayt karar/aksiyon slaytı, "Teşekkürler" değil
- [ ] Slayt sayısı süreye uygun, fazlası ek bölümünde
- [ ] Mavi/lacivert varsayılan zemin yok
- [ ] Uzun çizgi ve şapkalı a yok
- [ ] Metinler referans/yazim-kurallari.md kalıplarından temizlendi
- [ ] Slaytlar görüntüye çevrilip referans/tasarim-kurallari.md görsel kontrolünden geçti
- [ ] Şirkete özgü rakam yoksa yer tutucu var ve kullanıcıya söylendi

## Örnek istekler

- "Elimdeki bu 20 sayfalık proje raporunu genel müdüre 10 dakikalık sunum yap"
- "Yeni yatırım için direktörden onay alacağım, sunumu hazırla, kurumsal rengimiz turuncu"
- "Bu Excel'deki aylık verileri yönetim kurulu için 8 slayta çevir"
- "Pilot proje sonuçlarını üst yönetime sunacağım, karar istiyoruz"
