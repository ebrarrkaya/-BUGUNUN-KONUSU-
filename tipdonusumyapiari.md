# Tip Dönüşüm Yapıları
Python'da tip dönüşümleri, bir veri türünden başka bir veri türüne dönüşüm yapmaktır. Yani bir veri türünü mantıklı olacak şekilde farklı bir veri türüne dönüştürmektir. Bu dönüşümler, verileri doğru formatta kullanabilmek veya işleyebilmek için kullanılmaktadır. Tip dönüşümlerini kullanıcıdan girdi almadan önce kullanmak çok önemlidir. Örneğin: Kullanıcıdan sayısal bir değer almak istiyorsak input() fonksiyonundan önce uygun tip dönüşüm fonksiyonunu kullanmamız gerekir. Aksi takdirde girilen değeri, Python string bir ifade olarak algılayıp sayısal işlemleri doğru bir şekilde gerçekleştirmeyecektir. 
İşte Python'da yaygın olarak kullandığımız sayısal tip dönüşümü yapıları:
# int() 
Integer bildiğimiz üzere tam sayıyı ifade etmektedir. int() yapısı ise, sayısal bir ifadeyi tam sayı değerine dönüştürür. Yani bizler kullanıcıdan bir tam sayı değeri almak istiyorsak input() fonksiyonunun başına int() fonksiyonumuzu yazmamız gerekir.
Örnek:
int(input("Bir sayi degeri giriniz:"))

Buradaki mantık, matematikte de kullanmış olduğumuz iç içe fonksiyonlardır. Önce içerideki işlem ve daha sonra dışarıdaki işlem gerçekleşir. Burada da önce kullanıcıdan sayı değeri alıp daha sonra bu değeri int ile tam sayı değeri olarak dönüştürmektedir.

<a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/74ce85019acde742723509e33d1fd70bf4ab25a5/e.png">HATALI KULLANIM VE ÇIKTISI İÇİN TIKLAYINIZ</a>

<a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/d272643ea0533534223035182292d1c3ff7c3c62/b.png">DOĞRU KULLANIM VE ÇIKTISI İÇİN TIKLAYINIZ</a>

# float()

float() yapısı ise girilen bir ifadeyi ondalıklı sayıya dönüştürür. Yalnız, girilen ifadenin temel olarak sayıyı temsil etmesi gerekiyor. Örneğin: "Yilmaz" değeri girilirse hata ile karşılaşırız. int() yapısında olduğu gibi float() yapısını kullanmak da matematiksel işlemler yapabilmek için oldukça önemlidir. Yine istenilen ifadenin ondalıklı sayı olarak tanımlanmasını istiyorsak input() fonksiyonundan önce float() yapısını kullanırız. Örnek kodlarımızı inceleyelim:

<a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/e26df61add4124ed039e956e3e71d17f45c55a95/R.png">HATALI KULLANIM VE ÇIKTISI İÇİN TIKLAYINIZ</a>

<a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/1a6f7c67c2abf193fc4abe73536bbc3ca002a538/A.png">DOĞRU KULLANIM VE ÇIKTISI İÇİN TIKLAYINIZ</a>

NOT: Eğer gireceğimiz değer, boy gibi ondalıklı bir sayı değeri olmalıysa muhakkak float() yapısını çağırmamız gerektiğine dikkat edilmelidir. Bu örnekte kütle değerini isterken tam sayı olarak hesaplamak istediğimiz için int() yapısını çağırdık fakat onun da küsüratlı olarak hesaplanmasını istiyorsak yine float() yapısını çağırmalıyız.

# str() 
Bu yapı ise, verileri karaktersel veri olarak dönüştürmektedir. Dönüştürül mek istenen veri sayı veya mantıksal veri olabilir. Daha iyi anlamak amacıyla örneklerimizi inceleyelim.

#Değişkenlerimizi oluşturduk ve tip dönüşümü yaptık

deger1=str(159)

deger2=str(True)

Tip sorgulaması gerçekleştirdik.

print("deger1 degiskeninin tipi", type(deger1))

print("deger2 degiskeninın tipi", type(deger2))

Görüldüğü gibi 2 farklı değişken oluşturduk. Bu değişkenlerde str() tip dönüşümünü çağırdık ve farklı verileri İçerisinde tanımladık Son olarak tip dönüşüm işlemini gözlemlemek amacıyla tip sorgulama işlemi gerçekleştirdik. Kodumuzu çalıştırdığımızda <a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/5f90b389e79632365008fd020850c62d7f1b289b/k.png">görüntüdeki gibi bir sonuçla karşılaşacağız.</a> 

# bool()
Bu yapımızla birlikte, farklı verilerden mantıksal verilere dönüşüm işlemlerı gerçekleştiririz. Burada dikkat edilmesi gereken bir durum var. Boş veriler ve etkisiz veriler False olarak tanımlanmaktadır. Yani 0 değeri False, 1.25 değeri ise True olarak döndürülmektedir. Boş bir metinsel veri ** False, "T" verisi ise True olarak döndürülmektedir. Bu örnekler çoğaltılabilir. Şimdi örnek kodumuzu inceleyelim.

#Değişkenlerimizi oluşturduk ve tip dönüşümü yaptık

deger1=bool(159)

deger2=bool("Ozgur")

deger3=bool(0)

#Tıp ve değeri çıktı aldık

print("deger1 degeri: () tipi () ".format(deger1,type(deger1)))

deger4-bool("")

print("deger2 degeri: () tipi () ".format(deger2, type(deger2)))

print("deger3 degeri: () tipi () ".format(deger3,type(deger3)))

print("deger4 degeri: () tipi {} ".format(deger4, type(deger4)))

Kodumuzu çalıştırdığımızda ise <a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/83e21a6f161773dd25d77f2c89fb62aa27cfb2d8/y.png">görüntüdeki gibi bir sonuçla karşılaşacağız.</a> 

Tabii ki kıyaslama işlemlerinde de kullanabilmemiz mümkündür. Bunun için olan örneğimizi inceleyelim.

deger1-bool (159-80)

deger2-bool(10-10)

Tip ve değeri çıktı aldık

print("deger1 degeri: () tipi () ".format(deger1, type(deger1)))

print("deger2 degeri: () tipi () ".format(deger2, type(deger2)))

Kodumuzu çalıştırdığımızda ise <a href="https://github.com/ebrarrkaya/-BUGUNUN-KONUSU-/blob/e776802dde81b6bd1b68993b74f1bc0aac8ad4cc/ss.png">görüntüdeki gibi bir sonuçla karşılaşacağız.</a> 

# Tip Dönüşümleri Kullanımları
# 1. Yöntem:
a=input()
a=int(a)
# 2. Yöntem:
a=int(input())

