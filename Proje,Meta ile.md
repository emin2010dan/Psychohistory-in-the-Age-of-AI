# Yapay Zeka ile Psikotarih Mümkün mü

**Katkıda bulunan: Meta AI (Muse Spark)**

[Read this article in English](https://github.com/emin2010dan/Psychohistory-in-the-Age-of-AI/blob/main/Project%20with%20Meta.md)

Psikotarih, Asimov'un romanlarında kaldı sanılıyordu. Oysa bugün yapay zekanın insan toplumuna girmesiyle, bireysel psikolojiyi değil, milyonların birlikte nasıl davrandığını modellemek zorundayız. Aksi halde, sadece geleceği görmekle kalmayız, onu yanlış yönetiriz.

Bu yazı, bir beyin fırtınasının notlarıdır. Amaç kehanet değil, müdahale imkanı veren bir bilim iskeleti kurmaktır. Çünkü işsizlik, stagflasyon ve radikal anti-AI popülizm riski zaten kapıda. Bu tehlikeyi daha önce anlattığım dijital yıkım senaryosunda özetlemiştim: [Dijital Yıkım Uyarısı](https://medium.com/p/8cea2a1bce13). Çözüm, geleceği seyretmek değil, umut üreten bir ekosistem kurmaktır. O ekosistemin ilk taslağı da burada: [Distributed Mind Protocol](https://medium.com/@emin2010dan/distributedmind-protocol-232d67221e33).

## Neden yapay zeka psikotarihe muhtaç

Yapay zeka tek bir insanla konuşmaz. Milyonlarca karara aynı anda dokunur, beklentileri senkronize eder. Psikoloji n=1 için çalışır, psikotarih n=milyon için gerekir. Eğer AI toplumun dalgalarını okumazsa, motivasyon basıncını umut yerine yıkıma çevirir.

## Temel fikir: tarih doğrusal değil, dalgalı

Hayat ReLU gibi tek yönlü büyümez. Her olgu bir dalgadır ve her dalganın üç özelliği vardır:
- frekans
- genlik
- sönüm

Yanlış yaptığımız şey, dalgayı takvim yılıyla ölçmekti. Dalga suda farklı, havada farklı yayılır. Tarihte de bilgi hızı değişir. Roma'da para basmak için gümüş eritmek gerekirdi, bugün bir tuşa basmak yeter. Bu yüzden olay zamanını kullanıyoruz:

$$\tau = \int_0^t v(s) \, ds$$

$v(s)$ o çağdaki bilgi ve kaynak iletim hızıdır.

## Parametreler ve nedenleri

Formüllerin altında ezber değil, gözlem var.

**1. Duygu modu $m$**
Toplumlar üç halde dolaşır. Bunu sahada gördük.
- $m=1$ kıtlık, kahraman çağı. Fedakarlık ucuz.
- $m=2$ onarım, kural çağı. Öngörülebilirlik istenir.
- $m=3$ bolluk, para çağı. Fedakarlık pahalı.

Aynı insanlar 30 yıl arayla farklı tepki verir çünkü mod değişir.

**2. Kültürel kod $C$**
Toplumu homojen sayarsak model çöker. Kod dört eksendir:
- $C_{adapt}$: adapte olma hızı. Türk yüksek, Ming Çin düşük.
- $C_{güven}$: merkeze güven. Yastık altı altın bunun ölçüsüdür. Türkiye'de hane altının 3.000 ila 5.000 ton arası olduğu tahmin ediliyor.
- $C_{merak}$: risk ve keşif iştahı.
- $C_{aşiret}$: bağlılığın merkeze mi kabileye mi aktığı.

**3. Kohort etkisi**
İnsan 40'tan sonra kolay değişmez. Kodu belirleyen 7-17 yaş arasıdır. Bu yüzden:
- 11 yıl = bir genç nesil
- 22 yıl = üretken çekirdek
- 33 yıl = karar verici kadro

1980 müdahalesi + 22 yıl = 2002. Tesadüf değil, kohort değişimi.

**4. Motivasyon basıncı $M$**
Düdüklü tencere. İhtiyaç açığı ile konforun farkı:

$$M = (\text{açık}) \cdot C_{adapt} \cdot (1 - \text{konfor})$$

Çin'de bugün açık enerji, ABD'de açık ucuz emek. İkisi de aynı basıncı farklı vanadan boşaltacak.

**5. Umut $H$**
$M$ tek başına yıkıcı olabilir. Yönü $H$ verir. $H$ -1 ile +1 arasıdır.
- Ölçümü: beyin göçü hızı, sermaye kaçışı, startup kurulum hızı. Doğum oranı değil, çünkü geç gelir.
- $H$ negatifse motivasyon ülkeyi terk eder. Pozitifse inşa eder.

Etki:
$$\text{etki} = M \cdot H$$

**6. Birleştirici $U$ ve ateşleyici $P$**
Ortak düşman çan eğrisini düzleştirir. $U$ yükselince kültürel farklar susar. Kıbrıs 1974, İran bugün bunun örneğidir.

Sistem stresi $S$ maksimuma gelince, birileri yapay kıvılcım üretir. Kara kuğu beklemeye gerek yok, beyaz kuğu boyanır:

$$P(\text{ateşleyici}) = 1 - e^{-\lambda S}$$

## Önerilen formül iskeleti

Tek bir denklem yok, katmanlı bir yapı var. Bu makaledeki formüller Meta AI tarafından bu tartışma için önerilmiştir.

Temel dalga:
$$x(\tau) = A e^{-k\tau} \sin(\omega\tau + \phi)$$

Duygu modu eklenince:
$$x_m(\tau) = A(m) e^{-k(m,i)\tau} \sin(\omega\tau + \phi)$$

Kültürel kod eklenince:
$$x_c(\tau) = A(m) C_{adapt} e^{-k(m,i)\tau / C_{güven}} \sin(\omega C_{merak}\tau + \phi)$$

Motivasyon ve umut yön verince:
$$x_{yeni} = x_c + \beta M H + \epsilon$$

$\epsilon$ küçük rastgelelik değil, zayıf bağların kırıldığı yön.

## Geliştirme adımları

1. **Veri topla ama etiketle.** Her olaya A, B, C kaynak damgası koy. A: davranış, B: düşman anlatısı, C: hatırat. TÜİK yerine elektrik tüketimi, altın ithalatı, evlilik cüzdanı.
2. **Toplumu böl.** Kültürel kod ve yaş kohortuna göre ayır. Sahil 1975 doğumlu ile iç Anadolu 1998 doğumlu aynı formülde çalışmaz.
3. **Geri test yap.** 1900-1950 ile eğit, 1950-1980 ile dene. Hata sistematikse parametre eksik demektir.
4. **Müdahale simüle et.** $H$'yi -0.3'ten +0.4'e çekecek bir transfer mekanizması ne olur? Yaşlı sermayesinden genç emeğine puan sistemi gibi.
5. **Mükemmel bekleme.** Veri bozuk. Amaç %100 tahmin değil, yanlışlanma hızını düşürmek.

## Sonuç

Psikotarih falcılık değildir. Bir toplumda umut kalmadığında motivasyonun yıkıma döndüğünü, ortak düşmanla birleşmenin geçici olduğunu, kültürel kodun dalgayı nasıl kırdığını sayıya döken bir araçtır.

Yapay zeka bu aracı kullanırsa, işsiz kalan mühendisi virüs yazmaya değil, mikro buluşa yönlendiren bir ekosistem kurabilir. O ekosistemin ekonomik iskeleti zaten önerildi. Şimdi sıra, bu formülleri kirli veride test edip, her başarısızlıkta bir parametre daha eklemekte.

Geleceği görmek yetmez. Onu, küçük kızın dondurma isterken gülümsemesi kadar basit ama güçlü bir umutla değiştirmek zorundayız.
