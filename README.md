# kaan
cumle = input("bir metin girin")
sayi = int(input("sayi giriniz(saat)"))
def sayi_harfler(a):
    harf_sayisi = {}
    for harf in a:
        if harf in harf_sayisi:
            harf_sayisi[harf] += 1
        else:
            harf_sayisi[harf] = 1
    for harf, b in harf_sayisi.items():
        print(harf, "=", b, " tane")
print()
sayi_harfler(cumle)
def saat(yukseklik):
    print()
    for c in range(yukseklik + 1, 0, -1):
        print(("* " * c).center(27))
    for c in range(1, yukseklik + 2):
        print(("* " * c).center(27))
saat(sayi)
##asal sayı
sayi=int(input("Sayıyı Girin : "))
if sayi > 1:
   
   for i in range(2,sayi):
       if (sayi % i) == 0:
           print(sayi," Asal Sayı Değildir.")
           break
   else:
       print(sayi," Asal Sayıdır.")
 
else:
   print(sayi," Asal Sayı Değildir.")
 ##
dosya = open()
satirlar = dosya.read().split()
dosya.close()
dosya = open()
for satir in satirlar:
  boyut, karakter = satir.split(&quot; &quot;)
    for i in range(int(boyut),0,-1):
      for j in range(int(boyut)-i+1):
        dosya.write(" ")
      for j in range(2*i-1):
        dosya.write(karakter)
      dosya.write("\n")

dosya.close()
n = 5
for i in range(n):
    for j in range(n-i):
        print(" ", end="")
    for k in range(i+1):
        print("*", end="")
    print()
 ##
 cumle = input("Bir cümle yazınız: ")
kelimeler = cumle.split(" ")
sayilar = []
for k in range(len(kelimeler)):
     gelen_kelime = kelimeler[k]
     say = 0
     for j in range(len(gelen_kelime)):
         say+= 1
     sayilar =sayilar + [say]
