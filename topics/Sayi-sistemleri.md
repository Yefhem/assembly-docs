# Sayı Sistemleri 

## Binary System (İkili Sistem)

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

### Örnek 1

İkili sistemde **00001001** değerini inceleyelim. Sağdan başlarsak;

```
2 üzeri 0 = 1		(1)
2 üzeri 1 = 2 		(0)
2 üzeri 2 = 4		(0)
2 üzeri 3 = 8		(1)
2 üzeri 4 = 16		(0)
2 üzeri 5 = 32		(0)
2 üzeri 6 = 64		(0)
2 üzeri 7 = 128	    (0)
```

Aktif olan bitler görüldüğü üzere sıfırıncı ve üçüncü bitler bunların toplamları ise **1 + 8 = 9** olarak bulunur.

### Örnek 2

İkili sistemde farklı bir örnek olarak virgüllü bir değer olan **1111,011** değerini inceleyelim. Burada dikkat edilmesi gereken nokta;

Virgülün sol tarafında kalan kısım, yukarıdaki örnekte olduğu gibi sağdan sola doğru 2 üzeri 0 dan başlanarak her basamakta 2’nin bir kuvveti alınır. Virgülün sağ tarafında ise soldan sağa doğru 2 üzeri -1 den başlanarak her basamakta 2’nin bir kuvveti alınır.(-1, -2, -3 olarak devam eder yani kuvvet küçülür.)  

```
2 üzeri -3 = 1/8	(1)
2 üzeri -2 = 1/4 	(1)
2 üzeri -1 = 1/2	(0)
,
2 üzeri 0 = 1		(1)
2 üzeri 1 = 2		(1)
2 üzeri 2 = 4		(1)
2 üzeri 3 = 8	    (1)
```

Aktif olan bitleri toplayacak olursak...

```
0,125 + 0,25 + 1 + 2 + 4 + 8 = 16,375
```

**Not2:** 1/8 ve 1/4 değerlerinin ondalık karşıtları olan 0,125 ve 0,25 değerlerini yazdık. Kafa karışıklığı doğurmasın. 

## Dönüşümler

### İkili Sistemden(Binary) > Onluk Sisteme(Decimal) 

Bunun örneği yukarıdaki örneklerde yaptık. Yine de bir örnek daha yapalım.

İkili sistemde **01011000** değerinin onluk sistemde karşılığını bulalım...

```
2 üzeri 0 = 1		(0)
2 üzeri 1 = 2 		(0)
2 üzeri 2 = 4		(0)
2 üzeri 3 = 8		(1)
2 üzeri 4 = 16		(1)
2 üzeri 5 = 32		(0)
2 üzeri 6 = 64		(1)
2 üzeri 7 = 128	    (0)
```

Aktif bitleri toplayarak onluk sistemde karşılığını bulalım.

```
8 + 16 + 64 = 88
ikili sistemde 01011000 = onluk sistemde 88 değerine eşittir.
```

### İkili Sistemden(Binary) > Sekizlik Sisteme(Octal)

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

### İkili Sistemden(Binary) > Onaltılık Sisteme(Hexadecimal)

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