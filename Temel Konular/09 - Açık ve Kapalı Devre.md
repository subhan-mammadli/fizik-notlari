
# Açık ve Kapalı Devre

Elektronik tamiri yaparken veya bir bilgisayar kartına bakarken aslında sürekli aradığımız şey budur: _"Yol tam mı, kopuk mu?"_

En sade, su gibi berrak bir benzetmeyle **Açık Devre** ve **Kapalı Devre** masalını açalım.
### Elektriğin Altın Kuralı: "Çember (Döngü) Olmak Zunda!"

Önceki derslerden hatırlasana: Pilin eksi kutbunda elektronlar sıkışmıştı, artı kutup ise onları çekmek istiyordu. Elektronların amacı neydi? Eksi odadan çıkıp artı odaya ulaşmak.

İşte doğanın en katı kuralı şudur: **Elektronlar asla çıkmaz sokaklara girmezler.** Onların akabilmesi, enerjini konuşturabilmesi ve iş (Watt) üretebilmesi için eksi kutuptan çıkıp **hiç kesintisiz bir yoldan dolaşarak tekrar artı kutba geri dönmesi gerekir.**

İşte bu kesintisiz dönüş yoluna **"Devre"** denir.
### 1. Kapalı Devre (Closed Circuit): "Yol Tamam, Hayat Var!"

Kapalı kelimesi insanı yanıltmasın; buradaki "kapalı", bir şeyin kilitli olması değil, **yolun başının sonunun birleşmiş, çemberin tamamlanmış olması** demektir.

- **Nasıl Çalışır?** Pilin eksi kutbundan kablo çıkar; lambaya (veya cihaza) gider, lambanın içinden geçer ve diğer kabloyla pilin artı kutbuna kusursuz bir şekilde bağlanır. Ortada hiçbir kopukluk yoktur.

- **Elektronlar Ne Yapar?** Yolun açık (kesintisiz) olduğunu gören o milyarlarca elektron ordusu, eksi kutuptan coşkuyla fırlar. Kablodan akar, lambanın o dirençli tellerinden geçerken sürtünür, enerjisini ısıya ve ışığa dönüştürür (lamba yanar) ve yoluna devam edip artı kutba ulaşır. Döngü hiç durmadan devam eder.

- **Pratik Örnek:** Duvardaki lambanın düğmesine basıp ışığı yaktığın an, oda aydınlanır çünkü o an **kapalı bir devre** kurmuşsundur.
### 2. Açık Devre (Open Circuit): "Yol Kopuk, Hayat Durdu!"

Açık devre ise yine adıyla çelişir; buradaki "açık", **yolun açık (serbest) olması değil, ortada bir kesik, bir kopukluk olması** demektir.

- **Nasıl Çalışır?** Kablolardan biri ortadan kesilmiştir, araya plastik girmiştir ya da anahtar "kapalı" (off) konumdadır. Eksi kutuptan çıkan elektronlar ilerler, ancak yolun ortasında bir **uçurum (boşluk)** ile karşılaşır.

- **Elektronlar Ne Yapar?** O boşlukta hava vardır. Hava ise mükemmel bir yalıtkandır (elektronları iletmez). Elektronlar o uçurumdan karşı tarafa atlayamaz. Yolu bulamayınca ne olur? **Akış aniden durur.**

- **Sonuç:** Voltaj (itme basıncı) hâlâ pilin içinde durmaktadır ama ortada akan bir akım (Amper) olmadığı için hiçbir şey çalışmaz. Lamba yanmaz, cihaz tepki vermez.

- **Pratik Örnek:** Cihazın fişini prizden çektiğinde veya odanın lambasının anahtarına basıp söndürdüğünde aslında yaptığın şey **açık devre** yaratmaktır. Yolu ortadan kesersin, akış durur.

### Su Pompası ve Hortum Benzetmesiyle Canlandıralım

Bunu kafanda yüzde yüz netleştirmek için bir su motoru düşün:

1. **Kapalı Devre:** Su motoru suyu çeker, hortumdan dolaştırıp tekrar motorun deposuna geri gönderir. Su sürekli devir daim yapar, sistem çalışır.

2. **Açık Devre:** Hortumu tam ortasından makasla kesip iki ucunu birbirinden ayırırsın. Motor suyu pompalamaya çalışır ama su boşa dökülür, devir daim tamamlanmaz. Sistem iş yapamaz hale gelir.
### Elektronik Tamircisinin Gözüyle: "Açık Devre" Arızası

Hobi olarak elektronik tamiriyle uğraştığın için bu kısım senin hayatını kurtaracak:

Bir bilgisayar anakartı veya lamba eline geldiğinde ve "çalışmıyor" dediğinde, ustaların yaptığı ilk iş multimetre ile **"Devre bütünlüğünü (Continuity)"** ölçmektir.

- Kartın üzerindeki o bakır yollardan (trace) biri darbe almış, çatlamış veya yanmış olabilir.

- Bakır yol koptuğu an, orada görünmez bir **açık devre** oluşmuştur.

- Sen oraya lehimle mini bir köprü atıp o kopuk yolu birleştirdiğinde, tekrar **kapalı devre** kurarsın ve cihaz sihirli bir şekilde çalışmaya başlar! Tamir dediğimiz şeyin yüzde ellisi aslında bu kopuk yolları (açık devreleri) bulup kapatmaktan ibarettir.
### Bonus: Kısa Devre (Short Circuit) Nedir?

Tamir masasında en çok korkulan şeylerden biri de **Kısa Devre**dir. Onu da kısaca aradan çıkaralım:

Normalde elektrik eksi kutuptan çıkıp cihazın içindeki dirençli yerlerden (lamba, işlemci vb.) geçerek iş yapmak zorundadır.

- Ama bazen kabloların yalıtkanlığı bozulur ve artı ile eksi kablo ortada hiçbir dirençle karşılaşmadan **direkt birbirine değiverir.**

- Elektronlar "Harika, hiç yokuş çıkmadan, dirençle uğraşmadan en kestirme yoldan hop diye karşı tarafa geçiyoruz!" derler.

- Direnç sıfıra yakın olduğu için Ohm Kanununa ($I = V / R$) göre **Amper (akım) tavan yapar!** Saniyeler içinde o kablodan devasa bir elektron kalabalığı geçer, kablo kıpkırmızı kesilir, erir ve cihazdan dumanlar yükselir. Kısa devre budur.
