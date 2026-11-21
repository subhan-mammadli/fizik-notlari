
# Direnç(Resistor)

Elektronik kartların kalbindeki "Üç Büyük Pasif Eleman" ailesinin en temel, en eski ve en çok kullanılan üyesine, yani **Dirençe (Resistora)** ulaştık!

### 1. Direnç Tam Olarak Nedir? (Fiziksel Hali)

Elektronik devrelerinde her zaman elektronların deli gibi, engelsiz bir şekilde akmasını istemeyiz. Bazı yerlerde o akışı yavaşlatmak, sınırlamak ve kontrol altına almak gerekir. İşte direnç tam olarak bu işi yapar.

- **Düz Kablo:** Otoyolun en geniş, bomboş ve hiçbir engeli olmayan halidir. Elektronlar gaza basar ve son sürat geçer.

- **Direnç:** Otoyolun ortasına konulmuş **dar bir tünel, kalabalık bir sokak veya minik bir dar boğazdır.** Elektronlar o dar yerden geçmek zorundadır.

### 2. Su Borusu Benzetmesi: Dar Boru ve Sürtünme

Zihninde su pompası ve kalın bir su borusu hayal et.

- Su, kalın borudan hiçbir şeye takılmadan şırıl şırıl akar.

- Şimdi o borunun tam ortasına alıp **içinden suyun zorla geçebileceği kadar dar, pürüzlü bir parça (dar boğaz)** koyduğunu düşün.

- Ne olur? Su o dar yerden geçerken sıkışır, hızı düşer ve arkadaki basınç dengelenir.


İşte direnç de budur! Kablonun üzerindeki **elektron akışını (amperi) daraltan ve kısıtlayan** fiziksel bir bariyerdir.

### 3. Neden Isınır? (Sürtünmenin Bedeli)

Fizikte harika bir kural vardır: **Hareket olan yerde sürtünme vardır, sürtünme olan yerde ise mutlaka ISI vardır.**

- Elektronlar o daracık direncin içinden geçmeye çalışırken, içerideki atomlara çarparlar, birbirlerini sıkıştırırlar ve müthiş bir **trafik sıkışıklığı (sürtünme)** yaratırlar.

- Bu çarpışmalar sırasında elektrik enerjisinin bir kısmı **ısıya dönüşür** ve havaya karışır.

- _Gerçek Hayattan Örnek:_ Elektrikli sobaların, fırınların veya saç kurutma makinelerinin içindeki o kıpkırmızı yanan tellerin hepsi aslında devasa birer **dirençtir!** Elektrik oradan geçerken sıkışır, sürtünmeden dolayı kıpkırmızı kesilir ve ortalığı ısıtır.

### 4. Pratikte Direnci Neden Kullanırız? (Tamir Masası)

Kartların üzerinde milyonlarca direnç olmasının sebebi iki hayati görevi yerine getirmeleridir:

#### A. Hassas Parçaları Korumak (LED Örneği)

Elinde minik bir LED lamba var. LED, elektronik dünyasının narin cam bardağı gibidir; doğrudan büyük bir pile bağlarsan hemen patlar, yanar.

- **Direncin Rolü:** LED'in önüne bir direnç koyarsın. Direnç, pilden gelen elektronların çoğunu arkada tutar, sadece LED'in nefes alabileceği kadar minik bir akımın geçmesine izin verir. Böylece LED güvenle yanar. Direnç burada bir **güvenlik bekçisidir.**

#### B. Voltajı Paylaştırmak (Bölmek)

Devredeki bazı çiplere 5 Volt yerine sadece 3 Volt göndermen gerekir. Kaynaktaki voltajı düşürmek için dirençleri kol kola dizersin; dirençler voltajı aralarında paylaşır ve istediğin hassas parçaya doğru basınçta elektrik girmesini sağlarsın.

### Özetle Direnç Nedir?

- **Kondensatör:** _"Voltajın oynamasına izin vermem, enerji depolarım!"_

- **Bobin:** _"Akımın aniden değişmesine izin vermem, manyetik ordu kurarım!"_

- **Direnç:** _"Ben akışın ta kendisiyim! Otoyolu daraltırım, elektronları yavaşlatırım, fazla enerjiyi ısıya çevirip ortalığı güvenli tutarım."_


## Resistoru Ne Zaman Kullanırsın?

Teoride direncin bir "dar boğaz ve sürtünme noktası" olduğunu gördük. Peki eline havya alıp bir devre tasarlarken ya da bir kartı tamir ederken **direnci tam olarak hangi hayat kurtarıcı senaryolarda kullanırsın?**

Gerçek dünya projelerinde ve tamir masasında direnci en çok kullanacağın **4 temel senaryo** şunlardır:

### 1. Ne Zaman Kullanırsın? Hassas Parçaları Yanmaktan Korumak İçin (Akım Sınırlama)

- **Problem:** Elinde minik bir LED lamba veya hassas bir entegre var. Doğrudan pilin uçlarına bağlarsan, akım o kadar hızlı ve yüksek gelir ki parça anında aşırı ısınır, patlar veya yanar.

- **Nasıl Kullanırsın?** Parçanın önüne **seri olarak** (akım yolunun tam üstüne) uygun boyutta bir direnç yerleştirirsin. Direnç o dar boğazıyla elektronları yavaşlatır, geçmesine izin verilen akım miktarını güvenli bir seviyeye indirir. (Elektronik dünyasının en çok yapılan işidir: LED'in önüne direnç koymak).
### 2. Ne Zaman Kullanırsın? Büyük Voltajı Küçültmek İstediğinde (Gerilim Bölücü / Voltage Divider)

- **Problem:** Elinde 9 Volt'luk bir pil var ama beslemek istediğin sensör veya mikroişlemci pini en fazla 3.3 Volt istiyor. Doğrudan verirsen sensör bozulur.

- **Nasıl Kullanırsın?** İki direnci ard arda (kol kola) bağlayıp aradan bir kablo çekersin. Buna **Gerilim Bölücü** denir.

    - _Mantığı:_ Nasıl ki tek bir uzun su hortumuna iki tane dar boğaz koyduğunda suyun basıncı o dar boğazlar arasında paylaşılırsa, dirençler de o 9 voltluk toplam basıncı (gerilimi) aralarında paylaşırlar. Sen o iki direncin tam ortasından istediğin düşük voltajı (örneğin 3.3V) alıp hassas sensörüne güvenle verirsin.
### 3. Ne Zaman Kullanırsın? Dijital Pinlerin "Kafasının Karışmasını" Önlemek İçin (Pull-Up / Pull-Down Dirençleri)

- **Problem:** Mikroişlemcilerin (Arduino, STM32 vb.) giriş pinleri çok hassastır. Eğer bir butona basılmadığı anlarda o pin havada (boşta) kalırsa, havadaki statik elektrik ve elektromanyetik dalgalar pini "Acaba bastı mı, basmadı mı?" diye kandırır; devre kendi kendine saçma sapan hareketler yapar.

- **Nasıl Kullanırsın?** Pini ya sıkıca artı kutba ya da eksi kutba bağlayan küçük bir direnç koyarsın. Buna **Pull-Up** veya **Pull-Down** direnci denir. Direnç orada bir "çapa" gibi görev yapar; buton basılana kadar pinin değerini net bir şekilde sabit (0 veya 1) tutar. Kartlarda etrafı minik dirençlerle dolu çiplerin en büyük sırrı budur.

### 4. Ne Zaman Kullanırsın? Büyük Bir Şeyi Tetiklemek İçin Anahtar Sinyali Üretmek (Biasing)

- **Problem:** Büyük bir motoru veya güçlü bir lambayı çalıştırmak için bir Transistör (elektronik anahtar) kullanacaksın. Ama transistörün kapısını açmak için çok azıcık, hassas bir tetik akımına ihtiyacın var.

- **Nasıl Kullanırsın?** Ana hattan gelen akımın önüne küçük bir direnç koyarak o akımı inceltir ve transistörün "tetikleme bacağına" (Base) verirsin. Böylece büyük sistemi güvenle kontrol edersin.

### Tamir Masasında Direnç Seçerken En Önemli Kural: Watt (Güç) Değeri!

Direnç seçerken sadece kaç ohm (direnç büyüklüğü) olduğuna değil, **fiziksel boyutuna (Watt değerine)** de mutlaka bakarsın:

- Hani dirençler akımı yavaşlatırken fazla enerjiyi **ısıya çeviriyordu** ya?

- Eğer direnç üzerinden çok fazla akım geçecekse ve sen parmak kadar küçük bir direnç kullandıysan, o direnç o kadar çok ısınır ki bir süre sonra **kararır, kokar ve ortadan ikiye yanarak patlar.**

- Yüksek akım geçen yerlerde büyük, seramik veya kalın gövdeli dirençler (güç dirençleri) kullanırsın ki o ısıyı etrafa yayabilsin.

Özetle; devrede akımı kısmak, voltajı bölüştürmek veya pinleri kararlı tutmak istiyorsan devreye **direnci** koyarsın.
# Pull-up ve Pull-down

## 1. Sorun: Havada kalan nokta

Bir yerin voltajı ancak o nokta pilin artı odasına ya da eksi odasına **bağlıysa** belli olur. Hiçbirine bağlı değilse o noktanın voltajı belirsizdir. Buna **havada** (floating) denir.

Havada kalan bir nokta, etraftaki küçük elektriksel gürültülerle rastgele yüklenir. Bir an artıya yakın, bir an eksiye yakın, kendi kendine zıplar. Bu noktayı bir devre elemanının bacağına bağlarsan (MOSFET'in Gate'i gibi) o eleman ne yapacağını bilemez.

## 2. Örnek devre: Bir düğme

Düğmenin bir ucu pilin artısına (5 V), diğer ucu bir **giriş noktasına** bağlı. Bu noktaya bakıp "düğmeye basıldı mı?" diye soruyoruz.

```
 (+5V) ──[ düğme ]──── giriş noktası
```

- **Düğmeye basınca:** Giriş noktası artıya bağlanır, 5 V olur. Sorun yok.
- **Düğmeye basmayınca:** Düğme açık, giriş noktası hiçbir yere bağlı değil. **Havada.** Voltajı rastgele zıplar, "basıldı mı basılmadı mı" belli olmaz.

Çözüm: giriş noktasına, basılmadığı zamanlarda **ne olması gerektiğini söyleyen** bir yol bağlamak.

## 3. Pull-down: Basılmayınca eksiye çek

Giriş noktasını bir direnç üzerinden **eksiye (GND)** bağlıyoruz.

```
 (+5V) ──[ düğme ]──┬──── giriş noktası
                    │
                  [10 kΩ]
                    │
                  (GND)
```

**Düğmeye basılmıyor:** Giriş noktası havada kalmıyor, direnç üzerinden eksiye bağlı. Noktadaki fazla elektronlar bu yoldan eksiye akıp gidiyor. Voltaj **0 V'a** iniyor. Artık net: basılmadı.

**Düğmeye basılıyor:** Artı uç giriş noktasına bağlanıyor. Nokta **5 V** oluyor. Direnç hâlâ eksiye bağlı ama yol çok dar olduğu için sadece küçük bir akım sızıyor: I = 5 ÷ 10000 = **0,5 mA.** Voltajı bozmaz.

Adı bundan geliyor: direnç noktayı **aşağıya (eksiye) çekiyor.**

## 4. Pull-up: Basılmayınca artıya çek

Ayna görüntüsü. Direnç artıya, düğme eksiye bağlı.

```
 (+5V) ──[ 10 kΩ ]──┬──── giriş noktası
                    │
                 [ düğme ]
                    │
                  (GND)
```

**Düğmeye basılmıyor:** Giriş noktası direnç üzerinden artıya bağlı, **5 V.**

**Düğmeye basılıyor:** Düğme noktayı doğrudan eksiye bağlıyor, **0 V** oluyor. Direnç sadece 0,5 mA'lik küçük bir akımı artıdan eksiye geçirir.

Adı: direnç noktayı **yukarıya (artıya) çekiyor.** Dikkat: burada basınca 0 V olur, mantık ters.

## 5. Neden düz tel değil, direnç?

Pull-down'da direnç yerine düz tel kullansan, giriş noktası her zaman doğrudan eksiye bağlanır. Düğmeye basınca artı ile eksi, telden ve düğmeden **direnç olmadan** birbirine bağlanır. Ohm Kanunu'na göre direnç sıfıra yakınsa akım uçar, pil ya da tel yanar (kısa devre). Direnç hem noktayı eksiye çekmeye yetiyor hem de akımı küçük tutuyor.

## 6. Neden 10 kΩ?

- **Çok küçük direnç (örneğin 100 Ω):** Düğmeye basınca 5 ÷ 100 = 50 mA akar. Boşa enerji harcar.
- **Çok büyük direnç (örneğin 10 MΩ):** Yol o kadar dar ki gürültü noktayı rahatça iterebilir. Nokta yine kararsız kalır.
- **10 kΩ:** İkisinin ortası, standart seçim.

## 7. Tablo

||Pull-down|Pull-up|
|---|---|---|
|Direnç nereye bağlı|Giriş noktası ile eksi|Artı ile giriş noktası|
|Basılmayınca|0 V|5 V|
|Basılınca|5 V|0 V|
## Nasıl Kullanılır?

Teoride ne işe yaradığını ve nerelerde hayat kurtardığını gördük. Peki eline gerçek bir direnç aldığında, onu devreye **fiziksel olarak tam olarak nasıl bağlarsın?**

Breadboard (deney kartı) üzerinde veya havya ile çalışırken direnci devreye yerleştirirken bilmen gereken **3 pratik kural** şunlardır:

### 1. Seri Bağlantı (Dar Boğazı Akımın Yolunun Üstüne Koymak)

Amacın akımı sınırlamaksa (örneğin bir LED'i korumak), direnci **seri** bağlarsın.

- **Nasıl Yapılır?** Akımın aktığı telin tam orta yerini makasla kesip araya direnci ekliyormuş gibi düşün. Pilden çıkan elektronlar mecburen önce direncin o daracık tünelinden geçmek zorundadır. Başka alternatif bir yol yoktur. Akım yavaşlar, koruma sağlanır.

### 2. Gerilim Bölücü (İki Direnci Kol Kola Takmak)

Amacın yüksek voltajı düşürüp ara bir değer elde etmekse, iki direnci **ard arda (seri)** bağlarsın.

- **Nasıl Yapılır?** Birinci direncin çıkış bacağını, ikinci direncin giriş bacağına lehimlersin (ortada birleşirler). İki uç dışarıda kalır. İşte o iki direncin **tam ortasındaki birleşim noktasından** bir kablo çekersin. Toplam voltaj o iki direnç arasında paylaşılır ve ortadaki noktadan tam istediğin düşük voltajı alırsın.

### 3. Doğru Direnci Nasıl Seçersin? (Renkler ve Multimetre)

Elindeki bir direncin değerini (kaç ohm olduğunu) anlamanın iki yolu vardır:

- **Renk Kodları:** Dirençlerin üzerinde minik renkli çizgiler (kahverengi, siyah, kırmızı vb.) vardır. Her rengin bir rakam karşılığıdır; bu çizgileri okuyarak direncin gücünü anlarsın.

- **Multimetre (En Kolayı):** Ölçü aletini (multimetreyi) direnç (Ohm - $\Omega$) simgesine getirirsin, prob uçlarını direncin iki bacağına dokundurursun; ekran direkt değerini yazar.

### Üç Büyük Pasif Elemanı Tamamladık! 🏆

Kondensatör, Bobin ve Direnç... Elektronik kartların kalbindeki bu üç temel "pasif" (kendi başına akım üretmeyen ama yön veren/depolayan) elemanın mantığını ve pratik kullanımını tamamen çözdün:

1. **Kondensatör:** Voltajın oynamasından nefret eder, basıncı sabit tutar (Su deposu).

2. **Bobin:** Akımın oynamasından nefret eder, manyetik ordu kurup akışı pürüzsüzleştirir (Ağır tren / Eylemsizlik).

3. **Direnç:** Akışın ta kendisidir; otoyolu daraltır, elektronları yavaşlatır ve güvenliği sağlar (Dar boğaz / Sürtünme).

