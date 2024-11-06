# Veri Yapıları ve Algoritmalar Patika.dev Proje 2 Çözümleri

## Soru 1: [16,21,11,8,12,22] -> Merge Sort

```mermaid
graph LR
A[16, 21, 11, 8, 12, 22]  --> B([16, 21, 11])
A --> C([8, 12, 22])
B --> D(16) ----> Q(11,16,21)
B --> E(21, 11)
E --> F(21) --> X(11,21) 
E --> G(11) --> X(11,21) --> Q(11,16,21)


C --> H(8) -----> S(8,12,22)
C --> I(12, 22)
I --> J(12) --> W(12, 22) 
I --> K(22) --> W(12, 22) ---> S(8,12,22)

```

## Soru 2: Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.

**Aşamalar:**

Adım 1 : [16, 21, 11] | [8, 12, 22]  

Adım 2: [16] | [21, 11] | [8] | [12, 22]  

Adım 3: [16] | [21] | [11] | [8] | [12] | [22]

Adım 4: [16] | [11, 21] | [8] | [12]  [22]

Adım 5: [16] | [11, 21] | [8] | [12, 22]

Adım 6: [11, 16, 21] | [8, 12, 22]

Adım 7: [8, 11, 12, 16, 21, 22]  



## Soru 3: Big-O gösterimini yazınız.

Merge Sort'un Big-O gösterimi O(n log n)'dir.


