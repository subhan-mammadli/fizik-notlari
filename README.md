# Fizik → Elektronik → Bilgisayar Bilimi Notları

Elektroniğin ve bilgisayar bilimlerinin altında yatan fiziği, sıfırdan ve sade bir dille anlatan kişisel çalışma notları.

Bu notlar; yapay zekâ ile birlikte yürüttüğüm **self-study** sürecinde, konuları gerçekten anlamak için tutuldu. Formül ezberi yerine "bu şey neden böyle davranıyor?" sorusuna cevap arıyor: enerjiden başlayıp atomik yapıya, oradan manyetizmaya, oradan da diyot, transistör ve MOSFET'e kadar uzanan tek bir zincir kuruyor.

## Öğrenme Yolu

Notlar numaralandırılmış iki ana bölümden oluşuyor. Sırayla okunacak şekilde tasarlandı:

1. **Temel Konular (01–11):** Fiziksel temeller — enerji, elektromanyetizma, madde, ısı, manyetizma, Ohm kanunu, AC/DC.
2. **Temel Komponentler (12–19):** Bu temellerin devre elemanlarına ve yarı iletkenlere dönüşmesi — kondansatör, bobin, motor/jeneratör, direnç, bant teorisi, doping, diyot, transistör, MOSFET.

## İçindekiler

### Temel Konular

| # | Not | Ne anlatıyor? |
|---|-----|---------------|
| 01 | [Elektromanyetik Kuvvet](Temel%20Konular/01%20-%20Elektromanyetik%20Kuvvet.md) | Enerji, elektromanyetik kuvvet, foton, elektrik, çekirdek, güçlü nükleer kuvvet |
| 02 | [Molekül](Temel%20Konular/02%20-%20Molekul.md) | Atomlar arası bağlar, su molekülü, moleküllerin birleşmesi |
| 03 | [Isı ve Sıcaklık](Temel%20Konular/03%20-%20Isı%20ve%20Sıcaklık.md) | Sıcaklık, kıvılcım, soğuk ve donma |
| 04 | [Agregat Hal](Temel%20Konular/04%20-%20Agregat%20Hal.md) | Katı, sıvı, gaz ve plazma halleri |
| 05 | [Maddeler](Temel%20Konular/05%20-%20Maddeler.md) | İletkenler/yalıtkanlar, iletim, sertlik, kovalent bağlar, erime |
| 06 | [Manyetizma](Temel%20Konular/06%20-%20Manyetizma.md) | Spin, orbital, mıknatıslık, elektromıknatıs, sağ el metodu |
| 07 | [Ohm Kanunu](Temel%20Konular/07%20-%20Ohm%20Kanunu.md) | Gerilim, akım, direnç, birim çevirmeleri, güç |
| 08 | [AC ve DC](Temel%20Konular/08%20-%20AC%20ve%20DC.md) | Doğru/alternatif akım, trafo, şebekeden prize yolculuk, AC→DC |
| 09 | [Açık ve Kapalı Devre](Temel%20Konular/09%20-%20Açık%20ve%20Kapalı%20Devre.md) | Devre kavramı ve akımın dolaşması |
| 10 | [Referans Noktası (GND)](Temel%20Konular/10%20-%20Referans%20Noktası%28GND%29.md) | Toprak/ground ve referans gerilimi |
| 11 | [Seri ve Paralel Bağlantı](Temel%20Konular/11%20-%20Seri%20ve%20Paralel%20Bağlantı.md) | Dirençlerin seri/paralel davranışı |

### Temel Komponentler

| # | Not | Ne anlatıyor? |
|---|-----|---------------|
| 12 | [Kondansatör](Temel%20Komponentler/12%20-%20Kondensatör.md) | Yük depolama, şarj/deşarj, ne zaman kullanılır |
| 13 | [İndüktör (Bobin)](Temel%20Komponentler/13%20-%20İndüktör.md) | Manyetik alanda enerji depolama, kullanım alanları |
| 13.1 | [Motor](Temel%20Komponentler/13.1%20-%20Motor.md) | Dönme kuvveti, komütatör, fırçalar, hız/yön kontrolü |
| 13.2 | [Jeneratör](Temel%20Komponentler/13.2%20-%20Jeneratör.md) | Hareketten gerilim üretimi, motor–jeneratör ilişkisi |
| 14 | [Rezistör](Temel%20Komponentler/14%20-%20Rezistör.md) | Direnç, pull-up/pull-down, değer seçimi |
| 15 | [Bant Teorisi](Temel%20Komponentler/15%20-%20Bant%20Teorisi.md) | Bant yapısı, iletken/yasıtkan/yarı iletken |
| 16 | [Doping](Temel%20Komponentler/16%20-%20Doping.md) | N-tipi ve P-tipi yarı iletkenler |
| 17 | [Diyot](Temel%20Komponentler/17%20-%20Diyot.md) | PN eklemi, tek yönlü kapı, doğrultma, LED, test |
| 18 | [Transistör](Temel%20Komponentler/18%20-%20Transistör.md) | NPN yapısı, beyz kontrolü, anahtarlama ve yükseltme |
| 19 | [MOSFET](Temel%20Komponentler/19%20-%20MOSFET.md) | Gate kontrolü, kanal genişliği, gerçek devre ve test |

## Nasıl Okunur?

**GitHub üzerinde:** Yukarıdaki bağlantılardan doğrudan okuyabilirsin. Notlar düz Markdown olduğu için herhangi bir Markdown görüntüleyicide açılır.

**Obsidian ile (önerilen):** Repoyu klonla ve klasörü Obsidian'da aç:

```bash
git clone https://github.com/<kullanici-adin>/fizik-notlari.git
```

Obsidian ayarları ve kullanılan tema (`Nord-i Hümâyûn`) repoda hazır geliyor; ekstra kurulum gerekmez.

## Notların Yaklaşımı

- **Somut benzetmeler:** Elektronlar, duvarlar, kalabalık odalar, su boruları… Soyut kavramlar gündelik hayattan örneklerle anlatılıyor.
- **Kademeli inşa:** Her not, önceki notun üzerine kuruluyor. Diyot notu, doping ve bant teorisini bilmeden tam oturmuyor.
- **Pratik bağlantı:** Teori bitince "tamir masasında bunu nasıl ölçersin?", "hangi durumda bu komponenti kullanırsın?" gibi kısımlar geliyor.

## Bilinen Eksikler

Bazı notlardaki el çizimi/şema görselleri orijinal arşivde bulunamadığı için ilgili yerlerde "Görsel arşivde bulunamadı" notu görünebilir. Bu görseller tamamlandıkça repoya eklenecek.

## Lisans

Kişisel öğrenme notlarıdır; alıntı ve kullanım için kaynak belirtmen yeterli.
