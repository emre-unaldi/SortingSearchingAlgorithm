# `Insertion Sort Project`
```javascript
[22,27,16,2,18,6]
```
1. Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.
3. Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız

- **Average case**: Aradığımız sayının ortada olması

- **Worst case**: Aradığımız sayının sonda olması

- **Best case**: Aradığımız sayının dizinin en başında olması.

## 1. Cevap

> Adım 1 : `[22]` : Dizi başlangıçta sıralıdır 

> Adım 2 : `[22, 27]` : 27, 22'den büyük olduğu için yer değiştirir

> Adım 3 : `[16, 22, 27]` : 16, 22'den küçük olduğu için 22'nin soluna eklenir

> Adım 4 : `[2, 16, 22, 27]` : 2, 16'dan küçük olduğu için 16'nın soluna eklenir

> Adım 5 : `[2, 16, 18, 22, 27]` : 18, 16'dan büyük olduğu için yer değiştirir

> Adım 6 : `[2, 6, 16, 18, 22, 27]` : 6, 16'dan küçük olduğu için 16'nın soluna eklenir
>> `[2, 6, 16, 18, 22, 27]` : Dizi artık sıralanmış haldedir.

## 2. Cevap
>Insertion Sort'un Big-O gösterimi `O(n^2)`'dir, yani bu algoritma en kötü durumda dizi uzunluğunun karesi kadar işlem yapar.

## 3. Cevap
>Average case (Ortalama durum): Aradığımız sayının dizinin ortasında olması ihtimali en yüksektir. Bu nedenle 18 sayısı ``"Average case"`` kapsamına girer.
----
----

# ``Selection Sort Project``
```javascript
[7,3,5,8,2,9,4,15,6]
```
- Yukarıdaki dizinin Selection Sort'a göre ilk 4 adımını yazınız.

> Adım 1 : `[2, 3, 5, 8, 7, 9, 4, 15, 6]` : Dizinin en küçük elemanı olan 2, ilk sıraya getirilir

> Adım 2 : `[2, 3, 4, 8, 7, 9, 5, 15, 6]` : Dizinin en küçük ikinci elemanı olan 4, 3'ün yerine getirilir

> Adım 3 : `[2, 3, 4, 5, 7, 9, 8, 15, 6]` : Dizinin en küçük üçüncü elemanı olan 5, 8'in yerine getirilir

> Adım 4 : `[2, 3, 4, 5, 6, 9, 8, 15, 7]` : Dizinin en küçük dördüncü elemanı olan 6, 7'nin yerine getirilir
>> Bu adımlar sonucunda dizinin ilk 4 elemanı sıralanmış olur.

----

# `Merge Sort Project`
```javascript
[16,21,11,8,12,22]
```
1. Yukarıdaki dizinin Merge Sort türüne göre aşamalarını yazınız.
2. Big-O gösterimini yazınız.

## 1. Cevap
> Adım 1 : Dizi ikiye Bölünür. 
```
Sol yarı: [16, 21, 11]
Sağ yarı: [8, 12, 22]
```
> Adım 2 : Sol ve sağ yarılar ayrı ayrı sıralanır.
```
Sol yarı: [11, 16, 21]
Sağ yarı: [8, 12, 22]
```

> Adım 3 : Birleştirme işlemi yapılır.
>> Dizi artık sıralanmış haldedir: [8, 11, 12, 16, 21, 22]
```
Birleştirilmiş dizi: [8, 11, 12, 16, 21, 22]
```

## 2. Cevap
> Merge Sort'un Big-O gösterimi `O(nlogn)'`dir, yani bu algoritma **nlogn** zamanında çalışır, where n dizi uzunluğunu temsil eder.
----
----
# `Binary Search Tree Project`
```javascript
[7, 5, 1, 8, 3, 6, 0, 9, 4, 2]
```
- Yukarıdaki dizinin Binary Search Tree aşamalarını yazınız.

> Adım 1 : 7 değerine sahip kök düğümü oluşturun.
```javascript
7 -> Root
```

> Adım 2 : 5 dizideki ikinci öğedir, dolayısıyla kökün soluna gider.
```javascript
 7 -> Root
  \
   5
```

> Adım 3 : 1, kökten (7) küçüktür, dolayısıyla 5'in soluna gider.
```javascript
 7 -> Root
  \
   5
  /
 1
```

> Adım 4 : 8, kökten (7) büyüktür, dolayısıyla kökün sağına gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
```

> Adım 5 : 3, 1'den büyük ancak 5'ten küçüktür, dolayısıyla 1'in sağına gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
  \
   3
```

> Adım 6 : 6, 3'ten büyük ancak 5'ten küçüktür, dolayısıyla 3'ün sağına gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
  \
   3
    \
     6
```


> Adım 7 : 0, kök (7)'den küçüktür, dolayısıyla 7'nin soluna gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
  \
   3
    \
     6
    /
   0
```

> Adım 8 : 9, kök (7)'den büyüktür, dolayısıyla 7'nin sağına gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
  \
   3
    \
     6
    /
   0
    \
     9
```

> Adım 9 : 4, 3'ten büyük ancak 5'ten küçüktür, dolayısıyla 3'ün sağına gider.
```javascript
 7 -> Root
  \
   5
  / \
 1   8
  \
   3
    \
     6
    / \
   0   9
    \
     4
```

> Adım 10 : 2, 1'den büyük ancak 3'ten küçüktür, dolayısıyla 1'in sağına gider.
```javascript
 7 -> Root
 \
  5
 / \
1   8
 \   
  3
   \
    6
   / \
  0   9
   \
    4
     \
      2
```