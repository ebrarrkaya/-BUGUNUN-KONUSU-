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
