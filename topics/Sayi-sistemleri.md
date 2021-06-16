# Sayı Sistemleri 

# Decimal System(Onluk Sistem)

Günlük hayatta kullandığımız, 10 tabanlı sayı sistemidir. 0,1,2,3,4,5,6,7,8,9 rakamlarından oluşur. Decimal kullanılarak herhangi bir içerik ondalık sisteme göre kodlanabilir ve bu kodlama insanlar tarafından okunup, anlaşılabilir. 

Matematikte ondalık sayı sistemi insanlığın ilk çağlarına kadar dayanır. Bu kadar eskilere uluşmasının sebebi kağıt kalem yokken insanların parmaklarını kullanarak hesaplamalar yapmasıdır.

## Onluk Sistemde Basamak Kavramı

Onluk sayı sisteminde her rakam bulunduğu basamağa göre değer alır. Adından da anlaşılacağı üzere tabanı 10'dur. Sağdan 0 ile başlayarak her sayı 10 üzeri sayının bulunduğu basamak değeriyle çarpılır. Örnek verecek olursak.

***Örnek 1***

İkili sistemde **563** değerini inceleyelim. Sağdan başlarsak;

```
-> 5 * (10²) + 6 * (10¹) + 3 * (10⁰)

-> (5 * 100) + (6 * 10) + (3 * 1) 

-> 500 + 60 + 3 = 563
```
```
Sonuç olarak onluk sistemdeki 563 değerinin basamak değeri 563 değerine eşittir.
```

# Dönüşümler

## Onluk Sistemden(Decimal) > İkili Sisteme(Binary) 

Elimizde bulunan onluk sistemdeki değeri bölebildiğimiz kadar 2'ye bölelim. Daha sonra en düşük değerli bit(en sağdaki bit)'den başlayarak en yüksek değerlikli bit'e(en soldaki bit) doğru ilk bulduğumuz kalandan son bölüme kadar yazılır. Örnekle daha iyi pekişecektir...

Onluk sistemde **216** değerinin ikili sistemde karşılığını bulalım...

```
-> 216/2 = 108     = kalan 0
-> 108/2 = 54      = kalan 0
-> 54/2  = 27      = kalan 0
-> 27/2  = 13      = kalan 1
-> 13/2  = 6       = kalan 1
-> 6/2   = 3       = kalan 0
-> 3/2   = 1       = kalan 1
-> 1

İlk bulduğumuz kalandan son bölüme kadar yazacak olursak(en düşük değerlikli bit'ten en yüksek değerli bit'e doğru yazacağız) ikili sistemde 11011000 değerine ulaşırız. 
```
```
Sonuç olarak onluk sistemdeki 216 değerinin ikili sistemdeki değeri (11011000) değerine eşittir.
```

## Onluk Sistemden(Decimal) > Sekizli Sisteme(Octal) 

Bu dönüşümde elimizdeki onluk tabanlı sayı sekize bölünür. Çıkan sonuçta sağdan başlanarak ilk olarak bölüm daha sonra kalan yazılır. Örnekle pekiştirelim.

Onluk sistemde **61** değerinin sekizlik sistemde karşılığını bulalım...

```
-> 61/8 = 7     = kalan 5 

sağdan başlanarak ilk olarak bölüm daha sonra kalanı yazacak olursak sekizlik sistemde 75 değerini elde etmiş oluruz.
```
```
Sonuç olarak onluk sistemdeki 61 değerinin sekizlik sistemdeki değeri (75) değerine eşittir.
```

## Onluk Sistemden(Decimal) > Onaltılık Sisteme(Hexadecimal)

Sekizlik sisteme dönüştürürken yaptığımız işlemin aynısını yapacağız. Onluk tabanlı sayıyı onaltıya böleceğiz. Çıkan sonuçta sağdan başlanarak ilk olarak bölüm daha sonra kalan yazılır. Örnekle pekiştirelim.

Onluk sistemde **102** değerinin onaltılık sistemde karşılığını bulalım...

```
-> 102/16 = 6     = kalan 6 

sağdan başlanarak ilk olarak bölüm daha sonra kalanı yazacak olursak onaltılık sistemde 66 değerini elde etmiş oluruz.
```
```
Sonuç olarak onluk sistemdeki 102 değerinin onaltılık sistemdeki değeri (66) değerine eşittir.
```

# Binary System (İkili Sistem)

Bu sayı sisteminin tabanı ikidir. 0 ve 1 rakamlardan oluşur. Bu sistemde bulunan her bir rakam BIT(Binary Digit) ile tanımlanır. Buradaki 0 ve 1 , elektriğin olup olmama durumuna eşittir. Bilgisayarlarımız temelde ikili kod kullanır.

8 haneden oluşan ikili kod, 256 farklı değer alabilir. Bu değerler sembollere, harflere ya da yapılara denk gelir. İkilik sistemdeki sekiz haneli değerler; 

**8 x 1 bit = 8 bit yani 1 byte** eşit olur.

**not:**
```
4 bit   = nibble
8 bit   = byte
16 bit  = word 
32 bit  = double word
```

## İkili Sistemde Basamak Kavramı

İkili sistem gündelik hayatta kullandığımız ondalık sistem ile benzer şekilde çalışır. Ondalık sistemde sağdan 0 ile başlayarak her sayı 10 üzeri sayının bulunduğu basamak değeriyle çarpılıyordu. İkili sistemin de çalışma mantığı benzerdir. Sağdan 0 ile başlayarak her basamakta 2’nin bir kuvveti alınır. Daha sonra aktif olan(yani 1) bitlerin değerleri toplanır. Bir örnek yaparak pekiştirelim...

***Örnek 1***

İkili sistemde **00001001** değerini inceleyelim. Sağdan başlarsak;

```
2 üzeri 0 = 1		(1)
2 üzeri 1 = 2 		(0)
2 üzeri 2 = 4		(0)
2 üzeri 3 = 8		(1)
2 üzeri 4 = 16		(0)
2 üzeri 5 = 32		(0)
2 üzeri 6 = 64		(0)
2 üzeri 7 = 128	        (0)
```

Aktif olan bitler görüldüğü üzere sıfırıncı ve üçüncü bitler bunların toplamları ise **1 + 8 = 9** olarak bulunur.

***Örnek 2***

İkili sistemde farklı bir örnek olarak virgüllü bir değer olan **1111,011** değerini inceleyelim. Burada dikkat edilmesi gereken nokta;

Virgülün sol tarafında kalan kısım, yukarıdaki örnekte olduğu gibi sağdan sola doğru 2 üzeri 0 dan başlanarak her basamakta 2’nin bir kuvveti alınır. Virgülün sağ tarafında ise soldan sağa doğru 2 üzeri -1 den başlanarak her basamakta 2’nin bir kuvveti alınır.(-1, -2, -3 olarak devam eder yani kuvvet küçülür.)  

```
2 üzeri -3 = 1/8	(1)
2 üzeri -2 = 1/4 	(1)
2 üzeri -1 = 1/2	(0)
,
2⁰ = 1		(1)
2¹ = 2		(1)
2² = 4		(1)
2³ = 8	        (1)
```

Aktif olan bitleri toplayacak olursak...

```
0,125 + 0,25 + 1 + 2 + 4 + 8 = 16,375
```

**Not2:** 1/8 ve 1/4 değerlerinin ondalık karşıtları olan 0,125 ve 0,25 değerlerini yazdık. Kafa karışıklığı doğurmasın. 

# Dönüşümler

## İkili Sistemden(Binary) > Onluk Sisteme(Decimal) 

Bunun örneği yukarıdaki örneklerde yaptık. Yine de bir örnek daha yapalım.

İkili sistemde **01011000** değerinin onluk sistemde karşılığını bulalım...

```
2⁰ = 1		(0)
2¹ = 2 		(0)
2² = 4		(0)
2³ = 8		(1)
2⁴ = 16		(1)
2⁵ = 32		(0)
2⁶ = 64		(1)
2⁷ = 128	        (0)
```

Aktif bitleri toplayarak onluk sistemde karşılığını bulalım.

```
8 + 16 + 64 = 88
ikili sistemde 01011000 = onluk sistemde 88 değerine eşittir.
```

## İkili Sistemden(Binary) > Sekizlik Sisteme(Octal)

Burada yapacağımız işlem binary değeri üçerli gruplara ayırmak olacaktır. Aklınızda  8 bit'i eşit bir şekilde nasıl üçe böleceğiz sorusu oluduğunun farkındayım. Yüksek değerlikli bit'in (en soldaki bit) yanına bir tane daha 0 eklememiz gerekiyor. Bu işlemi yaptıktan sonra her grup için ayrı ayrı sağdan 0 ile başlayarak her basamakta 2’nin bir kuvveti alınır. Her grup için değerler ayrı ayrı toplanır zaten maksimum 7 olabilir. Soldan başlanarak yazılmaya başlanır. 

Yine aynı değeri kullanalım. İkili sistemde **01011000** değerinin sekizlik sistemde karşılığını bulalım.

İlk olarak üçlü gruplara ayıralım..

```
(001) (011) (000)
```
son gruba otomatik olarak bir 0 ekledik. Şimdi grupların toplam değerlerini bulalım.

```
(001) = 1 (011) = 3 (000) = 0
```
Soldan başlayarak değeri yazacak olursak karşımıza şöyle bir sonuç çıkar:
```
ikili sistemde 01011000 = sekizlik sistemde 88 değerine eşittir.
```

## İkili Sistemden(Binary) > Onaltılık Sisteme(Hexadecimal)

Burada da binary değerimizi iki eşit parçaya ayırmalıyız. Bu işlemden sonra her iki grup için de ayrı ayrı sağdan 0 ile başlayarak her basamakta 2’nin bir kuvveti alınır. Her iki grup için değerler ayrı ayrı toplanır zaten maksimum 15 olabilir. Sekizlik sistemde olduğu gibi soldan başlanarak yazılmaya başlanır. 

İkili sistemde **01011000** değerinin onaltılık sistemde karşılığını bulalım.

İlk olarak iki gruba ayıralım..

```
(0101) (1000)
```
Şimdi grupların toplam değerlerini bulalım.
```
(0101) = 5 (1000) = 8
```
Soldan başlayarak değeri yazacak olursak karşımıza şöyle bir sonuç çıkar:
```
ikili sistemde 01011000 = onaltılık sistemde 58 değerine eşittir.
```

# Octal System(Sekizlik Sistem)

Bu sayı sisteminin tabanı sekizdir. 0,1,2,3,4,5,6,7 rakamlarından oluşur. 

## Sekizlik Sistemde Basamak Kavramı

Ondalık sistem ile benzer şekilde çalışır. Sağdan 0 ile başlayarak her sayı 8 üzeri sayının bulunduğu basamak değeriyle çarpılır. Ardından basamak değerleri toplanır. Bir örnek yapıp dönüşümlere geçelim.

***Örnek 1***

Sekizlik sistemde **123** değerini inceleyelim. Sağdan başlarsak;
```
-> 1 * (8²) + 2 * (8¹) + 3 * (8⁰)

-> (1 * 64) + (2 * 8) + (3 * 1) 

-> 64 + 16 + 3 = 83
```
```
Sonuç olarak sekizlik sistemdeki 123 değerinin karşılığı onluk sistemde 83 değerine eşittir.
```

# Dönüşümler

## Sekizlik Sistemden(Octal) > İkili Sisteme(Binary)

Hatırlayacağınız üzere ikili sistemden sekizlik sisteme dönüşüm yaparken bit'leri üçerli gruplara ayırıyorduk. Burada da tam/keskin bir dönüşüm işlemi olmasa da benzer bir işlem uygulayacağız. Öncelikle dönüştürmek istediğimiz sekizlik sistemdeki değerin en sağından başlayarak o rakamın ikili sistemde karşılığını bulmamız gerekiyor. Aynı işlem sol tarafa doğru devam eder ve en son ikili değerler birleştirilir. Bilindiği üzere sekizlik sistemde maksimum değer 7'dir. İkili sistemde düşük değerli ilk üç bit'in toplamının alabileceği maksimum değer de 7'dir. Sayılara üçerli gruplara ayırmamızdaki temel etken de bu aslında. 
Eğer sekizlik sistemdeki değerimiz iki rakamdan oluşuyor ise sol tarafa ek olarak iki sıfır eklenir.
Örnek yapıp daha da pekiştirelim.

Sekizlik sistemde **65** değerinin ikili sistemde karşılığını bulalım...

```
5 rakamının ikili sistemde karşılığı = (101)
    -> 2⁰ = 1		(1)
    -> 2¹ = 2 		(0)
    -> 2² = 4		(1)
6 rakamının ikili sistemde karşılığı = (110)
    -> 2⁰ = 1		(0)
    -> 2¹ = 2 		(1)
    -> 2² = 4		(1)
```

```
Sağ taraftan sola doğru değerlerimizi birleştirirsek ayrıca başına da iki sıfır ekleyelim. Sonuç olarak sekizlik sistemdeki 65 değerinin karşılığı ikili sistemde (00110101) değerine eşittir. 
```

Bir başka örnek yapacak olursak..

Sekizlik sistemde **232** değerinin ikili sistemde karşılığını bulalım...

```
2 rakamının ikili sistemde karşılığı = (010)
    -> 2⁰ = 1		(0)
    -> 2¹ = 2 		(1)
    -> 2² = 4		(0)
3 rakamının ikili sistemde karşılığı = (011)
    -> 2⁰ = 1		(1)
    -> 2¹ = 2 		(1)
    -> 2² = 4		(0)
2 rakamının ikili sistemde karşılığı = (010)
    -> 2⁰ = 1		(0)
    -> 2¹ = 2 		(1)
    -> 2² = 4		(0)
```

```
Sağ taraftan sola doğru değerlerimizi birleştirelim. Sonuç olarak sekizlik sistemdeki 232 değerinin karşılığı ikili sistemde (10011010) değerine eşittir. 
```

## Sekizlik Sistemden(Octal) > Onluk Sisteme(Decimal) 

Bunun örneği yukarıdaki örnekte yaptık. Yine de bir örnek daha yapalım.

Sekizlik sistemde **232** değerinin onluk sistemde karşılığını bulalım...
```
-> 2 * (8²) + 3 * (8¹) + 2 * (8⁰)

-> (2 * 64) + (3 * 8) + (2 * 1) 

-> 128 + 24 + 2 = 154
```
```
Sonuç olarak sekizlik sistemdeki 232 değerinin karşılığı onluk sistemde (154) değerine eşittir.
```

## Sekizlik Sistemden(Octal) > Onaltılık Sisteme(Hexadecimal)

Sekizlik sistemdek bir değeri onaltılık sisteme dönüştürürken ilk olarak yapmamız gereken sekizlik sistemdeki değeri onluk sisteme çevirmektir. Daha sonra onluk sistemdeki değeri 16'ya bölmemiz gerekir. Bu işlem sonucu ilk bölüm daha sonra kalan yazılır. Örneklerle pekiştirelim.

Sekizlik sistemde **232** değerinin onaltılık sistemde karşılığını bulalım...
```
Sekizlik sistemdeki 232 değerinin onluk sistemde karşılığının 154 olduğunu bulmuştuk. Sırada 154 sayılısını 16'ya bölmeye geldi

154/16 = bölüm (9) kalan ise (10=A)
       = 9A
```

```
Sonuç olarak sekizlik sistemdeki 232 değerinin karşılığı onaltılık sistemde (9A) değerine eşittir.
```

# Hexadecimal System(Onaltılık Sistem)

16 benzersiz sembolden oluşan(0-1-2-3-4-5-6-7-8-9 rakamları ve A,B,C,D,E,F) ve bir veriyi temsil etmek için kullanılan 16 tabanlı sayı sistemidir. Hexadecimal'de 9'un üstündeki sayılar için harf kullanılır.

```
A=10
B=11
C=12
D=13
E=14
F=15
```

Hexadecimal çok kullanışlı bir sistem olduğu için hata kodları, durum kodları, durdurulma hataları ve mavi ekran hatalarında karşımıza sürekli Hexadecimal biriminden hata kodları çıkar. Bunun nedeni programcıların hata kodlarını HEX olarak kodlamasıdır.

## Hexadecimal'in Tarihçesi?

1960‘ larda Latin alfabesinin ve noktalama, kontrol, matematik vs. işaretlerin genel amaçlı bilgisayarların alfabesine girmesiyle; bilgi ölçme ve temsil birimi olarak byte (8 basamaklı ikili kod) kabul edilmiştir. Bundan sonra 8 / 3 = 2,66 tamsayı olmadığı için 8′ li sayıların bellekte yerleştirilmesi ve incelenmesi zorlaşmış, buna karşılık olarak iki rakamı tam bir Byte’ da yerleşen 16’ lı sistem alternatifsiz bir aralık sistem olarak kullanılmaya başlamıştır.

## Onaltılık Sistemde Basamak Kavramı

Ondalık sistem ile benzer şekilde çalışır. Sağdan 0 ile başlayarak her sayı 16 üzeri sayının bulunduğu basamak değeriyle çarpılır. Ardından basamak değerleri toplanır. Örnek yapıp dönüşümlere geçelim...

***Örnek 1***

Onaltılık sistemde **1F** değerini inceleyelim. Sağdan başlarsak;
```
-> 1 * (16¹) + F * (16⁰)

-> (1 * 16) + (15 * 1) 

-> 16 + 15 = 31
``` 
```
Sonuç olarak onaltılık sistemdeki 1F değerinin karşılığı onluk sistemde (154) değerine eşittir.
```
# Dönüşümler

## Onaltılık Sistemden(Hexadecimal) > İkili Sisteme(Binary)

Öncelikle elimizdeki onaltılık sistemdeki değeri parçalara ayıralım, burada ayrılan her bir basamak 4 bit'e karşılık gelmektedir. Yani sonuç olarak basamaktaki değerin ikili sistemdeki karşılığını bulmamız gerekmektedir.
Örneklerle daha iyi bir şekilde anlaşılacaktır.

Onaltılık sistemde **BE** değerinin ikili sistemde karşılığını bulalım...

```
-> B = 11 - E = 14

-> B = (1011) - E = (1110)
    
-> BE = (10111110)
```
```
Sonuç olarak onaltılık sistemdeki BE değerinin karşılığı ikili sistemde (10111110) değerine eşittir.
```

## Onaltılık Sistemden(Hexadecimal) > Sekizlik Sisteme(Octal)

Onaltılık sistemden sekizlik sisteme dönüşüm yapmanın çeşitli yolları var. İlk olarak değerin binary karşılığını bulduktan sonra, binary değeri üçerli bölümlere ayıracağız. 8 tam olarak üç eşit parçaya ayrılmadığı için sol tarafa bir sıfır ekleriz. Daha sonra sağ taraftan başlayarak sola doğru basamak değerleri bulunur ve yazılır. Örnek ile daha da pekişecektir.

Onaltılık sistemde **BE** değerinin sekizlik sistemde karşılığını bulalım...

```
-> BE değerinin ikili sistemde karşılığını yukarıda bulmuştuk.
-> BE = (10111110)
-> Üçerli gruplara ayıralım ve basamak değerlerini bulalım.

-> (010) = 2 (111) = 7 (110) = 6
-> 276

```
```
Sonuç olarak onaltılık sistemdeki BE değerinin karşılığı sekizlik sistemde (276) değerine eşittir.
```

## Onaltılık Sistemden(Hexadecimal) > Onluk Sisteme(Decimal)

Yukarıda zaten buna değinmiştik. Kısaca değinip geçelim. Sağdan 0 ile başlayarak her sayı 16 üzeri sayının bulunduğu basamak değeriyle çarpılır. Ardından basamak değerleri toplanır.

Onaltılık sistemde **BE** değerinin onluk sistemde karşılığını bulalım...

```
-> B * (16¹) + E * (16⁰)

-> (11 * 16) + (14 * 1) 

-> 176 + 14 = 190
```
```
Sonuç olarak onaltılık sistemdeki BE değerinin karşılığı onluk sistemde (190) değerine eşittir.
```