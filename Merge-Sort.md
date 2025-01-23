# **MERGE SORT PROJESİ**

*[16,21,11,8,12,22] -> Merge Sort*

*Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.*

*Big-O gösterimini yazınız.*

---
## ***Verilen dizinin insertion sort adımları***


**Merge Sort**, "böl ve birleştir" yöntemine dayanır. Dizi sürekli olarak ikiye bölünür ve en küçük birimlere ayrıldıktan sonra sıralı bir şekilde birleştirilir. Aşamalar aşağıdaki gibidir:
## ***1. Bölme Aşaması***
**Dizi: [16, 21, 11, 8, 12, 22]**
```
Dizi sürekli olarak ikiye bölünür:

1. bölme:
[16, 21, 11] ve [8, 12, 22]

2. bölme:
[16] [21, 11] ve [8] [12, 22]

3. bölme:
[16] [21] [11] ve [8] [12] [22]
```

## ***2. Birleştirme ve Sıralama Aşaması***
Bölünen alt diziler sırayla birleştirilip sıralanır:
```
İlk birleştirme:
[21] ve [11] birleştirilip sıralanır → [11, 21]
[12] ve [22] birleştirilip sıralanır → [12, 22]

Artık: [16], [11, 21], [8], [12, 22]

İkinci birleştirme:
[16] ve [11, 21] birleştirilip sıralanır → [11, 16, 21]
[8] ve [12, 22] birleştirilip sıralanır → [8, 12, 22]
Artık: [11, 16, 21] , [8, 12, 22]

Son birleştirme:
[11, 16, 21] ve [8, 12, 22] birleştirilip sıralanır → [8, 11, 12, 16, 21, 22]
```
---

## ***Big-O Gösterimi***
**Merge Sort**'un her aşaması şu şekilde değerlendirilir:

Bölme işlemi: Dizi her defasında ikiye bölünür. Bu, log(n) derinliğinde bir bölme oluşturur.

Birleştirme işlemi: Her seviyede n eleman birleştirilir.
Bu nedenle, Merge Sort’un zaman karmaşıklığı:

**Big-O: O(n log n)**

En kötü, en iyi ve ortalama durumların tümünde Merge Sort’un zaman karmaşıklığı aynıdır: O(n log n)

---


