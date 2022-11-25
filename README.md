# Veri yapıları ve Algoritmalar
**[22,27,16,2,18,6] -> Insertion Sort** 

1. aşama :*2 en küçük sayı olduğu için en başa geçer. [2,27,16,22,18,6]*
2. aşama :*6, diğer en küçük sayı olduğu için 2'nin yanına geçer. [2,6,16,22,18,27]*
3. aşama :*18, 22den küçük olduğu için 16'nın yanına geçer.  [2,6,16,18,22,27]*
- : **Diğer tüm rakamlar küçükten büyüğe göre sıralandığı için işlem bitmiştir.**


**Dizideki eleman sayısı n olsun. Big-O yöntemine göre sıralama yapılırken işlem sayısı da n olur. Son işlem sayısı 1 olana kadar devam eder.**
**[22,27,16,2,18,6] dizisinde 6 tane eleman vardır, yani 6 tane işlem yapılacaktır demektir. Şöyle ki,**

1. n-> 6 tane işlem,
2. en küçük elemanı (yani birinci) bulmak için (n-1)-> 6-1=5 tane işlem,
3. ikinci elemanı bulmak için (n-2)-> 6-2=4 tane işlem,
4. adımda üçüncü elemanı bulmak için (n-3)-> 6-3=3 tane işlem,
5. adımda dördüncü elemanı bulmak için (n-4)-> 6-4=2 tane işlem yapılır.
6. Altı elemanlı dizi olduğu için daha fazla işlem yapılmasına gerek yoktur çünkü son eleman altıncı elemandır.-
7. Bu algoritmada n+(n-1)+(n-2)+(n-3)+(n-4)+1 kadar işlem yapılır. Bu işlemin formülü: [n(n+1)]/2'dir. Bu formül sadeleştirilerek: (n²+n)/2 elde edilir.
8. Big-O Notation'da kat sayı önemsizdir; yani domine eden fonksiyon n² alınır.

- Big-O değeri = O(n²)



 **Time Complexity: Dizi sıralandıktan sonra 18 sayısı aşağıdaki case'lerden hangisinin kapsamına girer? Yazınız**

*[2,6,16,18,22,27] olarak sonuçlandığı için ve "18" ortada kaldığı için Average case'e girer.*

**[7,3,5,8,2,9,4,15,6] dizisinin Selection Sort'a göre ilk 4 adımını yazınız.**
- En küçük "2" olduğu için, 2 ve 7'nin yerini değiştireceğiz. **[2,3,5,8,7,9,4,15,6]** n + (n-1)
- 3 diğer en küçük olduğu için olduğu yerde kalır, 4 rakamı 3 ve 5 arasına konulur. **[2,3,4,5,8,7,9,15,6]**  ( n-2)
- 6 , 5 ve 8 arasına geçer. **[2,3,4,5,6,8,7,9,15]** (n-3)
- 7, 6 ve 8 arasına geçer. **[2,3,4,5,6,7,8,9,15]** (n-4)
