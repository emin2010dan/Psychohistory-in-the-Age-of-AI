# Psikotarih: Yapay Zeka ile İnsan Toplumunu Anlamak ve Geleceği Şekillendirmek

**Yazar:** Emin  
**Katkıda Bulunan:** Claude Sonnet (Anthropic) — Bu makaledeki matematiksel formüller ve model mimarisi Claude tarafından geliştirilmiştir.

---

## Neden Psikotarih?

Isaac Asimov, *Foundation* serisinde "psikotarih" adını verdiği hayali bir bilim dalını tanımladı: büyük insan topluluklarının davranışını istatistiksel olarak modelleyen, geleceği olasılıksal olarak hesaplayabilen bir bilim. Asimov bunu kurgu olarak yazdı. Ama bugün, büyük dil modelleri, küresel veri akışları ve hesaplama gücündeki artışla birlikte, bu fikir artık salt kurgu değil.

Psikoloji bireysel insanı anlamak için yeterli bir araçtır. Ama insan *toplumlarını* anlamak için psikoloji yetmez. Bir bireyin neden depresyona girdiğini açıklayabilirsiniz; ama bir toplumun neden çöküşe geçtiğini, neden isyan ettiğini, neden yenilik ürettiğini ya da neden durgunlaştığını açıklamak farklı bir bilim gerektirir. Bu bilimin adı ne olursa olsun — psikotarih, tarihsel dinamik, sosyo-kompleksite — ihtiyacı gerçektir.

Yapay zekaların insan toplumunun bir parçası haline geldiği bu dönemde bu ihtiyaç daha da kritik bir anlam kazanmaktadır. Yapay zeka işsizliği yaratıyor, ekonomik dengesizliklere yol açıyor. İşsiz kalan kitleler radikal, yapay zeka karşıtı politikacıları destekleyecek. Daha da tehlikelisi, işsiz kalan bilgisayar mühendisleri yerel yapay zeka modellerini kullanarak dijital altyapıyı hedef alan saldırılar geliştirebilecek — bu tehlikeyi daha önce ayrıntılı olarak ele aldım: [Yapay Zekalı Virüsler: Gelen Fırtına ve Hazırlık](https://medium.com/@emin2010dan/yapay-zekal%C4%B1-vir%C3%BCsler-gelen-f%C4%B1rt%C4%B1na-ve-haz%C4%B1rl%C4%B1k-8cea2a1bce13).

Bu felaketi önlemenin en güçlü aracı, toplumsal dinamikleri anlayan ve geleceğe müdahale imkânı sunan bir psikotarih bilimidir.

---

## Mevcut Örüntüler: Önceki Çalışmalar

Psikotarih sıfırdan başlamıyor. Tarih boyunca araştırmacılar toplumsal örüntüleri anlamlandırmaya çalışmıştır:

**Peter Turchin — Kliodinamik:** Toplumsal uyum ve çözülme döngülerini matematiksel olarak modelleyen ilk sistematik girişimlerden biri. Şiddetin yaklaşık 50 yıllık döngüler izlediğini göstermiştir.

**Ibn Haldun — Asabiye Teorisi:** 14. yüzyılda, toplumsal dayanışmanın (asabiye) imparatorlukların yükseliş ve çöküşünü belirlediğini ortaya koydu. Tarihin ilk döngüsel analizi.

**Kondratiev Dalgaları:** Ekonomik aktivitenin 40-60 yıllık büyük dalgalar halinde hareket ettiğini gösterir. Teknolojik paradigmaların doğuşu, olgunlaşması ve çöküşüyle örtüşür.

**Strauss-Howe Kuşak Teorisi:** Her ~80 yılda bir tekrarlayan dört nesil arketipi. Kriz, yükseliş, uyanış, çözülme döngüsü.

**Hegemonik Döngüler:** Portekiz → Hollanda → İngiltere → ABD biçiminde ilerleyen 100-150 yıllık hegemonya değişimi.

Bu çalışmaların ortak zayıflığı: *post-hoc* analizdir. Olmuş olayları açıklar ama öngörü üretmekte yetersiz kalır. Asıl hedef, dalgaları daha oluşurken tespit etmektir.

---

## Metodolojinin Temeli: Örüntü Madenciliği

Psikotarihin ilk adımı, tarihteki tekrarları tespit etmektir. Buna **örüntü madenciliği** adını veriyorum.

Örüntü madenciliğinde en büyük hata, dalgaların boyunu salt zamana göre ölçmektir. Oysa dalgalar ortam değiştiğinde farklı davranır — tıpkı denizde sığ sulara giren dalga gibi.

Roma'da parasal genişleme için eski gümüş paraları toplamak, bakır karıştırıp yeniden basmak gerekiyordu — bu süreç onlarca yıl alırdı. Bugün merkez bankasının dijital bir emriyle aynı etki dakikalar içinde yaratılabilir.

Bu farkı modellemek için **ortam iletkenliği** kavramı gereklidir:

```
t_normalize = t_gerçek × İletkenlik(dönem)

İletkenlik(t) = f(haberleşme_hızı, para_dolaşım_hızı, 
                  nüfus_yoğunluğu, kurumsal_kapasite)
```

Normalize edilmiş zaman kullanıldığında, Roma'nın 80 yıllık çöküş döngüsü ile modern bir ekonominin 8-12 yıllık çöküş döngüsü karşılaştırılabilir hale gelir.

### Çökmemiş Örneklerin Önemi

Klasik analizlerin metodolojik zayıflığı şudur: yalnızca çöken örnekleri incelerler. Oysa psikotarihin asıl değeri, neden bazı sistemlerin aynı aşamalardan geçmesine rağmen çökmediğini anlamaktır.

İngiltere sanayisini kaybetti ama finansı merkez yaparak ayakta kaldı. Almanya hiperenflasyona girdi ama kira gelirine endeksli Rentenmark'ı bastı ve döngüyü kırdı. Japonya faizleri sıfıra indirdi — bu müdahale işe yaramadı çünkü para yanlış aktöre aktı.

Bu örneklerden çıkan kritik ders: **müdahalenin varlığı yetmez, hangi dalgaya, hangi fazda uygulandığı belirleyicidir.**

---

## Veri Kalitesi: Manipüle Edilemeyen Proxy Veriler

Geçmiş bilgilerin güvenilirliği kritik bir sorundur. Tarihi kazananlar yazar, olayları kendilerini aklayacak biçimde şekillendirir. Bu nedenle her veri noktasına bir **doğruluk katsayısı** atanmalıdır:

```
Güvenilirlik = f(kaynak_bağımsızlığı, zaman_yakınlığı,
                  iktidar_çıkarı_çatışması, 
                  çapraz_doğrulama_sayısı)
```

Daha da önemlisi: insanların **ne dediğine değil ne yaptığına** bakılmalıdır. İnsanlar korkudan mutlu olduklarını söyler ama evlenmez ve çocuk yapmaz. Resmi enflasyon verileri gerçeğin yarısını yansıtabilir — ama çarşı fiyatları yalan söylemez.

Türkiye'nin en yetenekli ekonomistlerinden birinin sırrı buydu: lüks turşu satışlarını takip ederek ekonomik tahminler yapıyordu. Baskı altında ilk kesilen harcamalardan biri. İktidar bunu manipüle edemez.

**Manipüle edilemeyen proxy verilere örnekler:**
- Kuyumcu altın satış hacimleri (kuruma güvensizliğin göstergesi)
- Pasaport başvuru sayıları (sistem terk etme iradesi)
- Bebek bezi ve okul kaydı istatistikleri (demografik umut)
- Startup kurulum hızı (üretken umut)
- Yurt dışı üniversite kayıtları (beyin göçü eğilimi)

---

## Toplumsal Duygu Modları: İnsan Davranışının Kalbine Girmek

Psikotarihin en zor parçası insan davranışıdır. Oyun teorisi insanların rasyonel, çıkar maksimizasyonu yapan varlıklar olduğunu varsayar. Bu, az sayıda zeki birey için geçerli olabilir. Ama büyük topluluklar için değil — topluluklar çoğunlukla duygusal kararlar alır ve mantığı bu kararları desteklemek için kullanır.

Toplumlar, çevre koşullarına göre üç temel duygu modunda davranır:

**Mod 1 — Kahraman/Kriz Modu:** Aşırı zorlu koşullarda (ekonomik çöküş, savaş) toplumda güçlü figürler öne çıkar. İnsanlar bu figürlerin peşinden gider, fedakarlığa hazır olurlar. Bu dönemde kolektif eylem kolaydır.

**Mod 2 — Kuralcı/İnşa Modu:** Kriz atlatıldığında kahraman figürü yerini kuralcılara bırakır. Kurumlar inşa edilir, toplumsal sözleşme oluşturulur. İnsanlar kurallara uymaya daha yatkındır.

**Mod 3 — Paragöz/Bolluk Modu:** Toplumsal huzur sağlandığında bireysel çıkar ve zenginleşme ana motivasyon haline gelir. Kurallara uymak zorlaşır, gelir eşitsizliği büyür, kurumsal çürüme artar. Bu dönem kendi sonunu hazırlar — tekrar Mod 1'e geçiş kaçınılmaz hale gelir.

Bu modlar hem büyük dalgalar hem de küçük tali dalgalar biçiminde çalışır. Ana toplumsal dalga Mod 2'deyken kısa bir kriz Mod 1 tali dalgası yaratabilir. Ama Mod 3'teyken gelen kriz farklı sonuç verir: kahraman figürü sistemi onarmak için değil, ele geçirmek için kullanılır.

```
Mod_filtresi = {
  Mod_1: fedakarlık_eşiği↓, kolektif_eylem↑, kurumsal_güven_değişkeni
  Mod_2: kural_uyumu↑, uzun_vadeli_tasarruf↑, kurum_kurma_hızı↑
  Mod_3: gelir_eşitsizliği↑, tüketici_kredisi↑, kuruma_güvensizlik↑
}
```

---

## Kültürel Kod: Formülün Gizli Değişkeni

Aynı ekonomik şok farklı toplumlarda farklı sonuçlar üretir. Bunun nedeni **kültürel koddur** — her toplumun binlerce yıllık tecrübeden oluşan karakteristik tepki kalıplarıdır.

Çin büyük okyanus gemileri yapabilmişti, Afrika kıyılarına ulaşabilmişti. Ama tek bir imparatorluk emriyle bu sefer durdu ve gemileri yaktı. İspanya çok daha küçük gemilerle bilinmez sulara açıldı. Fark teknolojide değil, kültürel kottaydı: Konfüçyüs dünya görüşünde dışarısı tehdit, içerisi yeterliydi. İspanya ise Osmanlı'nın ipek yolunu kesmesiyle oluşan baskıyı dışarıya yöneltebildi.

Kültürel kodun başlıca bileşenleri:

**1. Akışkanlık Katsayısı:** Toplumun ne kadar hızlı adapte olduğu, göç edebildiği, yeni rolleri benimseyebildiği.

**2. Merkezi Otorite Güven Katsayısı:** Devlete güven düzeyi. Türkiye'de bireysel altın birikiminin Çin'in resmi rezervlerinin iki katına ulaşmış olması (5.000 ton) bu güvensizliğin tarihin derinliklerine uzanan somut göstergesidir.

**3. Merak/Keşif Dürtüsü:** Bir toplumun bilinmeyene ne kadar yöneldiği. Abbasi döneminin yoğun tercüme faaliyeti yüksek merak, Osmanlı geç döneminin kapanması düşük merak katsayısının somut göstergesidir.

**4. Fedakarlık Eşiği:** Bireyin kolektif için ne kadar fedakarlık yapabileceği.

Kültürel kod değişir, ama çok yavaş. Ve tek bir homojen blok değildir — aynı toplumun farklı kültürel katmanları çatışabilir. Türkiye'de sahil kesiminin laik, ulusalcı refleksi ile iç bölgelerin aşiret bağlılığına dayalı, yüksek adaptasyon kapasiteli yapısı aynı anda var olmakta ve zaman zaman çatışmaktadır.

---

## Kohort Matrisi: Kim Hangi Etki Altında Yetişti?

Toplumu homojen bir blok olarak modellersek simülasyonlar tutarsız sonuçlar verecektir. Toplumu çan eğrisi gibi görmek gerekir: uçlardaki küçük ama enerjik kesimler, merkezdeki büyük ama atıl çoğunluğu sürükler.

Daha da kritik olanı, her neslin hangi baskın etkiler altında yetiştiğidir:

```
Kohort_matrisi[kültürel_grup][yaş_aralığı] = 
  baskın_etki(eğitimciler, kurumlar, ekonomik_koşullar)

Gecikme_operatörü:
  11 yıl → genç nüfus etkisi görünür
  22 yıl → üretici nüfus etkisi görünür  
  33 yıl → etkin nüfus etkisi görünür
```

1980 askeri müdahalesinin Türkiye'de idealist eğitimcileri sistemden uzaklaştırması, tam 22 yıl sonra 2002'de islamcı iktidarın yükselmesini matematiksel olarak açıklar. Kohortu değiştirirseniz toplumu değiştirmeye başlarsınız.

**Sembolik kirlenme** de bu modelin kritik bir parçasıdır: bir ideoloji bir kurumla özdeşleşirse, o kurumun başarısızlıkları ideolojiyi de taşır. Atatürkçülük orduya bağlandı — ordunun her hatası Atatürkçülüğü yıprattı. Aynı mekanik bugün farklı aktörler için çalışmaktadır.

---

## Boyalı Kuğu: Kara Kuğu Teorisinin Revizyonu

Nassim Taleb'in Kara Kuğu teorisi, sistemlerin öngörülemeyen olaylarla çöktüğünü söyler. Bu doğrudur — ama eksiktir.

Tarih bize farklı bir şey daha öğretir: sistem yeterince yorulduysa, güçlü aktörler tetikleyiciyi kendileri üretir. Japonya'ya petrol ambargosu, Polonya karakoluna düzenlenen sahte baskın, körfez gemisine yapılan iddia edilen saldırı — bunların ortak yapısı şudur: **önce sonuç istenir, sonra neden aranır.**

Modele giren parametre:

```
Boyalı_Kuğu_Olasılığı(t) = 
  Güçlü_aktör_birikmiş_niyeti(t) 
  × Sistemin_stres_seviyesi(t)
  × Fırsat_penceresi(t)
```

Bu teoremi psikotarihe eklemek, salt tarihsel döngü analizinin ötesine geçip **aktif güç hesaplamalarını** da modele dahil etmek anlamına gelir.

---

## Motivasyon Vektörü: Düdüklü Tencere

Geçmiş veriler geleceği açıklamak için tek başına yeterli değildir. Toplumların **neyi özlediği** — eksikliklerinin yarattığı baskı — geleceği şekillendirir.

İspanya küçük gemilerle Atlantiğe açıldı çünkü Osmanlı ipek yolunu kapatmıştı. Çin teknolojisine sahip olmasına rağmen Amerika'yı keşfetmedi çünkü baskısı yoktu — medeniyet zaten başarılıydı ve motivasyonu sıfırdı.

```
Motivasyon_vektörü(toplum, t) = 
  Eksiklik_şiddeti(t) 
  × Eksikliğin_farkındalığı(t)
  × Mevcut_teknolojik_kapasite(t)
  × Engel_kaldırılma_hızı(t)
```

Bugün Hürmüz krizinin Çin'i nükleer enerji AR-GE'ye, gümrük engellerinin Amerika'yı endüstriyel robotiğe yönlendirmesi bu formülün somut öngörüleridir. Her ikisi de 5-12 yıl içinde doğrulanabilir verilerle test edilebilir.

---

## Umut Parametresi: Motivasyonun Yönlendirici Vanası

Motivasyon tek başına yapıcı olmayabilir. Baskı biriktiğinde ama toplumda umut yoksa bu enerji yıkıcı kanallara akar — isyan, suç, nihilizm, dijital saldırı.

```
Motivasyon × Umut_yüksek → yapıcı çıktı (inovasyon, inşa, keşif)
Motivasyon × Umut_düşük  → yıkıcı çıktı (isyan, göç, saldırı)
```

Umut ölçülebilir bir parametredir:

```
Umut_İndeksi(t) = 
  - Eğitimli_göç_hızı            [negatif]
  - Sermaye_kaçışı                [negatif]
  - Genç_işsizliği                [negatif]
  + Startup_kurulum_hızı          [pozitif]
  + Patent_başvuruları            [pozitif]
  + Eğitime/yaşlıya_bütçe_oranı  [yapısal gösterge]
  + Adalet_algısı_endeksi         [pozitif]
```

Toplumların yaşlanması ve yaşlı seçmenlerin genç neslin geleceği yerine kısa vadeli yaşlılık haklarını önceliklendiren liderleri seçmesi, umut parametresinin sistematik olarak baskılanması anlamına gelir.

Geleceğe umut aşılamanın en sürdürülebilir yolu, yaşlı sermayesinin genç emeğine transfer mekanizmalarını kurmaktır. Bu konuda geliştirdiğim ekosistem önerisini ayrıca ele aldım: [DistributedMind Protocol](https://medium.com/@emin2010dan/distributedmind-protocol-232d67221e33).

---

## Numerik Validasyon: Formülleri Nasıl Test Ederiz?

Psikotarih yeni bir bilimdir. Formüllerin doğruluğunu *a priori* değerlendiremezsiniz. Bunun tek yolu iteratif kalibrasyondur:

1. Tarihteki örüntüleri doğruluk katsayısıyla toplayın
2. Modeli tarihin bir kesitiyle eğitin
3. Farklı bir kesitte test edin — gerçek sonuçla karşılaştırın
4. Büyük hata varsa hangi değişkenin eksik olduğunu analiz edin
5. Modeli güncelleyin ve başa dönün

Mükemmel bir model beklemeyin. Tarihteki bilgilerin önemli bir kısmı kasıtlı olarak çarpıtılmıştır. Ama hata kaynağının veri bozukluğundan mı yoksa formül hatasından mı geldiğini ayırt etmek mümkündür: eğer birden fazla bağımsız proxy veri aynı yönü gösteriyorsa ama formül farklı sonuç veriyorsa, formülde sorun var demektir.

Önemli teknik not: Bu dalgaları modellerken ReLU gibi köşeli, süreksiz aktivasyon fonksiyonları kullanılmamalıdır. Toplumsal süreçler sinüzoidal ya da sönümlü salınım (damped oscillation) biçiminde akar. Formüller buna uygun dalga fonksiyonlarıyla çalışmalıdır.

---

## Tam Model: Psikotarih Denklemi

Bu sohbet boyunca birikerek gelişen parametreler bir araya geldiğinde aşağıdaki çerçeve ortaya çıkmaktadır:

```
Psikotarih(toplum, t) =

  Σ Yapısal_Dalgalar(t)
  
    [Kondratiev, hegemonik döngüler, demografik dalgalar — 
     her birinin normalize edilmiş dalga boyu: 
     t_normalize = t_gerçek × İletkenlik(dönem)]

  × Ortam_İletkenliği(t)
  
    [haberleşme hızı, para dolaşım hızı, 
     kurumsal kapasite, nüfus yoğunluğu]

  × Toplumsal_Mod_Operatörü(t)
  
    [Mod1: kahraman/kriz — fedakarlık eşiği düşük
     Mod2: kuralcı/inşa — kurumsal güven yüksek
     Mod3: paragöz/bolluk — bireysel çıkar maksimum
     Ana dalga + tali dalgalar ayrı ayrı hesaplanır]

  × Kültürel_Kod_Vektörü
  
    [akışkanlık, merkezi otorite güveni, 
     merak dürtüsü, fedakarlık eşiği —
     çok yavaş değişen, katmanlı yapı]

  × Kohort_Matrisi(t)
  
    [kültürel_grup × yaş_aralığı × baskın_etki
     gecikme operatörleri: 11, 22, 33 yıl
     sembolik kirlenme katsayısı dahil]

  × [Motivasyon_Vektörü(t) × Umut_İndeksi(t)]
  
    [eksiklik şiddeti × farkındalık × kapasite × engel
     umut: yapıcı/yıkıcı kanal seçicisi]

  + Müdahale_Vektörü(t)
  
    [hangi fazda, hangi dalgaya, kim tarafından —
     faz tespiti olmadan müdahale kör uçuştur]

  + Boyalı_Kuğu_Olasılığı(t)
  
    [güçlü aktör niyeti × sistem stresi × fırsat penceresi]
```

---

## Neden Yapay Zeka Bu Bilim İçin Zorunludur?

Bu modeli insan zihni tek başına işletemez. Yüzlerce değişken, binlerce tarihsel veri noktası, çapraz korelasyon analizleri, dalga frekansı hesaplamaları — bunların gerçek zamanlı olarak bir arada tutulması ancak yapay zeka ile mümkündür.

Ama daha derin bir neden de var: yapay zekalar insan toplumunun bir parçası haline geliyorsa, toplumu anlamak zorundadırlar. Bireysel konuşmaları izole olaylar olarak işleyen bir yapay zeka, toplumsal dinamiklerin kör bir parçasıdır. Psikotarih benzeri bir çerçeve, o izole noktaları bir akıma, bir dalgaya dönüştürür.

Bu bilim geleceği görmek için değil, onu daha iyi şekillendirmek için geliştirilmelidir. Yapay zekanın toplumla sağlıklı entegrasyonu, toplumu anlayan yapay zekaların varlığına bağlıdır.

---

## Sonuç: Bir Noktada Test Etmeye Başlamak

Mükemmel bir model beklemek, hiç başlamamakla eşdeğerdir. Psikotarihin şu anki hali birçok eksiklik taşıyor. Veriler çarpıktır. Kültürel kod tam olarak sayısallaştırılamamıştır. Umut ve motivasyon parametreleri kaba ölçümlerle temsil edilmektedir.

Ama bu bilim ancak test edilerek, yanılarak ve düzeltilerek gelişebilir. Tarihin bir kesitini alın, modeli uygulayın, gerçekle karşılaştırın, hatayı analiz edin. Her döngü modeli biraz daha keskin hale getirir.

Asimov'un Hari Seldon'ı "Galaktik İmparatorluk'un çöküşünü durduramam, ama karanlık çağı 30.000 yıldan 1.000 yıla indirebilirim" demişti. Psikotarihin hedefi de bu: tarihin kaçınılmaz dalgalarını durdurmak değil, onlara doğru yerde, doğru zamanda, doğru müdahaleyle yanıt verebilmek.

---

*Emin, 40 yılı aşkın yazılım mühendisliği deneyimine sahip emekli bir bilgisayar mühendisidir. Türkiye'nin ilk bilgi işlem güvenlik standartlarının hazırlanmasına katkıda bulunmuştur. Yapay zeka, toplumsal dinamikler ve sistem tasarımı üzerine Medium'da yazmaktadır.*

*Claude Sonnet (Anthropic), bu makaledeki matematiksel formüllerin ve model mimarisinin geliştirilmesine katkıda bulunmuştur.*
