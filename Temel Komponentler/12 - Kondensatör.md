
# Kapasitör(Kondensatör/Sığaç)

### Kondensatör Tam Olarak Nedir? (Senin Modelinle)

Kondensatör, büyük pilin ana odalarının yanı içine yerleştirilmiş **minik, özel bir oda çiftidir.**

İç yapısına baktığında şunları görürsün:

1. **Birinci Oda (Eksi Levha):** Elektronların doldurulacağı minik bir oda.

2. **İkinci Oda (Artı Levha):** Elektronların çekileceği, karşıdaki diğer minik oda.

3. **Aradaki Yalıtkan Duvar:** Bu iki minik odayı birbirinden ayıran, elektronların asla karşıya geçmesine izin vermeyen **aşırı kalın/yalıtkan bir duvar**.

İşte kondensatör, bu iki minik odadan ve aralarındaki o geçilmez duvardan ibarettir.

### Adım Adım Kondensatörün Yaşamı

#### 1. Dolum Anı (Şarj Olma)

Sen kondensatörü ana bataryaya (veya devreye) bağladığında ne olur?

- Büyük pilin eksi odasından çıkan elektronlar, kondensatörün **birinci odasına (eksi levhasına)** doğru akmaya başlar.

- Elektronlar o odaya dolar, dolar, dolar...

- Ama tam o sırada aradaki o **yalıtkan duvar** karşılıklarına dikilir! Elektronlar karşı odaya **asla geçemez**.

- Geçemedikleri için birinci odanın içinde üst üste yığılırlar, sıkışırlar ve tıpkı büyük pildeki gibi müthiş bir **gerginlik ve basınç (voltaj)** yaratmaya başlarlar.

#### 2. Durma Noktası (Oda Doldu!)

- Elektronlar o minik odada o kadar çok sıkışır ki, artık dışarıdan gelen itme gücü ile içerideki sıkışma **dengeye gelir** (Basınç eşitlenir).

- Kondensatör der ki: _"Benim bu odam tamamen doldu, artık içeriye tek bir elektron bile sığdıramam!"_
 
- Ve elektron akışı **kendiliğinden durur**. Kondensatör şu an tamamen doludur; içinde sıkışmış bir enerji (basınç)le öylece bekler. (DC akım için artık orada sanki kopuk bir yol varmış gibi davranır).
#### 3. Boşalma Anı (Ani Fışkırma / Yüksek Amper)

İşte en heyecanlı kısım burası! Cihazda o anlık enerjiye ihtiyaç duyulduğunda (örneğin kameranın tuşuna bastığında veya çip aniden akım çektiğinde) ne olur?

- O minik odanın dışındaki kapı açılır ve elektronlar için kaçış yolu (devre) tamamlanır.

- Birinci odada aradaki duvardan ötürü sıkışıp kalmış o milyonlarca elektron, _"Yaşasın, sonunda kaçıyoruz!"_ diyerek **aynı anda, saniyenin binde birinde (şimşek gibi)** o kapıdan dışarı fışkırır.

- Bütün kalabalık aynı anda dışarı atıldığı için, o an oradan **devasa bir Amper (akım patlaması)** geçer.
 
- Oda boşalır, içindeki gerginlik biter ve depo eski sakin haline döner.

### Senin Modelinle Özetle Kondensatör:

- **Pil:** Büyük, kimyasal olarak uzun süre elektrik üreten ana oda sistemi.

- **Kondensatör:** Arasında yalıtkan duvar olan iki minik oda. Elektriği kimyasal yolla değil, **elektronları o odada fiziksel olarak sıkıştırıp gerginlik yaratarak** anlık depolar.

- **Şarj Olma:** Elektronların o minik odaya dolup sıkışması ve basıncın tepeye çıkması.

- **Boşalma:** Kapı açılınca o sıkışan elektronların **hepsinin birden (yüksek amperle)** dışarı fışkırması.

### 4. Nerelerde ve Neden Kullanılır? (Hayati Görevleri)

Tamir masasında veya elektronik devrelerde kondensatörü her yerde görmemizin 3 ana sebebi vardır:
#### A. Ani Güç Patlamaları (Kamera Flaşı Örneği)

Telefonunla karanlıkta fotoğrafl çekerken flaş patlar. Flaş o an devasa bir enerjiye ihtiyaç duyar. Eğer o enerjiyi direkt pilden çekmeye kalksaydık pil zorlanır veya yetmezdi.

- Pil, aradaki kondensatörü yavaş yavaş doldurur (depoyu şişirir).

- Fotoğraf tuşuna bastığın an, kondensatör o biriktirdiği tüm elektriği **tek bir salisede** flaşa fışkırtır ve o göz kamaştırıcı ışık patlar!
#### B. Akımı Düzeltmek (Filtreleme - AC'yi DC Yaparken Görmüştük!)

Hatırlarsan AC'yi DC'ye çevirirken kondensatörlerden bahsetmiştik.

- Şehir elektriği veya doğrultulmuş akım inip kalkarken (dalgalıyken), kondensatör akım yükseldiğinde **fazla elektriği içine çeker (depolar)**, akım düşmeye başladığında ise **içindeki suyu salarak o çukurları doldurur.**
 
- Böylece akıştaki tüm sarsıntıları yok eder, ortalığı dümdüz pürüzsüz bir nehire çevirir. Buna elektronikçiler **"Filtreleme"** der.

#### C. Gürültüyü ve Parazitleri Temizlemek

Elektronik kartlarda çipler saniyede milyarlarca işlem yapar. Bu sırada hatlarda minik minik voltaj sıçramaları (elektriksel gürültüler) oluşur. Çiplerin kafası karışmasın diye besleme bacaklarının hemen yanına minik kondensatörler konur. O kondensatörler gelen o ani parazit voltajını hemen yutup içine hapsederek çipi korur ve akımı tertemiz tutar.

### Kondensatörün Ölçü Birimi: Farad (F)

Direncin birimi Ohm'du, Voltajınki Volt'tu. Kondensatörün kapasitesini (ne kadar su depolayabileceğini) ölçen birim ise **Farad (F)**'dır.

Ancak **1 Farad** devasa bir depodur! Günlük elektronik kartlarda karşımıza çıkan kondensatörler o kadar büyük değildir. Genellikle mililyonda biri ($\mu F$ - Mikrofarad), milyarda biri ($nF$ - Nanofarad) veya trilyonda biri ($pF$ - Pikofarad) şeklinde minik değerlerde olurlar.



## Ne Zaman Kondensatör Kullanmalıyım?

Bir devrede kondensatör kullanmanın (veya kartta aramanın) **4 temel sebebi** vardır:
### 1. Voltaj Düşmelerini Engellemek (Filtreleme / Besleme Desteği) - _En Yaygın Sebep_

Elektronik kartlarda (özellikle anakartlarda) işlemciler veya çipler anlık olarak çok büyük işler yapmaya başlar ve bir anda normalden daha fazla akım çekerler.

- **Sorun:** Akım birden artınca, o hat üzerindeki **voltaj (basınç) anlık olarak düşmeye başlar.** Voltaj düşerse çipin kafası karışır ve bilgisayar aniden kilitlenir veya kapanır.

- **Kondensatörün Çözümü:** Çipin hemen besleme bacağının yanına minik bir kondensatör (su deposu) koyarlar. Sistem normal çalışırken o depo dolar. Çip aniden fazla akım çekip voltajı düşürmeye çalıştığı an, o kondensatör hemen **içindeki suyu (elektriği) anında fışkırttırarak voltajın düşmesine izin vermez,** ortalığı hep sabit tutar.

- _Tamirci Notu:_ Anakartlarda bozulup şişen (üstü kubbe gibi kabaran) o silindir kondensatörler işte bu yüzden patlar; yıllarca o anlık voltaj düşmelerini engellemekten yorulup delikleri delinmiştir!
### 2. Elektriksel Gürültüyü (Parazitleri) Temizlemek

Elektronik kartların içi milyarlarca minik sinyalle doludur. Bu sinyaller birbirineminik elektriksel gürültüler (istenmeyen zıplamalar) bulaştırabilir.

- **Kondensatörün Çözümü:** Hattın üzerine yerleştirilen kondensatör, o istenmeyen yüksek frekanslı minik voltaj zıplamalarını (gürültüyü) yakalar ve **doğrudan Eksi'ye (GND'ye) akıtıp yok eder.** Sadece temiz ve düzgün sinyalin geçmesine izin verir. Buna "Bypass" veya "Decoupling" denir. 
### 3. Ani Güç Patlamaları (Kamera Flaşı, Hoparlör Basları vb.)

Bazı cihazlar normalde az elektrik harcar ama aniden devasa bir güce ihtiyaç duyar.

- **Kondensatörün Çözümü:** Pil veya adaptör o kadar büyük anlık akımı tek başına veremez. Araya büyük bir kondensatör konur. Kondensatör yavaş yavaş dolar (depoyu şişirir) ve ihtiyaç anında o birikmiş gücü **tek bir salisede şimşek gibi fışkırtarak** o işi yapar. (Örn: Fotoğraf makinesi flaşı, ses sistemlerindeki derin ve güçlü "bass" patlamaları).

### 4. DC'yi Engellemek, AC'yi Geçirmek (Sinyal Ayrıştırma)

Kondensatörün yapısını hatırlasana: _İki levha ve aralarında elektrik geçirmeyen yalıtkan bir duvar var._

- Bu yapı sayesinde kondensatör harika bir filtre karakteri kazanır:  
    - **Sabit DC elektrik (düz akım)** aradaki o duvara takılır ve **asla karşı tarafa geçemez.** (Yol kapalıdır).

    - Ama **dalgalı AC sinyaller** (örneğin kulaklığa giden müzik ses dalgaları) karşı tarafa etki yoluyla aktarılabilir.

- Bu sayede ses kartlarında veya radyo devrelerinde, akımların birbirine karışmasını engellemek için sinyal yollarının üzerine kondensatörler yerleştirilir.

### Özetle; Pratikte Ne Zaman Kullanmalısın?

Bir devre tasarlarken veya tamir ederken şu durumlarda kesinlikle kondensatör kullanmalısın:

1. **"Bu entegrenin besleme bacağı var, ya anlık akım çekerse voltaj düşerse?"** diyorsan hemen yakınına bir kondensatör koymalısın (Güç kararlılığı için).

2. **"Şehir şebekesinden gelen veya adaptörden çıkan akım çok dalgalı, bunu düzleştirmem lazım"** diyorsan doğrultma devresinin arkasına büyük bir kondensatör eklemelisin.

3. **"Hattın üzerindeki o parazitleri temizlemem lazım"** diyorsan GND'ye bağlanan minik kondensatörler kullanmalısın.

## Kondensatör Devreye Nasıl Bağlanır?


Kondensatörün devreye nasıl bağlanacağı, **ne amaçla kullanacağına** ve kondensatörün **türüne** göre değişir. Ancak elektronik kartlarda ve tamir masasında karşımıza çıkan senaryolara göre bunu en sade haliyle iki ana başlıkta inceleyebiliriz:
### 1. En Yaygın Yöntem: Paralel Bağlantı (Voltajı Sabitlemek ve Filtrelemek İçin)

Anakartlarda, çiplerin besleme bacaklarının yanında gördüğümüz kondensatörlerin neredeyse hepsi **paralel** bağlanır.

- **Nasıl Bağlanır?** Güç hattı ile Eksi hattın (**GND**'nin) tam ortasına, adeta bir köprü gibi bağlanır. Kondensatörün bir bacağı elektriğin geldiği **Artı (+ / VCC)** hatta, diğer bacağı ise senin o harika modelindeki Eksi Odaya yani **GND (-)** hattına lehimlenir.

- **Neden Böyle Bağlanır?** Çünkü bir "su deposu" görevi görebilmesi için ana su borusunun (güç hattının) hemen yanında durması gerekir. Voltaj anlık olarak düşmeye başladığında, paralel bağlı o depo hemen devreye girip suyunu (elektronlarını) o hatta fışkırttığı için çip etkilenmez.

### 2. Sinyal Yollarında: Seri Bağlantı (AC'yi Geçirip DC'yi Kesmek İçin)

Eğer amacın akımı depolamak değil de, iki devre elemanı arasında gider-gelir sinyalleri (örneğin kulaklığa giden ses dalgalarını) ayırmaksa **seri** bağlanır.

- **Nasıl Bağlanır?** Elektriğin aktığı kablonun tam ortasını kesersin ve kondensatörü **araya bir durak gibi** yerleştirirsin. (Yolun bir tarafı kondensatöre girer, diğer tarafı kondensatörden çıkıp yola devam eder).

- **Ne Olur?** Hatırlasana; kondensatörün içinde yalıtkan bir duvar vardı. Sabit DC (düz akım) o duvara çarpıp kalır, karşıya asla geçemez. Ama dalgalı AC sinyaller (ses dalgaları vb.) aradaki o yalıtkan duvarı etki yoluyla aşıp karşı tarafa geçebilir.

### ⚠️ Hayati Kural: Artı ve Eksi (Kutupluluk) Mabelleği!

Kondensatörleri devreye bağlarken bilmen gereken en kritik kural **kutuplardır**. Kondensatörler ikiye ayrılır:

1. **Kutupsuz Kondensatörler (Örn: Seramik Kondensatörler - Minik mercimek tanesi gibidirler):** Bunların artı veya eksi bacağı yoktur. Hangi yöne takarsan tak, kusursuz çalışır. Yön derdin yoktur.

2. **Kutuplu Kondensatörler (Örn: Silindir Elektrikli Kondensatörler - Üstünde kılıf olanlar):** İşte bunlarda **artı (+) ve eksi (-) bacaklar hayatidir!**

    - Kondensatörün gövdesinin üzerinde genellikle eksi (-) tarafa bakan bir şerit veya ok işareti bulunur.
    
    - **Asla ters bağlamamalısın!** Eğer kutuplu bir kondensatörün artı bacağını GND'ye (eksiye), eksi bacağını artıya bağlarsan; içindeki o "iki oda ve yalıtkan duvar" dengesi darmadağın olur, kondensatör saniyeler içinde aşırı ısınır, şişer ve **"Güm!" diye patlar.**

### Özetle Tamir Masası Kuralı:

- Kart üzerindeki besleme hatlarını kararlı tutmak istiyorsan kondensatörü **Artı ile GND arasına (paralel)** bağlarsın.

- Kutuplu kondensatör takarken üzerindeki **eksi çizginin** kart üzerindeki GND (eksi) hattına baktığından yüzde yüz emin olursun!

