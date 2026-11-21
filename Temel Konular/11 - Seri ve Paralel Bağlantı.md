
# Seri ve Paralel Bağlantı

Elektronik kartları tamir ederken, pil yataklarına bakar veya devre kurarken sürekli karşımıza çıkan iki kural vardır: **Seri Bağlantı** ve **Paralel Bağlantı**
### 1. Seri Bağlantı (Tek Sıra / Tek Yol)

Seri kelimesi "sıralı, ard arda"dan gelir.

- **Nasıl Bağlanır?** Elemanlar (örneğin iki pil veya iki lamba) **tek bir dosya halinde, arka arkaya** dizilir. Birinci elemanın çıkışı, ikincinin girişine bağlanır. Elektronların önünde **tek bir yol (tek bir koridor)** vardır.

- **Su Borusu Benzetmesi:** İki su pompasını veya iki musluğu **aynı borunun üzerine ard arda** takmak gibidir. Su mutlaka birinci musluktan geçmek zorundadır, başka çaresi yoktur; oradan çıkıp hemen ikinci musluğa girer.
#### Seri Bağlantının Altın Kuralları:

1. **Tek Yol Kuralı (Kopukluk Her şeyi Bitirir):** Elektronların izleyeceği tek bir hat olduğu için, o zincirin herhangi bir yerinde en ufak bir kopukluk (açık devre) olursa, **tüm sistem anında durur.** (Eski tip yılbaşı ağacı ışıkları gibi; lambalardan biri patlayınca bütün dizi söner).

2. **Voltaj (Basınç) Katlanır:** Pilleri seri bağladığında (örneğin iki tane 1.5 Volt'luk pili arka arkaya dizdiğinde), birinci pilin ittiği elektronlar ikinci pilden de geçer ve **itme gücü (voltaj) iki katına çıkar** ($1.5V + 1.5V = 3V$).
### 2. Paralel Bağlantı (Çoklu Yol / Otoban Kolları)

Paralel kelimesi, yan yana uzanan ve asla kesişmeyen yolları hatırlatsın.

- **Nasıl Bağlanır?** Elemanlar yan yana konur. Hepsine giden yol ayrı ayrıdır ama girişleri bir noktada, çıkışları başka bir noktada **ortak birleşir.** Elektronlar yol ayrımına geldiğinde "Ben bu koldan gideyim, arkadaşım da diğer koldan gitsin" diye kollara ayrılır.

- **Su Borusu Benzetmesi:** Ana borunun bir anda üç ayrı ince boruya (musluğa) ayrılması ve sonra tekrar tek boruda birleşmesi gibidir. Su, o üç musluktan **aynı anda** akar.
#### Paralel Bağlantının Altın Kuralları:

1. **Bağımsızlık Kuralı (Biri Bozulursa Diğeri Çalışır):** Kollar ayrı olduğu için, kollardan birindeki lamba patlasa veya kablo kopsa bile, diğer koldaki elektronlar akmaya devam eder. Evimizdeki prizler ve lambalar **paralel** bağlıdır; mutfaktaki lamba patlasa odadaki lamba yanmaya devam eder.

2. **Voltaj Değişmez, Süre Uzar:** Pilleri paralel bağladığında voltaj artmaz (örneğin iki tane 1.5V pil yine 1.5V verir) ama **su deposu büyümüş olur.** Elektronlar paylaşıldığı için o pil çok daha uzun süre dayanır (akım kapasitesi / Amper-saat artar).
### Tamir Masasından Özetle Farkı:

- **Seri Bağlantı:** **"Tek yol, artan voltaj."** (Voltajı yükseltmek istiyorsan pilleri arka arkaya dizersin).

- **Paralel Bağlantı:** **"Çoklu yol, bağımsız kollar, ortak güç."** (Cihazların aynı voltajı almasını ve birbirine bağımlı olmamasını istiyorsan paralel bağlarsın).

