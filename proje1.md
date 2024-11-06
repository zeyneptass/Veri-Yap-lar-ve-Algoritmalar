# Veri Yapıları ve Algoritmalar Patika.dev Proje 1 Çözümleri

## Soru 1: Insertion Sort

**[22,27,16,2,18,6] -> Insertion Sort**

**Aşamalar:**

Aşama 1: İlk aşamasında dizi [22,27,16,2,18,6] şeklindedir. İlk elaman [22] kalır
Aşama 2: İkinci eleman (27) > ilk eleman (22) olduğundan [22,27] olarak kalır.
Aşama 3: Üçüncü eleman (16) < 27  ve (16) < 22 olduğundan 22'nin soluna yerleştirilir. [16,22,27] olur.
Aşama 4: Dördüncü eleman (2) alırız. (2) < 16, (2) < 22, (2) < 27 olduğundan en başa yerleştiril. [2,16,22,17] olur.
Aşama 5: Beşinci eleman (18) alırız. (18) > 2, (18) > 16, (18) < 22, (18) < 27 olduğundan, 16'nin soluna yerleştirilir. [2, 16, 18, 22, 27] olur.
Aşama 6: Altıncı eleman (6) alırız. (6) > 2 ve 16,18,22 ve 27'den küçük olduğu için 16'nin soluna yerleştirilir.  [2, 6, 16, 18, 22, 27] 

**Sonuç:** Insertion Sort'a göre sıralanmış dizi [2, 6, 16, 18, 22, 27] olur.

**Big-O Gösterimi:**

Çözüm: Average case ve Worst case => O(n^2) iken, Best case => O(n) 

**Time Complexity:**

Çözüm: Dizi sıralandıktan sonra 18 sayısı dizinin ortalarında yer aldığı için average case kapsamına girer.

## Soru 2: Selection Sort

**[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.**

**Aşamalar:**

Adım 1: En küçük elemanı bulmak için tüm diziyi tararız ve bulunduğu elemanla yer değiştirerek dizinin en başına yazarız => [2, 3, 5, 8, 7, 9, 4, 15, 6]
Adım 2: Kalan elemanlardan en küçüğünü buluruz. En küçük eleman 3, zaten ikinci sırada olduğu için yer değiştirme yapılmaz => [2, 3, 5, 8, 7, 9, 4, 15, 6]
Adım 3: Kalan elemanlardan en küçüğünü buluruz. En küçük eleman 4, üçüncü sıradaki 5 ile yer değiştirilir => [2, 3, 4, 8, 7, 9, 5, 15, 6]
Adım 4: Kalan elemanlardan en küçüğünü buluruz. En küçük eleman 5, dördüncü sıradaki 8 ile yer değiştirilir => [2, 3, 4, 5, 7, 9, 8, 15, 6]