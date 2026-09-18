# Kurumsal AI Skills

Beyaz yakalı profesyoneller için Türkçe Claude skill'leri. Amaç basit: Claude'a "yönetime sunum hazırla" dediğinizde çıkan şey Amerikan startup şablonu değil, Türk kurumsal dünyasında bir yöneticinin ciddiye alacağı bir sunum olsun.

Skill nedir? Claude'a belirli bir işi nasıl yapacağını anlatan bir talimat dosyası. Bir kez kurarsınız, ilgili istek geldiğinde Claude kendiliğinden devreye sokar. Kod bilmenize gerek yok.

## Skill'ler

| Skill | Ne yapar | Durum |
|---|---|---|
| `kurumsal-sunum` | Üst yönetime, direktöre veya müdüre sunulacak 8-12 slaytlık sonuç odaklı yönetim sunumu hazırlar. Slayt planını önce gösterir, onaydan sonra pptx üretir. | Hazır |
| `yonetici-ozeti` | Uzun bir doküman, mevzuat metni veya analizden tek sayfalık yönetici özeti çıkarır. | Yakında |
| `haftalik-durum-raporu` | Bir birimin haftalık ilerleme raporunu üretir. | Yakında |

### kurumsal-sunum ne yapıyor

- Sonuç önce: ikinci slayt tek cümlede sonucu ve yöneticiden istenen kararı verir. Yönetici sadece o slaytı görse sunumu anlamış olur.
- Genel geçer testi: her slayta "şirket adını değiştirsem bu slayt başka şirkete gider mi?" sorusunu sorar. Evetse slayt somutlaşır ya da silinir.
- Slayt başına tek mesaj, en fazla 30 kelime, başlıklar bulgu cümlesi.
- Yapay zeka kokan ifadeleri temizler (`referans/yazim-kurallari.md`): "kritik bir dönüm noktası", "-erek katkı sunmaktadır", üçlü sıfat listeleri, bürokratik edilgen çatı.
- Tasarım sistemi (`referans/tasarim-kurallari.md`): kurumsal renginiz ana renk, beyaz zemin, altı slayt tipi, "yapma" listesi. Mavi/lacivert varsayılan yok.
- Her slayta konuşma notu ekler.

## Kurulum

### claude.ai (kod bilmeyenler için önerilen yol)

1. Bu repodan `skills/kurumsal-sunum` klasörünü zip olarak indirin (veya Releases bölümündeki `.skill` dosyasını).
2. claude.ai'de Ayarlar > Yetenekler (Capabilities) > Skills bölümüne gidin.
3. Dosyayı yükleyin. Bundan sonra "yönetici sunumu hazırla" dediğiniz her sohbette skill devreye girer.

### Claude Code

```
/plugin marketplace add guvenser09-png/kurumsal-ai-skills
/plugin install kurumsal-ai-skills@kurumsal-ai-skills
```

Alternatif: `skills/kurumsal-sunum` klasörünü `~/.claude/skills/` altına kopyalayın.

### Cowork

`skills/kurumsal-sunum` klasörünü Cowork'ün skill klasörüne kopyalayın; klasör yapısı aynıdır.

## Örnek istekler

- "Elimdeki bu 20 sayfalık proje raporunu genel müdüre 10 dakikalık sunum yap"
- "Yeni yatırım için direktörden onay alacağım, sunumu hazırla, kurumsal rengimiz turuncu"
- "Bu Excel'deki aylık verileri yönetim kurulu için 8 slayta çevir"
- "Şu mevzuat değişikliğini yönetime sunacağım, karar istiyoruz"

## Nasıl çalışır

1. Claude eksik bilgiyi sorar: kime sunulacak, ne karar isteniyor, kaç dakika, kurumsal renk.
2. Slayt planını gösterir; siz onaylarsınız.
3. Metinleri yazım kurallarından geçirir, tasarım kurallarına göre pptx üretir.
4. Teslim öncesi kontrol listesini uygular.

## Katkı

Bir slaytın iyi ya da kötü çıktığını gördüyseniz issue açın; hangi kuralın eksik olduğunu birlikte bulalım. Yeni skill önerileri de issue olarak gelsin.

## Lisans

MIT
