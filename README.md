# Patika-Veri-Yapilari
Patika.dev üzerinde veri yapıları ve algoritmalar modülünün son ödevi.

# Insertion Sort Ödevi

[22,27,16,2,18,6] -> Insertion Sort

* Yukarı verilen dizinin sort türüne göre aşamalarını yazınız.
* Big-O gösterimini yazınız.
* Time Complexity: Average case: Aradığımız sayının ortada olması,Worst case: Aradığımız sayının sonda olması, Best case: Aradığımız sayının dizinin en başında olması.
* Dizi sıralandıktan sonra 18 sayısı hangi case kapsamına girer? Yazınız.
* [7,3,5,8,2,9,4,15,6] dizisinin Insertion Sort'a göre ilk 4 adımını yazınız.

# Çözümler

* Insertion sort aşamaları:
```
 [22|,27,16,2,18,6]
 [22,27|,16,2,18,6]
 [16,22,27|,2,18,6]
 [2,16,22,27|,18,6]
 [2,16,18,22,27|,6]
 [2,6,16,18,22,27]
```
* Big-o gösterimleri:

  * Average Case: O(n^2)
  * Worst Case: O(n^2)
  * Best Case: O(n)

* Time Complexity
  * Average case: Birden fazla cevap mevcut. Dizinin hemen hemen sıralanmış olması diyebiliriz.
  * Worst case: Dizinin büyükten küçüğe sıralanmış hali. 
  * Best case: Dizinin küçükten büyüğe sıralanmış hali.
* 18 sayısı
  * 18 sayısı average case kapsamına girer.
* [7,3,5,8,2,9,4,15,6] ilk 4 adımı.
```
 [7|,3,5,8,2,9,4,15,6]
 [3,7|,5,8,2,9,4,15,6]
 [3,5,7|,8,2,9,4,15,6]
 [3,5,7,8|,2,9,4,15,6]
```

# Merge Sort Ödevi
[16,21,11,8,12,22] -> Merge Sort

* Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
* Big-O gösterimini yazınız.

# Çözümler
* Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
```
 
 [16,21,11,8,12,22] ilk önce diziyi ikiye böleriz
 * [16,21,11]     [8,12,22]
 Daha küçük parçalar etmek için 2 ye bölmeye devam ediyoruz.
 * [16]   [21, 11]   [8]   [12,22]
 Dizi bölünemeyecek hale geldiği için her birini kendi içinde sıralamaya başlarız.
 * [16]   [11,21]   [8,12]   [22]
 Birleştirme işlemine başlıycaz fakat birleştirirken sıralamaya devam ederiz.
 * [11,16,21]   [8,12,22]
 Tekrar birleştireceğiz ve sıralamaya devam ediyoruz.
 * [8,11,12,16,21,22]
 Sıralı dizimizi elde ettik.
 
```
* Big-O gösterimini yazınız.
  * 3 durum içinde Big-o gösterimi O(nlogn) olur 
