# Transistör

Diyotta iki parçamız vardı: N ve P. Şimdi **üç parça** var. Bu bölümde sadece bu üç parçayı tanıyacağız ve yapıştırınca ne olduğuna bakacağız. **Pil yok, bağlantı yok.** Pili sonraki adımda bağlayacağız.

# NPN Transistör: Parçalar ve Yapıştırma

## 1. Üç parçayı tanıyalım

Üç parçanın hepsi silikon, hepsi nötr. Fark, içlerindeki kalabalıkta.

**Sol parça: Emiter (N-tipi).** Çok kalabalık bir şehir. İçinde dolup taşan serbest elektronlar var. Adı "salan, yayan" demek, çünkü elektron kaynağı olacak.

**Orta parça: Beyz (P-tipi).** İnce, neredeyse boş, küçük bir sokak. İçinde serbest elektron yok, sadece birkaç boşluk (boş bağ) var. Hem **çok ince** hem de **çok az boşluklu.** Bunu aklında tut, sonraki adımlarda en önemli şey bu olacak.

**Sağ parça: Kollektör (N-tipi).** O da bir şehir, içinde serbest elektronlar var ama emiter kadar kalabalık değil. Adı "toplayan" demek.

Üçünü yan yana koyuyoruz: **N - P - N.** Bir sandviç, ortası ince peynir.

## 2. Önce soldaki sınırı yapıştıralım

Emiter ile beyz yan yana geliyor. Diyot hikâyesinin aynısı:

- Emiter tarafı kalabalık, beyz tarafı boş. Kalabalık taraf kendiliğinden boş tarafa yayılmak ister.
- Sınıra yakın emiter elektronları beyze geçiyor.
- Beyze girince karşılarında boş bağlar (boşluklar) buluyorlar ve içlerine düşüyorlar. Elektron da boşluk da ortadan kalkıyor.

Şimdi geride ne kaldığına bakalım. Bu yeri diyotta yanlış anlamıştın, o yüzden yavaş gidelim:

- **Emiter tarafında:** Elektronunu veren atomlar yerlerinde duruyor (kristale bağlılar, kaçamazlar). Elektronları gitti, protonları kaldı. Bu atomlar artık **artı yüklü.**
- **Beyz tarafında:** Elektron alan atomlar da yerinde duruyor. Elektron fazlası var. Bu atomlar artık **eksi yüklü.**

Yani sınırın emiter tarafında sabit artılar, beyz tarafında sabit eksiler birikti. İşte bu, **ilk duvar.**

Neden duruyor? Duvardaki eksi yükler, emiterden gelmeye çalışan yeni elektronları geri itiyor (eksi eksiyi iter). Kısa süre sonra geçiş kendiliğinden duruyor.

## 3. Şimdi sağdaki sınırı yapıştıralım

Beyz ile kollektör yan yana. Aynı hikâye, bu sefer ayna görüntüsü:

- Kollektördeki serbest elektronlar sınıra yakın yerde beyze geçiyor.
- Beyzdeki boşluklara düşüyorlar.
- Kollektör tarafında elektron kaybeden atomlar **artı yüklü** kalıyor.
- Beyz tarafında elektron alan atomlar **eksi yüklü** oluyor.

Bu da **ikinci duvar.** Burada da beyz tarafındaki eksiler, kollektörden gelmeye çalışan elektronları geri itiyor.

## 4. Sonuç: Manzara

Yan yana yazarsak:

```
EMİTER (N)        BEYZ (P)        KOLLEKTÖR (N)
çok elektron      ince, az boşluk  orta elektron

      [ + | − ]  1. duvar        [ − | + ]  2. duvar
```

İki duvarın ortasında, beyzin içinde, çok dar bir şerit kalıyor. Bu şerit o kadar ince ki iki duvar neredeyse birbirine değiyor. Bu, beyzin çok ince yapılmasının sonucu.

## 5. Şu an elektronlar ne yapıyor?

- Emiterdeki elektronlar kendi şehirlerinde duruyor. Beyze gitmek isteseler karşılarında eksi yüklü duvar var, geri itiliyorlar.
- Kollektördeki elektronlar da aynı durumda. Beyze gitmek isteseler yine eksi yüklü duvar var, geri itiliyorlar.
- Beyz ortada, kendi dar sokağında, iki duvarın arasında sıkışmış.

Hiçbir yerde net bir akış yok. İki duvar da kapalı. Transistör pil olmadan kendi kendine dengeye oturmuş, uyuyor.

## Özet

- Üç parça: **Emiter** (çok kalabalık N), **Beyz** (ince, az boşluklu P), **Kollektör** (orta kalabalık N).
- İki sınır var, ikisinde de diyottaki hikâye yaşanıyor: elektronlar karşıya geçip boşluklara düşüyor.
- Geride sabit yüklü atomlar kalıyor ve **iki duvar** oluşuyor.
- Beyz çok ince olduğu için iki duvar birbirine çok yakın.
- Pil yokken elektronlar iki duvar arasında hapsolmuş, akım yok.

# NPN Transistör: Pili Bağlayalım (Beyz Boşta)

Önceki adımda üç parçayı yapıştırmış, iki duvar kurmuştuk. Pil yoktu, elektronlar iki duvarın arasında uyuyordu. Şimdi pili bağlıyoruz ve duvarlara ne olduğuna bakıyoruz.

## 1. Pili nasıl bağlıyoruz?

- Pilin **eksisi** emitere.
- Pilin **artısı** kollektöre.
- **Beyz** bacağı hiçbir yere bağlı değil, havada.

(Gerçek devrede kollektörün önünde bir yük olur, LED ya da motor gibi. Şimdilik hikâyeyi sade tutmak için yok sayıyoruz.)

```
(−) pil → EMİTER |1. duvar| BEYZ |2. duvar| KOLLEKTÖR ← (+) pil
                              (boşta)
```

## 2. Pil ne yapmak istiyor?

Pilin iki ucu iki şey söylüyor:

- **Eksi uç:** Emiterdeki elektronlara "ileri, beyze doğru" diye itiyor.
- **Artı uç:** Kollektördeki elektronları kendine çekiyor.

Pil, elektronların emiterden kollektöre doğru akmasını istiyor. Ama yolda iki duvar var. Sırayla bakalım.

## 3. Birinci duvar (emiter-beyz) ne yapıyor?

Hatırla, bu duvarın emiter tarafında sabit artılar, beyz tarafında sabit eksiler var. Emiterdeki elektron beyze geçmek isterse önünde eksi yükler görür ve geri itilir. Yani bu duvar emiter elektronları için bir **yokuş.**

Diyot dersinde duvarı yıkmanın yolunu görmüştük: N tarafı eksiye, **P tarafı artıya** bağlanmalıydı, ve gerilim yaklaşık 0,7 Volt olmalıydı. Şimdi durum ne? Emiter eksiye bağlı, ama P tarafı olan beyz **hiçbir yere bağlı değil.** Artıya bağlı olmadığı için duvarı yıkacak itme gelmiyor.

Bir şey daha var: iki duvar arka arkaya dizilmiş iki engel gibi. Direnç notundaki gerilim bölücüyü hatırla: seri engeller voltajı aralarında paylaşır ve en dirençli olan, voltajın büyük kısmını üstüne alır. Bu devrede en dirençli engel ikinci duvar (birazdan göreceğiz). Voltajın neredeyse tamamı oraya biner, birinci duvara yıkacak kadar itme kalmaz.

Sonuç: Emiter elektronları emiterde kalır.

## 4. İkinci duvar (beyz-kollektör) ne yapıyor?

Bu sınırı da diyot dersinden tanıyoruz. Pilin artısı kollektöre bağlı, yani **ters yön:** artı uç kollektördeki serbest elektronları kendine çekiyor, yani sınırdan **uzaklaştırıyor.**

Sınırdan çekilen elektronların yerinde yine sabit artı atomlar kalıyor. Boş (ölü) şerit genişliyor. Duvar **kalınlaşıyor.**

Kollektör elektronları da beyze geçemiyor. Bu kadar da değil, bir şey daha var, aklında tut:

- Bu duvarın beyz tarafı eksi, kollektör tarafı artı yüklü.
- **Kollektörden beyze** gitmeye çalışan bir elektron, eksiyi görür ve geri itilir: yokuş.
- **Beyzden kollektöre** gitmeye çalışan bir elektron ise artıyı görür ve çekilir: **kaydırak.** Üstüne kollektör pilin artısına bağlı, bu çekim daha da güçlü.

Şu an bu kaydırağın tepesinde, yani beyzde, geçecek elektron yok. Kaydırak hazır ama boş. Bunu unutma, bir sonraki adımda çok önemli olacak.

## 5. Sonuç: Kapalı

Elektronlar şu an şöyle duruyor:

- **Emiter şehri:** Pil itiyor ama birinci duvar durduruyor. Elektronlar bekliyor.
- **Beyz sokağı:** Boş, havada.
- **İkinci duvar:** Kalın ve hazır, ama ardında yokuş ve önünde boş bir kaydırak var.
- **Kollektör şehri:** Elektronların bir kısmı artıya doğru çekilmiş, duvar kalınlaşmış, sonra her şey durmuş.

Pil bağlı olduğu hâlde hiçbir yerden akım geçmiyor. Transistör **kapalı.**

## Özet

- Pilin eksisi emitere, artısı kollektöre bağlı. Beyz boşta.
- Birinci duvarı yıkmak için P tarafı (beyz) artıya bağlı olmalıydı, ama bağlı değil. Üstelik voltajın büyük kısmı ikinci duvara biniyor. Emiter elektronları geçemiyor.
- İkinci duvar ters yönde olduğu için kalınlaşıyor. Kollektör elektronları da geçemiyor.
- İkinci duvarın beyzden gelen elektronlar için bir **kaydırak** olduğunu unutma. Kaydırak hazır ama tepesinde kimse yok.
- Sonuç: akım yok, transistör kapalı.


# NPN Transistör: Beyzi Bağlayalım (Kolu Çevirmek)

Önceki adımda pili bağlamıştık ama beyz havada olduğu için transistör kapalıydı. Şimdi beyz bacağını bağlıyoruz, yani kolu çeviriyoruz.

## 1. Beyzi nasıl bağlıyoruz?

Beyz bacağını bir **direnç** üzerinden pilin **artısına** bağlıyoruz. (Direncin neden gerekli olduğunu bir sonraki adımda göreceğiz, şimdilik orada dursun.)

```
(−) pil → EMİTER |1. duvar| BEYZ |2. duvar| KOLLEKTÖR ← (+) pil
                              ↑
                       direnç üzerinden (+) pile bağlı
```

Bu bağlantıya diyot dersindeki gözle bak. Emiter (N) eksiye, beyz (P) artıya bağlı. Bu, diyodu **ileri yönde** bağlamakla aynı şey.

## 2. Birinci duvar yıkılıyor

Diyot dersinde bunu görmüştük: N tarafı eksiye, P tarafı artıya bağlanınca ve gerilim yaklaşık **0,7 Volt**'a çıkınca duvar çöker. Aynısı burada oluyor:

- Pilin eksisi emiterdeki elektronları sınıra doğru itiyor.
- Beyze bağlı artı uç, beyzdeki elektronları kendine çekiyor.
- İki taraftan gelen bu baskı birinci duvarı aşıyor ve duvar yıkılıyor.

Artık emiter elektronları beyze geçebilir.

## 3. Elektronlar beyze doluyor

Emiterdeki o kalabalık elektron topluluğu, duvar yıkıldığı için beyze akmaya başlıyor. Pilin eksisi arkadan itmeye devam ettiği için emiter hiç boşalmıyor, sürekli yeni elektron geliyor.

Burada diyottaki hikâyeyi hatırlayalım. Diyotta bu elektronlar P tarafına girince boşluklara düşüp bitiyordu. Burada ne oluyor? Bu sefer işler başka türlü gelişiyor.

## 4. Beyzde ne oluyor?

Beyzin iki özelliğini hatırla: **çok ince** ve **çok az boşluklu.**

Beyze giren elektronların önünde iki ihtimal var:

- **Boşluğa düşmek:** Ama boşluk çok az, düşebilecekleri delik sınırlı.
- **Karşı tarafa varmak:** Beyz o kadar ince ki karşı tarafa varmak için kat edecekleri yol çok kısa.

Köprü benzetmesiyle: kısa bir köprü var, üzerinde birkaç çukur. Köprüye giren kalabalığın çoğu çukurlara düşmeden köprüyü koşarak geçer.

Beyze giren 100 elektronu düşün:

- **Yaklaşık 1 tanesi** bir boşluğa düşer ve orada kalır.
- **Yaklaşık 99 tanesi** boşluğa düşmeden beyzin karşı ucuna ulaşır.

Boşluğa düşen o 1 elektron nereye gidiyor? Hiçbir yere gitmiyor ama beyzdeki boşluk da kaybolmuş oluyor. Beyze bağlı artı uç beyzdeki elektronlardan birkaçını sürekli çekip alıyor, yani yeni boşluklar açıyor. O 1 elektron bu şekilde **beyz bacağından dışarı çıkıp pilin artısına gidiyor.** Bu, **beyz akımı.**

## 5. İkinci duvarda kaydırak

Geri kalan 99 elektron beyzin sonuna, ikinci duvarın kenarına geliyor. Önceki adımda söylemiştik, bu duvarın bir yüzü kaydırak:

- Duvarın beyz tarafı eksi, kollektör tarafı artı yüklü.
- Beyzden gelen elektron karşısında **artı yükleri** görüyor ve çekiliyor.
- Üstüne kollektör pilin artısına bağlı, bu çekimi daha da güçlendiriyor.

Önceki adımda kaydırak hazırdı ama tepesinde kimse yoktu. Şimdi emiterden gelen elektronlar kaydırağın tepesine yığıldı. 99 elektron kaydırağa varıyor ve kollektöre doğru kayıp gidiyor.

## 6. Kollektörde ve ötesinde

Kayan elektronlar kollektöre giriyor. Kollektör pilin artısına bağlı olduğu için onları kendine çekmeye devam ediyor. Elektronlar kollektör bacağından çıkıp pilin artısına doğru gidiyor.

Hepsini birleştirelim, elektronların yolu:

1. Pilin eksisinden çıkıp emitere giriyorlar.
2. Birinci duvarı (yıkılmış) geçip beyze giriyorlar.
3. Çoğu (99) beyzi koşarak geçip ikinci duvardan kayıyor ve kollektörden çıkıp pilin artısına gidiyor. Bu **kollektör akımı.**
4. Az bir kısmı (1) beyzdeki boşluklara düşüyor ve beyz bacağından çıkıp pilin artısına gidiyor. Bu **beyz akımı.**

Emiterden çıkan 100 elektron iki yoldan pilin artısına varıyor: 99'u kollektör yolundan, 1'i beyz yolundan. Emiterden çıkan toplam akım, beyz ve kollektör akımının toplamı.

## 7. Sonuç: Açık

Pilin gücü artık bir akım yaratıyor. Kolu çevirdik (beyze küçük bir akım verdik), kapı açıldı ve emiterden kollektöre güçlü bir elektron akışı başladı. Beyz bacağından geçen akım çok küçük, kollektör bacağından geçen akım çok büyük.

## Özet

- Beyz, direnç üzerinden pilin artısına bağlanınca emiter-beyz sınırı diyodun ileri yönü gibi çalışıyor ve 0,7 Volt civarında **birinci duvar yıkılıyor.**
- Emiterdeki elektronlar beyze doluyor.
- Beyz çok ince ve az boşluklu olduğu için elektronların çoğu boşluğa düşmeden karşı tarafa ulaşıyor.
- İkinci duvar beyzden gelen elektronlar için bir **kaydırak**, kollektördeki artı uç da onları çekiyor. Elektronlar kayıp kollektöre geçiyor.
- 100 elektrondan yaklaşık 99'u kollektörden, 1'i beyzden pilin artısına gidiyor.
- Küçük bir akımla (beyz) büyük bir akım (kollektör) yönetilmiş oluyor.

# NPN Transistör: Kapıyı Ayarlamak (Az, Çok ve Direnç)

Önceki adımda beyzi bağlamış ve kapıyı açmıştık. Elektronların yolunu da görmüştük: 100 elektrondan yaklaşık 99'u kollektörden, 1'i beyzden pilin artısına gidiyordu. Şimdi şuna bakacağız: kolu az çevirirsek ne olur, çok çevirirsek ne olur, ve bu "yüz kat" oranı nereden geliyor?

## 1. Kolu çevirmek ne demek?

Beyze ne kadar akım verdiğimizi, beyze bağladığımız **direnç** belirler:

- **Büyük direnç:** Beyze az akım girer.
- **Küçük direnç:** Beyze çok akım girer.

Beyze verdiğin akım arttıkça birinci duvar daha çok alçalır ve emiterden beyze **daha kalabalık bir elektron grubu** girer. Beyze verdiğin akım azaldıkça duvar yükselir ve girenler azalır. Kolu çevirmek, kapıdan geçen kalabalığın büyüklüğünü ayarlamak demek.

## 2. "Yüz kat" oranı nereden geliyor?

Önceki adımda 100 elektrondan 1'inin boşluğa düştüğünü, 99'unun geçtiğini söylemiştik. Bu oran rastgele değil, beyzin yapısından geliyor:

- Beyz **ne kadar ince** ve **ne kadar az boşluklu** olursa, elektronların boşluğa düşme şansı o kadar az olur, daha çoğu karşıya geçer.
- Beyz kalın ve çok boşluklu olsaydı, daha çok elektron boşluğa düşerdi.

Üretici beyzin inceliğini ve boşluk sayısını baştan ayarlar. Oran bir kere belirlenir ve o transistör için sabit kalır. Bu orana **kazanç** denir, küçük transistörlerde genelde 50 ile 300 arasındadır.

Kalabalık büyüyünce ne olduğuna bakalım. Oran sabit, yani her 100 elektrondan 1'i beyzde kalıyor:

|Emiterden giren kalabalık|Beyz bacağından çıkan|Kollektör bacağından çıkan|
|---|---|---|
|100|1|99|
|200|2|198|
|300|3|297|

Beyz akımı 2 katına çıkarsa kollektör akımı da 2 katına çıkar, çünkü ikisi **aynı kalabalığın iki payı.** Biri küçük pay, biri büyük pay. Araya sihirli bir büyütücü girmiyor.

## 3. Kapı üç durumda olabilir

Örnek devre: 5 Volt pil, bir LED ve 150 Ω direnç. Transistör olmasa bu devrede LED'den en fazla yaklaşık 20 mA geçiyordu (diyot notundaki hesap). Kazanç 100 olsun:

|Beyz akımı|Kollektör akımı|LED|
|---|---|---|
|0|0|Sönük|
|0,05 mA|5 mA|Loş|
|0,1 mA|10 mA|Yarı parlak|
|0,2 mA|20 mA|Tam parlak|
|1 mA|Yine 20 mA|Yine tam parlak|

**Kapalı:** Beyze akım yok, duvar yıkılmamış, hiçbir şey geçmiyor.

**Yarım açık:** Beyz akımı küçük, kollektör akımı onun 100 katı. LED loş yanıyor. Beyz akımını azıcık artırıp azaltırsan LED'den geçen akım da aynı şekilde, ama 100 kat büyük artıp azalıyor. Yükselteç dediğimiz şey bu orantıyı kullanmak. Ses konusunda bunu gerçek örnekle göreceğiz.

**Tam açık:** Son satıra dikkat. Beyz akımını 0,2 mA'den 1 mA'e çıkardık ama kollektör akımı 20 mA'de kaldı. Çünkü artık kapıyı transistör değil, **devredeki dar boğaz** sınırlıyor: pilin gücü, LED ve direnç. Kapı tamamen açık olunca akımı yük belirler (Ohm Kanunu). Transistör akımı o sınırın üstüne çıkaramaz.

LED'in parlaklığını ayarlamanın "kontrol" olduğunu söylemiştin. Doğru, ve bu üç hâl tam olarak o kontrolün kendisi.

## 4. Beyz direnci neden şart?

Birinci duvar yıkılınca beyz-emiter sınırı diyot gibi neredeyse hiç direnç göstermez, sadece yaklaşık 0,7 Volt harcar. Beyze direnç bağlamazsan, geri kalan voltaj hiçbir engele takılmadan akıma yol verir. Ohm Kanunu'na göre direnç küçükse akım büyük olur. Sonuç: beyz bölgesi aşırı ısınır ve transistör yanar.

Bu, LED'in önüne neden direnç koyduğumuzla aynı sebep. Direnç beyz akımını güvenli bir seviyede tutar.

## 5. Beyz direnci nasıl hesaplanır?

Örnek: pinden 5 Volt veriyoruz ve 100 mA çeken bir motoru süreceğiz.

1. Kazanç 100 ise teoride beyz akımı 1 mA yeter. Ama kazanç transistörden transistöre değişir ve biz kapıyı **kesin ve tam açmak** istiyoruz. O yüzden güvenlik payı bırakıp beyz akımını yükün yaklaşık **onda biri** alıyoruz: 100 ÷ 10 = **10 mA.**
2. Beyz-emiter sınırı 0,7 Volt harcıyor. Direncin üzerine kalan düşüyor: 5 − 0,7 = **4,3 Volt.**
3. Direnç = Voltaj ÷ Akım = 4,3 ÷ 0,01 = **430 Ω.** En yakın standart değer **470 Ω.**

Pin 5 Volt verince beyze yaklaşık 9 mA akıyor, kapı tamamen açılıyor, motor dönüyor. Pin 0 Volt'a inince beyz akımı kesiliyor, kapı kapanıyor, motor duruyor. Tam bir anahtar.

## Özet

- Beyze verilen akımı, beyze bağlı **direnç** belirler.
- Beyz akımı arttıkça emiterden beyze giren kalabalık büyür.
- Her 100 elektrondan 1'i beyzde kalır, 99'u geçer. Bu oran beyzin inceliğinden ve az boşluklu olmasından gelir, **kazanç** diye adlandırılır, sabittir.
- Beyz akımı artınca kollektör akımı da aynı oranda artar. İkisi aynı kalabalığın iki payı.
- Kapı **kapalı**, **yarım açık** ya da **tam açık** olabilir. Tam açıkken akımı transistör değil devredeki yük belirler.
- Beyz direnci şart, yoksa duvar yıkılınca akım uçar ve transistör yanar.
- Hesap: beyz akımı ≈ yükün onda biri, direnç = (Voltaj − 0,7) ÷ beyz akımı.
# NPN Transistör: Gerçek Devre (Motor, Geri Tepme Diyotu, Test)

Önceki adımlarda transistörün içinde ne olduğunu gördük. Şimdi gerçek bir devrede ne yaptığına bakalım: küçük bir pin ile büyük bir motoru sürmek.

## 1. Sorun ne?

Elinde bir mikrodenetleyici pini var. Pin en fazla yaklaşık 20 mA verebilir. Motor ise 100 mA çekiyor. Motoru doğrudan pine bağlarsan pin yanar.

Transistör bu işi çözer: pin sadece beyzin küçük akımını verir, motorun büyük akımı pilden gelir.

## 2. Devreyi kuralım

Bu bağlantıyı bir çember olarak düşün, tıpkı diyotta yaptığımız gibi:

- Motor pilinin **artısı** → **motor** → transistörün **kollektörü**
- Transistörün **emiteri** → motor pilinin **eksisi**
- Pinin **çıkışı** → **470 Ω direnç** → transistörün **beyzi**
- Pinin **GND** ucu → motor pilinin **eksisi** (ortak eksi)

```
(+) pil ──── MOTOR ──── KOLLEKTÖR
                          BEYZ ←── 470 Ω ←── PİN
(−) pil ──── EMİTER          
(−) pil ──── PİNİN GND'si
```

Son satır çok önemli. Beyz akımının dönebileceği çember şu: pin → direnç → beyz → emiter → eksi → pinin GND'si. Pinin GND'si pilin eksisine bağlı değilse bu çember kopuk kalır, beyze akım gitmez ve motor hiç dönmez. Tamir masasında en sık yapılan hata budur.

## 3. Çalışırken elektronlar ne yapıyor?

**Pin 5 Volt veriyor (1):**

- Beyze direnç üzerinden yaklaşık 9 mA akım giriyor (hesabı önceki adımda yapmıştık: 4,3 Volt ÷ 470 Ω).
- Birinci duvar yıkılıyor, kapı tamamen açılıyor.
- Pilin eksisinden gelen elektronlar emiterden beyze, oradan kaydırakla kollektöre geçip motordan pilin artısına gidiyor. Motor dönüyor.

**Pin 0 Volt veriyor (0):**

- Beyze akım gitmiyor, birinci duvar yıkılmıyor.
- Kapı kapalı, motordan akım geçmiyor. Motor duruyor.

Pin sadece küçük bir kolu çeviriyor, motorun gücü pilden geliyor.

## 4. Motor kapanırken ne oluyor?

Bobin notunu hatırla. Bobin (motorun içinde de sarılı teller var) akımın aniden değişmesine izin vermiyor. "Ağır tren" gibi, son sürat giderken önünü kestiğinde durmak istemiyor.

Transistör kapıyı aniden kapatınca, motorun bobininden geçen akım **şat diye kesilmek** zorunda kalıyor. Bobin buna izin vermek istemiyor:

- İçinde birikmiş manyetik ordu çökmeye başlıyor.
- Çöken manyetik alan elektronları kamçılayıp zorla ileri fırlatıyor.
- Yol kapalı olduğu için bu elektronlar transistörün kollektörüne yığılıyor ve orada **çok yüksek bir voltaj tekmesi** oluşuyor. Pilin voltajından çok daha yüksek, bazen onlarca Volt.

Bu tekme kollektördeki ikinci duvarı zorluyor ve transistörü yakabilir.

## 5. Çözüm: Geri tepme diyotu

Diyot dersinde bunu görmüştük. Motorun iki ucuna, **ters yönde** bir diyot bağlıyoruz:

- Diyotun **çizgili ucu** (N, katot) pilin artısı tarafına
- Diyotun **çizgisiz ucu** (P, anot) kollektör tarafına

```
(+) pil ──┬── MOTOR ──┬── KOLLEKTÖR
          └─ DİYOT ◄──┘
        (çizgili uç yukarıda, artı tarafta)
```

**Normal çalışırken:** Pilin artısı çizgili uca (N), kollektör tarafı çizgisiz uca (P) bağlı. P tarafı daha düşük voltajda, yani diyot **ters yönde.** Duvar kalın, diyot hiçbir şey yapmıyor. Motor normal çalışır.

**Kapanma anında:** Bobinin tekmesi kollektör tarafının voltajını pilin artısından **daha yüksek** yapıyor. Bu, diyot için **ileri yön** demek: P tarafı N tarafından daha yüksek. Duvar yıkılıyor, diyot geçirmeye başlıyor.

Bobinin kamçıladığı elektronlara artık gidecek bir yol var: motorun içinden çıkıp diyottan geçip tekrar motora giriyor ve bir çember çiziyor. Enerji bu çemberin içinde yavaş yavaş sönüyor. Voltaj tekmesi transistöre ulaşmıyor.

Rölelerin yanında küçük bir diyot görürsen sebebi budur.

## 6. Transistörü multimetreyle test etmek

NPN transistörün içinde iki diyot var. Birinci adımda gördüğümüz iki duvar iki diyot demek. Multimetreyi **diyot moduna** al (▷| sembolü):

|Kırmızı prob|Siyah prob|Sağlam transistörde|
|---|---|---|
|Beyz|Emiter|0,5 - 0,7 civarı|
|Beyz|Kollektör|0,5 - 0,7 civarı|
|Emiter|Beyz|OL|
|Kollektör|Beyz|OL|
|Emiter|Kollektör|OL (iki yönde de)|

Neden bu şekilde? Kırmızı prob artı, siyah prob eksi. Kırmızıyı beyze (P) ve siyahı emitere ya da kollektöre (N) bağlayınca diyodu ileri yönde bağlamış olursun. Duvar yıkılır, 0,5-0,7 değeri görürsün.

**Arıza işaretleri:**

- İki bacak arasında her iki yönde de sıfıra yakın değer: kısa devre.
- Beklenen değerlerin yerine her yönde OL: kopuk.

**Dikkat:**

- Bacak sırası (E, B, C) modele göre değişir, datasheet'e bak.
- Şemada emiterin ucunda bir ok vardır. NPN'de ok dışarı bakar.
- Devre üstündeyken ölçüm yanıltabilir, çünkü çevredeki parçalar ölçümü etkiler. Şüphede bir bacağı sök.

## Özet

- Küçük pin, transistörün beyzine **direnç** üzerinden bağlanır. Motorun akımı pilden gelir, pin sadece kapıyı açıp kapatır.
- Pinin GND'si ile motor pilinin eksisi **ortak** olmalı, yoksa beyz akımının çemberi kopuk kalır.
- Pin 1 ise kapı açık, motor döner. Pin 0 ise kapı kapalı, motor durur.
- Kapı kapanınca bobin akımın kesilmesine izin vermek istemez ve **voltaj tekmesi** üretir. Bu tekme transistörü yakabilir.
- **Geri tepme diyotu** motorun uçlarına ters yönde bağlanır: çizgili uç artı tarafta. Normal çalışırken hiçbir şey yapmaz, tekme gelince geçirir ve enerjiyi motorun içinde söndürür.
- Transistör içinde iki diyot gibi test edilir: beyz-emiter ve beyz-kollektör arası bir yönde 0,5-0,7, ters yönde OL.

# Mikrodenetleyici ve Pin

Bu kelimeyi açıklamadan kullandım, haklısın. Sade anlatayım.

## 1. Mikrodenetleyici nedir?

**Küçücük bir bilgisayar.** Tek bir çipin içine sığmış.

Normal bir bilgisayarda işlemci, hafıza ve dış dünyayla bağlantı kuran parçalar ayrı ayrı yerlerde durur. Mikrodenetleyicide hepsi **tek bir çipin içinde.** Çok güçlü değil (oyun oynatamaz, internette gezemez), ama çok ucuz, çok az elektrik harcıyor ve tek bir işi yapmak için biçilmiş kaftan.

Evde onlarca tane var, farkında bile değilsin: çamaşır makinesi, mikrodalga fırın, TV kumandası, klima, elektrikli diş fırçası. Çamaşır makinesinde "30 dakika yıka, sonra sıkma yap" diye karar veren, içindeki mikrodenetleyici.

Arduino, ESP32 ya da Raspberry Pi Pico gibi şeyler, bir mikrodenetleyicinin üzerine bacaklar ve USB girişi eklenmiş **hazır deney kartları.** Başlamak için kullanılırlar.

## 2. Pin nedir?

Çipin **bacakları**, yani dış dünyaya açılan bağlantı noktaları. Mikrodenetleyici kendi içinde düşünüyor ama dışarıdaki bir şeyi yakmak, çevirmek ya da okumak için bir yola ihtiyacı var. O yol pinler.

Çipin içindeki program her pini tek tek yönetebilir. Pinin iki işi olabilir:

**Çıkış olarak (komut vermek):** Pin ya 0 Volt ya da 5 Volt (bazı kartlarda 3,3 Volt) verir. 5 Volt "1", 0 Volt "0" demek. Program "bu pini 1 yap" der, pin 5 Volt verir. "0 yap" der, 0 Volt verir. Bu bir pilin, programın istediği an açılıp kapanan hâli gibi.

**Giriş olarak (bilgi okumak):** Pin dışarıdan gelen voltajı ölçer. Bir butona basıldığında pine 5 Volt geliyorsa program "butona basıldı" diye anlar. Dirençte öğrendiğin pull-up ve pull-down dirençleri burada devreye giriyor.

## 3. Pin neden kolayca yanıyor?

Pin, güçlü bir pil değil. Çipin içindeki küçücük bir devre. Bu yüzden verebileceği akım çok az: yaklaşık **20 mA**. Bu bir LED'i yakmaya yeter ama bir motoru, röleyi ya da LED şeridi süremez. Fazlasını çekersen pin ya da çipin kendisi yanar.

Transistörün işi tam burada başlıyor.

## 4. Transistörle bağlantısı

Önceki devreye bak:

- **Pin 1 (5 Volt) olunca:** 470 Ω direnç üzerinden transistörün beyzine küçük bir akım (yaklaşık 9 mA) gider. Kapı açılır, motorun büyük akımı pilden geçer.
- **Pin 0 olunca:** Beyze akım gitmez, kapı kapanır, motor durur.

Pin hiçbir güç yükü taşımıyor. Sadece "aç" ya da "kapa" diyor. Programın bu kararı verdiği satır Arduino'da şöyle görünür:

```
digitalWrite(8, HIGH);
```

Bunun anlamı: "8 numaralı pini 1 yap, yani 5 Volt ver". Pin 5 Volt verir, transistör açılır, motor döner. Bilgisayar bilimine geçişin ilk köprüsü burası: bir satır kod, gerçek dünyada bir motoru çalıştırıyor.

## 5. Küçük bir not

Bazı kartlarda (ESP32 gibi) pinler 5 Volt yerine **3,3 Volt** verir. O zaman beyz direncini hesaplarken 5 yerine 3,3 kullanırsın: (3,3 − 0,7) ÷ 0,01 = 260 Ω, yani yaklaşık 270 Ω.

## Özet

- **Mikrodenetleyici:** Tek çipin içine sığmış küçük bir bilgisayar. Çamaşır makinesi, klima, kumanda gibi cihazların beyni.
- **Pin:** Çipin bacağı, dış dünyayla bağlantı noktası.
- Pin **çıkış** olursa program ona 0 ya da 1 (0 Volt ya da 5 Volt) verdirir. **Giriş** olursa dışarıdan gelen bilgiyi okur.
- Pin en fazla yaklaşık **20 mA** verebilir, bu yüzden büyük yükleri doğrudan süremez.
- Transistör araya girer: pin küçük akımla kapıyı açıp kapatır, büyük akım pilden gelir.

Devreyi çizdim. Alttaki iki düğmeyle "motor çalışırken" ve "kapı kapanınca (tekme anı)" durumları arasında geçiş yapabilirsin. Mavi hareketli noktalar elektronların yolunu gösteriyor.

![Pasted image 20261029095653](../assets/Pasted%20image%2020261029095653.png)


![Pasted image 20261029095709](../assets/Pasted%20image%2020261029095709.png)
Çizimi şöyle okuyabilirsin.

**Devrenin parçaları:** Üstteki tel pilin artısından A noktasına gidiyor. Motor A ile B arasında duruyor. B, transistörün kollektörüne bağlı. Emiter pilin eksisine gidiyor. Pin, 470 Ω direnç üzerinden beyze bağlı. Pinin GND'si pilin eksisiyle ortak. Motorun sağında, A ile B arasında diyot var. Çizgili ucu (N) üstte, yani A tarafında.

**Motor çalışıyor düğmesi:** Pin 1 olduğu için transistör açık. Elektronlar pilin eksisinden çıkıp alttaki telden emitere, transistörden kollektöre, B noktasından motora ve A noktasından pilin artısına dönüyor. İnce mavi hat beyz akımı: beyzden direnç üzerinden pine gidiyor. Diyot soluk, çünkü ters yönde ve hiçbir şey yapmıyor.

**Kapı kapandı düğmesi:** Pin 0 oldu, transistör kapandı, pilin yolu kesildi. Bobin akmaya devam etmek istiyor ve elektronlar turuncu çemberde dönüyor: motordan B'den A'ya, sonra diyottan A'dan B'ye, sonra tekrar motora. B noktası yaklaşık 12,7 V'ta kalıyor, çünkü diyot açılınca voltajı orada tutuyor. Transistör soluk, tehlikeli voltajı hiç görmüyor.

Tek bir yere bakacaksan şuna bak: ikinci durumda elektronların yolu pile hiç uğramıyor, sadece motor ve diyot arasında dönüyor. Tren duvara çarpmıyor, kapalı bir halka rayda yavaşlıyor.
