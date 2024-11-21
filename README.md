# Merge Sort
[16,21,11,8,12,22]

Yukarıdaki dizinin sort türüne göre aşamalarını yazınız.
Big-O gösterimini yazınız.

---------------------------------------------------------------

**Merge Sort Aşamaları:**
Başlangıç dizisi: [16, 21, 11, 8, 12, 22]

*İlk bölme:*

Diziyi ikiye bölelim:
Sol: [16, 21, 11]
Sağ: [8, 12, 22]
Sol tarafın bölünmesi:

Sol dizi [16, 21, 11] ikiye bölünür:
Sol: [16]
Sağ: [21, 11]
Sağ tarafın bölünmesi (21, 11):

[21, 11] dizisini ikiye bölelim:
Sol: [21]
Sağ: [11]
Bu diziler tek elemanlı oldukları için sıralıdır.
Birleştirme işlemi (Sol: [21], Sağ: [11]):

[21] ve [11] sıralandığında: [11, 21]
Sol tarafın birleştirilmesi:

[16] ile [11, 21] dizileri birleştirilir:
[11, 16, 21]
Sağ tarafın bölünmesi (8, 12, 22):

[8, 12, 22] dizisi zaten sıralı olduğu için doğrudan geçilir:
[8, 12, 22]
Son birleştirme (Sol: [11, 16, 21], Sağ: [8, 12, 22]):

[11, 16, 21] ile [8, 12, 22] dizileri birleştirilir:
[8, 11, 12, 16, 21, 22]
Sonuç: [8, 11, 12, 16, 21, 22]

**Big-O Gösterimi:**

Merge Sort'un zaman karmaşıklığı O(n log n)'dir. Bunun nedeni:
n elemanlı diziyi her adımda ikiye böldüğümüz için log n seviyelerine iniyoruz.
Her seviyede tüm n elemanları karşılaştırmamız gerektiği için O(n) işlem yapılır.
*Best Case:* O(n log n) — Dizi sıralı olsa bile Merge Sort her durumda bölme ve birleştirme işlemleri yapacaktır.
*Worst Case:* O(n log n) — Dizi ters sıralı olsa bile aynı şekilde çalışacaktır.
