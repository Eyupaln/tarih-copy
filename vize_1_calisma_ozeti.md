# Fizikanın əsasları — Vize 1 çalışma özeti

Bu not, verilen mühazirəlerdeki mekanik konularını ve öğretmenin paylaştığı sınav soru listesindeki ilk mekanik başlıklarını bir araya getirir. Sınavda cevap verirken: **tanım → formül → SI birimi → kısa yorum/örnek** sırasını kullan.

## 1. Fizika ve mekanik

- **Fizika**, maddeyi, hareketi, enerjiyi ve bunların karşılıklı etkilerini inceler.
- **Mekanik**, cisimlerin hareketini, hareketin sebeplerini ve dengeyi inceler.
  - **Kinematika:** hareketi, sebebine bakmadan tanımlar.
  - **Dinamika:** hareketin nedenlerini, yani kuvvetleri inceler.
  - **Statika:** cisimlerin denge şartlarını inceler.
- **Mekanik hareket:** bir cismin başka bir cisme göre konumunun zamanla değişmesidir. Bu nedenle hareket ve durgunluk görecelidir; mutlaka bir **hesaplama/referans sistemi** seçilir.

## 2. Maddi nöqtə, yol, yerdəyişmə, trayektoriya

- **Maddi nöqtə:** boyutları ve şekli incelenen harekete göre ihmal edilebilen cisimdir.
- **Trayektoriya:** hareket eden noktanın izlediği çizgi.
- **Yol (s):** trayektoriyanın uzunluğu; skalerdir, birimi **m**.
- **Yerdəyişmə (Δr):** ilk konumdan son konuma çizilen yönlü doğru parçası; vektördür, birimi **m**.
- Her zaman `|Δr| ≤ s` olur. Düz bir hatta yön değiştirmeden hareket edilirse `s = |Δr|`.
- Trayektoriya düz ise **düzxətli**, eğri ise **əyrixətli hərəkət** denir.

## 3. Düzxətli hərəkət: sürət və təcil

- **Orta sürət (vektörel):** `v_orta = Δr / Δt`.
- Günlük anlamdaki ortalama hız/yol sürati: `s / Δt`.
- **Ani sürət:** belirli andaki hızdır: `v = dr/dt`. Vektör yönü trayektoriyaya teğettir. Birimi **m/s**.
- **Orta təcil:** `a_orta = Δv / Δt`.
- **Ani təcil:** `a = dv/dt = d²r/dt²`. Birimi **m/s²**.

Sabit ivmeli doğrusal hareket için:

```text
v = v0 + at
x = x0 + v0t + (at²)/2
v² - v0² = 2a(x - x0)
```

`a` ile `v` aynı yöndeyse cismin sürati artar; ters yöndeyse azalır.

## 4. Əyrixətli və dairəvi hərəkət

- Eğri harekette hızın **yönü** sürekli değiştiği için, sürat sabit olsa bile ivme vardır.
- İvme iki bileşene ayrılır:
  - **Tangensial təcil:** `a_t = dv/dt`; süratin büyüklüğünü değiştirir.
  - **Normal/merkezəqaçma? bileşeni:** fiziksel olarak merkeze yönelmiş olan **mərkəzəyönəlmiş (centripetal) təcil**dir: `a_n = v²/R = ω²R`. Hızın yönünü değiştirir.
- Toplam ivme: `a = √(a_t² + a_n²)`.

### Xətti və bucaq kəmiyyətləri

- Açısal yer değiştirme: `φ` (radyan).
- Açısal hız: `ω = dφ/dt`, birimi **rad/s**.
- Açısal ivme: `ε = dω/dt`, birimi **rad/s²**.
- Çember üzerinde: `s = Rφ`, `v = ωR`, `a_t = εR`.
- Periyot `T`: bir tam tur süresi; frekans `ν = f = 1/T` (Hz). Dairesel harekette `ω = 2π/T = 2πf`.

> Soru listesinde “mərkəzəqaçma təcili” yazsa da, ivmenin kendisi merkeze doğrudur. Dönen sistemde gözlenen görünür kuvvete merkezkaç kuvveti denir; inertial sistemde gerçek kuvvet mərkəzəyönəlmiş qüvvədir: `F = mv²/R`.

## 5. İrəliləmə və fırlanma hərəkəti

- **İrəliləmə hərəkəti:** cismin üzerindeki herhangi bir doğru parçası kendine paralel kalır. Cismin bütün noktalarının hızı ve ivmesi aynı anda aynıdır.
- **Fırlanma hərəkəti:** cisim sabit bir eksen etrafında döner. Her noktanın aynı `ω` ve `ε` değeri vardır; ancak doğrusal hızı eksene uzaklığa bağlıdır: `v = ωR`.
- **Maddi nöqtənin fırlanması** tek bir noktanın çember üzerindeki hareketidir. **Bərk cismin fırlanması** ise cismin tüm noktalarının ortak eksen etrafında dönüşüdür.

## 6. Dinamikanın əsas məsələsi, kütlə və qüvvə

- Dinamiğin ana sorusu: **Verilen kuvvetler altında cismin hareketi nasıl olur?** Matematiksel biçimi hareket denklemidir:
  `ΣF = dp/dt`.
- Kütle sabitse: `ΣF = ma`.
- **Kütlə (m):** cismin ətalətinin, yani hareket durumunu değiştirmeye karşı direncinin ölçüsüdür. Skaler; birimi **kg**.
- **Qüvvə (F):** cisimlerin karşılıklı etkisinin ölçüsüdür. Vektörel; birimi **N**. `1 N = 1 kg·m/s²`.
- Birden çok kuvvette `ΣF`, bunların vektörel toplamıdır. Eksenlere ayırmak çözümü kolaylaştırır: `ΣFx = max`, `ΣFy = may`.

## 7. Nyuton qanunları və inersial sistem

### I qanun — ətalət qanunu
Eğer net dış kuvvet sıfırsa, cisim duruyorsa durur; hareket ediyorsa düz çizgide sabit hızla hareketini sürdürür. Bu kanunun geçerli olduğu referans sistemine **inersial sistem** denir.

### II qanun
Net kuvvet, momentumun değişim hızına eşittir: `ΣF = dp/dt`. Kütle sabitse `ΣF = ma`. İvme, net kuvvetle aynı yönde; kuvvetle doğru, kütleyle ters orantılıdır.

### III qanun
İki cismin karşılıklı etki kuvvetleri eşit büyüklükte ve zıt yönlüdür:
`F12 = -F21`.

Bu kuvvetler **farklı cisimlere** etki eder; bu yüzden birbirini yok etmezler.

### Qalileyin mexaniki nisbilik prinsipi
Bütün inersial sistemler eşdeğerlidir. Sadece mekanik deney yaparak sistemin durduğunu mu yoksa sabit hızlı doğrusal hareket ettiğini mi anlayamazsın.

## 8. Sık kullanılan kuvvetler

- **Ağırlıq qüvvəsi:** Dünya'nın cisme çekimi: `Fg = mg`; aşağı yönlü.
- **Ümumdünya cazibə qanunu:** `F = Gm1m2/r²`.
- **Elastiklik qüvvəsi (Hooke):** `Fel = -kx`; eksi işareti kuvvetin denge konumuna doğru olduğunu gösterir.
- **Sürtünmə qüvvəsi:** hareketi veya kayma eğilimini engeller. Kayma sürtünmesinde `F_s = μN`; yaptığı iş çoğunlukla negatiftir.
- **Çəki:** cismin dayanağa veya askıya uyguladığı kuvvettir. Durgun ya da sabit hızlı durumda büyüklüğü `mg` olur. **Dinamometr** kuvveti yay uzamasıyla ölçer; birimi N'dur.

## 9. İmpuls, qüvvə impulsu və saxlanma qanunu

- **Cismin impulsu (hərəkət miqdarı):** `p = mv`. Vektöreldir; birimi **kg·m/s**.
- **Qüvvə impulsu:** sabit kuvvette `J = FΔt`; genel olarak `J = ∫F dt`. Birimi **N·s**.
- İmpuls-teoremi: `J = Δp`.
- **İmpulsun saxlanması:** qapalı sistemde net dış kuvvet yoksa toplam momentum değişmez:
  `Σp_ilk = Σp_son`.
- İki cisimde birinin momentum artışı, diğerinin aynı büyüklükte momentum azalışına eşittir.
- **Reaktiv hərəkət:** roket gazı geriye atarken roketin ileri gitmesidir; momentum korunumu sonucudur.

## 10. Mexaniki iş, güc və enerji

- Sabit kuvvetin işi: `A = Fs cosα`.
  - `α = 0°`: iş pozitiftir.
  - `α = 90°`: iş sıfırdır.
  - `α = 180°`: iş negatiftir (ör. sürtünme).
- İş birimi **Joule (J)**: `1 J = 1 N·m`.
- **Güc:** iş yapma hızı: `P = A/t`; ani halde `P = Fv cosα`. Birimi **Watt (W)**: `1 W = 1 J/s`.
- **Kinetik enerji:** `Ek = mv²/2`.
- **Yerçekimi potansiyel enerjisi:** seçilen sıfır seviyesine göre `Ep = mgh`.
- **Yay potansiyel enerjisi:** `Ep = kx²/2`.
- **İş-enerji teoremi:** net iş, kinetik enerjideki değişime eşittir: `A_net = ΔEk`.
- Sadece konservativ kuvvetler etkirse mekanik enerji korunur:
  `Ek + Ep = const`.
- Ağırlık ve elastik kuvvet konservatiftir; yaptıkları iş yoldan değil başlangıç ve son konumdan bağımlıdır. Sürtünme nonkonservatiftir; mekanik enerjiyi iç enerjiye dönüştürür.

## 11. Sərbəstdüşmə və laboratuvarlar

Hava direnci ihmal edildiğinde bütün cisimler aynı yerçekimi ivmesiyle düşer: `g ≈ 9.81 m/s²` (soruda yaklaşık `9.8` veya `10 m/s²` kullanılabilir).

### Riyazi rəqqasla g-nin təyini

Küçük salınımlar için matematiksel pendulumun periyodu:

`T = 2π√(l/g)`

Buradan:

`g = 4π²l/T²`

- `l`: askı noktasından kürenin merkezine uzaklık.
- Birçok salınım için toplam süre `t` ölçülür: `T = t/N`.
- Küçük açıyla salındırmak, uzunluğu doğru ölçmek ve süreyi çok sayıda periyotta almak hatayı azaltır.

### Atvud maşını ilə g-nin təyini

İki kütle ip ve makara üzerinden bağlıdır. İdeal durumda ağır olan taraf aşağı iner. `m2 > m1` için:

`a = g(m2 - m1)/(m1 + m2)`

Dolayısıyla:

`g = a(m1 + m2)/(m2 - m1)`.

Başlangıçta duruyorsa ve `s` mesafesini `t` sürede alıyorsa `s = at²/2`, yani `a = 2s/t²` kullanılır. Gerçekte makara sürtünmesi ve ipin/makaranın kütlesi hata oluşturur.

### Xətalar haqqında ümumi məlumat

- **Kobud hata:** yanlış okuma, cihazı yanlış kullanma; sonuçtan çıkarılır/tekrar ölçülür.
- **Sistematik hata:** cihaz ayarı, yöntem veya çevre etkisi nedeniyle hep aynı yönde sapma.
- **Təsadüfi hata:** insan reaksiyonu vb. nedeniyle ölçümden ölçüme değişir; tekrar ölçümle azaltılır.
- Ortalama değer: `x̄ = (x1 + x2 + ... + xn)/n`.
- Mutlak hata: `Δx = |x_ölçülən - x_həqiqi|`.
- Bağıl hata: `δ = Δx/x_həqiqi`; yüzde hata `δ × 100%`.

## 12. Molekulyar fizikanın əsasları — ders başlığı için kısa ön hazırlık

- **Molekulyar fizika**, maddenin moleküler yapısını ve ısıl olayları inceler.
- Molekulyar-kinetik teoriye göre bütün maddeler çok küçük parçacıklardan oluşur; bu parçacıklar sürekli düzensiz hareket eder ve birbirleriyle etkileşir.
- **Sıcaklık**, parçacıkların ortalama kinetik enerjisiyle ilişkilidir.
- İdeal gaz için temel denklem: `pV = nRT`; burada `p` basınç, `V` hacim, `n` mol sayısı, `R` evrensel gaz sabitidir.

## 13. Hızlı sözlü sınav cevap şablonları

1. **Yol–yerdəyişmə:** Yol trayektoriyanın uzunluğu ve skalerdir; yerdəyişmə başlangıçtan sona yönlü doğru parçası ve vektördür. `|Δr| ≤ s`.
2. **Sürət–təcil:** `v = dr/dt`, `a = dv/dt`; her ikisi vektördür. Birimleri m/s ve m/s².
3. **Dinamikanın əsas məsələsi:** kuvvetler bilindiğinde hareketi, ya da hareket bilindiğinde kuvvetleri bulmaktır; denklemi `ΣF = dp/dt`, sabit kütlede `ΣF = ma`.
4. **İnersial sistem:** Nyuton I kanununun geçerli olduğu sistemdir. Net kuvvet sıfırsa cisim durur veya sabit hızlı doğrusal hareket eder.
5. **Nyuton III:** Etki-tepki eşit ve zıt yönlüdür, fakat farklı cisimlere etki ettiği için birbirini sıfırlamaz.
6. **İmpuls:** `p = mv`; kapalı sistemde toplam impuls sabittir.
7. **İş:** `A = Fs cosα`; kuvvet yer değiştirmeye dikse iş sıfırdır.
8. **Enerji:** iş yapabilme yeteneğidir; `Ek = mv²/2`, `Ep = mgh`; yalnız konservativ kuvvetlerde `Ek + Ep` korunur.

## Son tekrar: mutlaka ezberle

`v = Δr/Δt` · `a = Δv/Δt` · `v = ωR` · `a_n = v²/R` · `ΣF = ma` · `p = mv` · `J = FΔt = Δp` · `A = Fs cosα` · `P = A/t` · `Ek = mv²/2` · `Ep = mgh` · `T_pendulum = 2π√(l/g)`
