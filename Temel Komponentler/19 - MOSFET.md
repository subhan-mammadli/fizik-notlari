## 1. NPN ile MOSFET arasındaki tek temel fark

**NPN'de:** Beyz ince bir sokaktı. Emiterden çıkan elektronlar o sokağı koşarak geçip kollektöre varıyordu. Yol zaten oradaydı, biz beyze akım vererek duvarı yıkıp kapıyı açıyorduk.

**MOSFET'te:** Ortada ince bir sokak yok. Geniş, boşluklu bir arazi var ve elektronlar oradan geçemez. Yani **yol yok.** MOSFET'in işi, bu yolu **kendi inşa etmek.** Yolu inşa eden şey Gate.

Bütün konu şu soruya bağlı: Gate yolu nasıl inşa ediyor?

## 2. Parçalar

```
        GATE (metal plaka)
   ──────────────────────────
        CAM
   ──────────────────────────
   [ SOURCE ]  geniş P arazi  [ DRAIN ]
      (N)                       (N)
```

- **Source:** Soldaki N şehri, bol elektron var.
- **Drain:** Sağdaki N şehri, bol elektron var.
- **Ortadaki geniş P arazi:** NPN'deki gibi iki duvar var ama sokak ince değil, geniş. Elektron geçemez.
- **Üstte cam, camın üstünde Gate plakası.**

Gate'e hiçbir şey vermezsen iki şehir arasında yol yok. MOSFET kapalı.

## 3. Gate'e artı voltaj vermek: artı yüklü plaka

Elektrik alanı notunu hatırla: "Bir yük etrafına görünmez bir etki alanı yayar. Hareket etmesine gerek yok, var olması yeterli. Başka bir yükle karşılaşırsa kuvvet uygular, zıt yükleri çeker."

Gate'e artı voltaj verince Gate artı yüklü bir plaka olur ve etrafına alan yayar. Bu alan aşağıya doğru, camın içinden geçip silikona ulaşır. Eksi yükler (elektronlar) bu artı plakanın çekimini hisseder.

## 4. Cam: elektron geçmez, alan geçer

Bir benzetme: bir pencerenin dışında mıknatıs tutuyorsun, içeride demir tozları var. Mıknatıs camın ardından tozları çekiyor: tozlar cama doğru gelip yığılıyor ama camı geçemiyor. Camın varlığı mıknatısın çekimini engellemiyor.

Gate'te de aynısı oluyor. Cam elektronları durduruyor ama çekimi durdurmuyor. Elektronlar artı plakaya doğru çekiliyor, camın hemen altına gelip orada yığılıyor.

## 5. Elektronlar nereden geliyor?

Arazide neredeyse hiç elektron yok. Ama iki yanında iki kalabalık şehir var: Source ve Drain. Gate'in çekimi, bu şehirlerden elektronları camın altına çağırıyor.

```
   GATE (+)   ← çekiyor
   ──────────────── cam
   [S] e e e e e e e e e e [D]   ← elektronlar camın altında yığıldı
        geniş P arazi
```

Camın altında yığılan elektron şeridi, Source şehri ile Drain şehrini birbirine bağlıyor. **İnşa edilen yol bu.** Buna **kanal** diyoruz.

## 6. Yol var olunca ne olur?

Pilin eksisi Source'a, artısı Drain'e bağlıysa, elektronlar bu yoldan Source'tan Drain'e koşar. MOSFET açık.

Gate voltajını kesersen çekim kalkar, elektronlar şehirlerine dağılır, yol kaybolur. MOSFET kapanır.

## Özet

- NPN'de yol vardı ve biz duvarı yıkıyorduk. MOSFET'te yol yok, yolu **inşa ediyoruz.**
- Yolu Gate inşa ediyor: artı yüklü plaka etrafına alan yayıyor.
- Cam elektronu geçirmiyor ama alanı geçiriyor.
- Alan, Source ve Drain şehirlerinden elektronları camın altına çağırıyor.
- Yığılan elektronlar iki şehri bağlayan yolu (kanalı) oluşturuyor.


# MOSFET: Gate Voltajını Değiştirmek (Yol Ne Kadar Geniş?)

Önceki adımda Gate'in yolu inşa ettiğini gördük: alan elektronları camın altına çağırıyor, yığılan elektronlar Source ile Drain'i bağlıyor. Şimdi şuna bakalım: Gate'e verdiğin voltajı artırıp azaltırsan yol nasıl değişir?

## 1. Gate voltajı = yolun genişliği

Gate'in voltajı ne kadar yüksekse, artı plaka o kadar güçlü çeker ve camın altına **o kadar çok elektron** yığılır.

- Az elektron yığılırsa yol **ince bir patika** olur.
- Çok elektron yığılırsa yol **geniş bir otoban** olur.

Direnç notundaki otoban ve dar boğaz benzetmesi burada da geçerli. Yol genişse elektronlar rahat akıyor, dar ise zorlanıyor. Gate, yolun genişliğini ayarlayan kol.

## 2. Gate, ayarlı bir direnç gibi

Bu, senin direnç bilginle çok güzel birleşiyor. Kanal bir yol olduğu için bir **direnci** var:

- Yol dar: Direnç yüksek, akım az geçer.
- Yol geniş: Direnç düşük, akım kolay geçer.

Gate voltajını artırdıkça kanalın direnci düşüyor. Ohm Kanunu'ndan (I = V ÷ R), direnç düştükçe aynı voltajda akım artar. Yani **Gate, Source-Drain arasına bağlı bir ayarlı direncin kolu gibi.** Bu direnci akımla değil, voltajla ayarlıyorsun.

## 3. Üç hâl (NPN'deki gibi)

Örnek olarak eşik gerilimi 2 V olan bir MOSFET alalım. Aşağıdaki değerler yaklaşık bir fikir verir:

|Gate voltajı|Yol|Kanal direnci|Akım|
|---|---|---|---|
|0 - 2 V|Yok, elektronlar delikleri doldurmakla meşgul|Sonsuz|Yok|
|3 V|İnce patika|Yüksek|Az|
|5 V|Geniş yol|Düşük|Çok|
|10 V|Çok geniş otoban|Çok düşük|Yük ne kadar isterse|

**Kapalı:** Gate voltajı eşiğin altında. Camın altına gelen elektronlar boşluklara düşüyor, yığılma olmuyor, yol yok.

**Yarım açık:** Voltaj eşiğin biraz üstünde. Yol var ama dar, direnç yüksek.

**Tam açık:** Voltaj yüksek, yol geniş, direnç çok düşük.

NPN'de gördüğün gibi, tam açık hâlde akımı transistör değil devredeki yük (pil, direnç, motor) belirliyor. Burada da aynı.

## 4. Neden tam açık tutulur?

Anahtar olarak kullanıldığında MOSFET'i ya tamamen kapalı ya tamamen açık tutarız. Tam açıkken kanalın direnci çok düşüktür (genelde birkaç on miliohm, yani Ohm'un binde biri düzeyinde).

Bunun ne kadar önemli olduğunu Watt formülüyle görelim. Motor 2 Amper çekiyor ve MOSFET'in kanal direnci 0,02 Ω olsun:

1. MOSFET'in üzerine düşen voltaj: V = I × R = 2 × 0,02 = **0,04 Volt.**
2. MOSFET'in harcadığı güç: P = V × I = 0,04 × 2 = **0,08 Watt.**

Pilin voltajının neredeyse tamamı motora gidiyor, MOSFET'te sadece 0,08 W ısıya dönüşüyor. Ihtimalle dokununca ısındığını bile hissetmezsin. İşte bu yüzden MOSFET, güç kaynaklarında ve motor sürücülerinde bu kadar yaygın.

Yarım açık bırakırsan kanal direnci yüksek olur, üzerine büyük voltaj düşer, aynı akımda çok ısınır. Bu yüzden anahtar olarak çalışan MOSFET'te hedef kapıyı hızla tam açmak ya da tam kapatmaktır.

## 5. Önemli bir not: Eşik ile tam açılma aynı şey değil

"Eşik gerilimi 2 V" demek, MOSFET'in **açılmaya başladığı** voltaj demek, tam açıldığı voltaj değil. Eşiğin hemen üstünde yol çok dar. Tam açılması için Gate'e çok daha yüksek voltaj gerekiyor.

Bu yüzden iki tür MOSFET var:

- **Standart MOSFET:** Tam açılması için genelde yaklaşık 10 V ister.
- **Logic-level MOSFET:** 5 V ya da 3,3 V ile tam açılacak şekilde üretilmiş. Mikrodenetleyici pini doğrudan sürebilir. Datasheet'te adının sonunda ya da açıklamasında "logic level" yazar. Örnek: IRLZ44N.

Standart MOSFET'i pinin 5 V'una bağlarsan yol yarı açık kalır, MOSFET ısınır ve yük yeterince çalışmaz. Arduino ile kullanacaksan logic-level seç.

## Özet

- Gate voltajı arttıkça camın altına yığılan elektron artar, **yol genişler.**
- Yol genişledikçe kanalın **direnci düşer.**
- Gate, Source-Drain arasında voltajla ayarlanan bir direnç gibi.
- Üç hâl var: kapalı, yarım açık (dar yol, yüksek direnç), tam açık (geniş yol, çok düşük direnç).
- Anahtar olarak tam açıkta çalıştırılır. Direnç çok düşük olduğu için MOSFET'in üzerinde neredeyse hiç voltaj düşmez, çok az ısınır.
- Eşik gerilimi ile tam açılma voltajı farklıdır. Mikrodenetleyiciyle **logic-level** MOSFET kullan.

# MOSFET: Gerçek Devre (Motor, Pull-down, Diyot, Test)

Önceki adımda Gate voltajının yolun genişliğini ayarladığını gördük. Şimdi MOSFET'i gerçek bir devrede kullanalım: mikrodenetleyici pini ile motor sürmek, tıpkı NPN'de yaptığımız gibi.

## 1. Devreyi kuralım

Kullanacağımız parça: **N-kanal, logic-level MOSFET** (örneğin IRLZ44N). N-kanal, şimdiye kadar anlattığımız çeşit: N şehirleri, Gate'e artı voltajla açılır. Motor 12 V ve 2 A çekiyor.

- Pilin **artısı** → **motor** → MOSFET'in **Drain**'i
- MOSFET'in **Source**'u → pilin **eksisi**
- Pinin çıkışı → **Gate**
- Pinin **GND**'si → pilin **eksisi** (ortak eksi, NPN'deki gibi)
- Motorun uçlarına **geri tepme diyotu** (çizgili uç pilin artısı tarafında)
- Gate ile pilin eksisi arasına **10 kΩ direnç** (pull-down, aşağıda açıklıyorum)

Elektronların yolu NPN'dekinin aynısı: pilin eksisi → Source → kanal → Drain → motor → pilin artısı. Bacak isimleri değişti, hikâye aynı.

## 2. Pin 1 ve pin 0 olunca

**Pin 5 V verince:** Gate artı plaka olur, alan Source'tan elektronları camın altına çağırır, kanal oluşur, kanal direnci çok düşüktür (yaklaşık 0,02 Ω). Motor döner. MOSFET'in üzerine düşen güç: P = I² × R = 2 × 2 × 0,02 = **0,08 Watt.** Neredeyse hiç ısınmaz.

**Pin 0 V verince:** Alan kalkar, kanal dağılır, motor durur.

## 3. NPN'de beyz direnci vardı, burada ne var?

Gate akım çekmediği için NPN'deki gibi akımı sınırlayan bir beyz direncine ihtiyaç yok. Ama iki küçük direnç işe yarar.

**Gate'e seri küçük direnç (isteğe bağlı, 100-220 Ω):** Kondansatör notundaki dolum anını hatırla: boş bir kondansatör pile bağlanınca başta çok yüksek bir akım akar, sonra azalır. Gate de bir kondansatör gibi olduğu için, pin 5 V verdiği an Gate'i doldurmak için bir anlık akım patlaması çeker. Seri direnç bu patlamayı yumuşatır ve pini korur.

**Gate ile eksi arasına büyük direnç (pull-down, 10 kΩ):** Asıl önemli olan bu, aşağıda anlatıyorum.

## 4. Gate'i havada bırakma: Pull-down

Gate, bir kondansatörün artı odası gibi çalışıyor. Kondansatör notundaki **boşalma** mantığını hatırla: odadaki yükün gitmesi için iki bacağın dışarıdan bir yolla birleşmesi gerekiyor. Yol yoksa yük odada kalıyor.

Gate'in bağlı olduğu pin "giriş" moduna geçtiğinde (örneğin mikrodenetleyici yeni açılırken ya da program çalışmadan önce), pin ne 0 ne 5 V veriyor, Gate'e hiçbir şey bağlı değil, yani Gate **havada.** Bu durumda iki sorun çıkıyor:

1. Gate'e bir kere yük girmişse (statik elektrik, parmağını yaklaştırmak) boşalacak yol yok. Yük orada kalıyor ve MOSFET açık kalabiliyor.
2. Çevreden gelen minik parazitler Gate'i rastgele dolduruyor, motor kendi kendine titreyip dönebiliyor.

**Çözüm: Gate'i 10 kΩ'luk bir direnç üzerinden eksiye (GND) bağlamak.** Bu direnç, Gate'in plakasını eksiye çok yavaş, kontrollü bir yoldan bağlıyor:

- Pin bir şey vermiyorsa, Gate'teki yük bu dirençten eksiye akıp boşalıyor. Gate 0 V'a iniyor, MOSFET kapanıyor.
- Pin 5 V verdiğinde, 10 kΩ'un üzerinden eksiye sızan akım: I = 5 ÷ 10000 = 0,0005 A, yani **0,5 mA.** Pin bunu rahatça taşır, Gate'i 5 V'ta tutmaya engel olmaz.

Direnç notundaki pull-down dirençleriyle aynı mantık: "pin bir şey söylemezken Gate'in ne yapacağını belirleyen direnç".

## 5. Geri tepme diyotu: Yine gerekli

Motor bobin içeriyor, bobin notundaki voltaj tekmesi hâlâ geçerli. MOSFET kapanınca bobin akmaya devam etmek ister, B noktasında (Drain tarafında) voltaj fırlar ve MOSFET'i bozabilir. NPN'de yaptığımız gibi diyotu motorun uçlarına **ters yönde** bağlıyoruz: çizgili uç (N) pilin artısı tarafında, çizgisiz uç (P) Drain tarafında. Mantık ve çalışma şekli aynı.

## 6. MOSFET'in içindeki gizli diyot

İlk adımda gördüğün iki duvarı hatırla. Gövde (P) ile Drain (N) arasındaki duvar aslında bir **diyot.** Bu yüzden her N-kanal MOSFET'in içinde, Source'tan Drain'e akımı geçiren, ters yönü kapalı bir **gizli diyot** (body diode) var. Bunu bilmek iki yerde işe yarıyor:

- Pili ters bağlarsan akım bu gizli diyottan geçer ve MOSFET zarar görebilir.
- Multimetreyle testte bu diyodu göreceksin.

## 7. N-kanal ve P-kanal

NPN ile PNP'nin aynada görüntüsü olması gibi, MOSFET'in de iki çeşidi var:

- **N-kanal (şimdiye kadar anlattığımız):** Kanal elektronlardan oluşur. Source pilin eksisine bağlanır, Gate'e **artı** voltaj verince açılır. Motor, pilin eksi tarafında durur.
- **P-kanal (ayna görüntüsü):** Kanal boşluklardan oluşur. Source pilin artısına bağlanır, Gate'i Source'tan **daha düşük** voltaja çekince açılır. Yük, pilin artı tarafında durur.

Başlangıç için N-kanalı iyice oturtmak yeter. P-kanalı gerektiğinde, bu aynalama mantığıyla öğrenirsin.

## 8. Multimetreyle test

Bacak sırası modele göre değişir (datasheet'e bak). Multimetreyi diyot moduna al.

**Önce:** Üç bacağı bir an birbirine değdirip Gate'teki yükü boşalt. Aksi halde önceki ölçümden kalan yük MOSFET'i açık tutup yanıltıcı değerler gösterebilir.

|Kırmızı prob|Siyah prob|Sağlam MOSFET'te|
|---|---|---|
|Source|Drain|0,4 - 0,7 civarı (gizli diyot)|
|Drain|Source|OL|
|Gate|Source ya da Drain|OL (iki yönde de)|

**Arıza işaretleri:**

- Drain-Source arası iki yönde sıfıra yakın: **kısa devre.** MOSFET'in en sık ölme şekli budur.
- Gate ile diğer bacaklardan biri arasında bir değer görüyorsan: cam delinmiş, MOSFET bozuk.

## 9. Dikkat: Gate'in camı çok ince

Gate'in altındaki cam tabaka çok ince bir yalıtkan. Fazla voltaj binerse delinir (genelde ±20 V civarı, modele göre değişir). Statik elektrik de yeterli olabilir, bu yüzden MOSFET'leri çıplak elle fazla ovuşturma, lehimlerken dikkat et.

## Özet

- Devre: pil artısı → motor → Drain, Source → pil eksisi, Gate → pin. Pinin GND'si ortak eksi.
- Gate akım çekmediği için beyz direnci gerekmiyor. Seri küçük direnç (100-220 Ω) Gate'in dolum patlamasını yumuşatır.
- Gate'i **havada bırakma**: Gate ile eksi arasına 10 kΩ **pull-down** koy. Kondansatör gibi Gate'teki yük boşalacak yol bulmalı.
- Motor için geri tepme diyotu hâlâ şart.
- Her N-kanal MOSFET'te Source'tan Drain'e geçiren **gizli diyot** var.
- P-kanal, N-kanalın ayna görüntüsü (Source artıda, Gate'i düşürünce açılır).
- Testte Drain-Source arası kısa devre en yaygın arıza.

