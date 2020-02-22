## lesson1_C


_1.#include<>:類似import. _

> #include <cs50.h> 

_2. clang 使程式碼轉換成二進位，讓電腦讀懂. _
clang -o(可命名) 原本檔名  
EX:hello.c(檔名) 正常輸出是a.out  
可以變成clang -o pp hello.c. 
把a.out輸出成pp(變換檔名)

> clang -o ____ -l___. 

> _l 連結某個包裝（例如cs50.h）. 

> make 檔名


_3. ./檔名_
> clang輸出的二進位檔
> ./在當前目錄執行此檔

![](https://i.imgur.com/HDgm8Bc.png)

_4. \n換行符號  _
_5. ls 可以直接叫出目錄的所有檔案_  
前面有標記＊為machine code機器代碼;其他為源代碼;aaa/：/代表資料夾

_6. rm 刪除檔案;mkdir 創立目錄;rmdir刪除目錄. _
![](https://i.imgur.com/H3tIBR8.jpg)



_7.資料型態 _ 

![](https://i.imgur.com/GWoA29r.png)
例如在上例中，整數 int 的記憶體空間是 4 個位元組，可以儲存的整數範圍為 -2147483648 至 2147483647，如果儲存值超出這個範圍的話稱之為「溢值」 （Overflow），會造成程式不可預期的結果。
整數計算範圍的方式很簡單，例如 int 整數佔 4 位元組的話，可儲存範圍為 2^32 / 2，除以 2 是因為要分另一半儲存負整數的關係，整數的最左邊位元被用來表示正負號，如果最左邊位元為 0 表示正號，若為 1 表示負號。
![](https://i.imgur.com/ugEips9.png)

資料來源：https://programming.im.ncnu.edu.tw/Chapter5.htm

_8. do while 迴圈. _
 do statement while ( expression ) ;  
 
執行迴圈的主體後，會評估 do-while 陳述式中的 expression。 因此，迴圈主體一律至少執行一次。  

do
{
    y = f( x );
    x--;
} while ( x > 0 );

在這個 do-while 陳述式中，會執行 y = f( x ); 和 x--; 兩個陳述式，無論 x 的初始值為何。 接下來會評估 x > 0。 如果 x 大於 0，會再次執行陳述式主體，並重新評估 x > 0。 只要 x 保持大於 0，陳述式主體就會重複執行。 x 變成 0 或負值時，do-while 陳述式會終止執行。 迴圈主體至少執行一次。


_9. **佔位符**_
> %s字串佔位符

> %f浮點數佔位符

> %.2f 算到小數點後第二位

> %i 整數佔位符

> %d 整數佔位符


_10. for(初始 ;條件 ;迴圈 ) _

是產生無限迴圈的慣用方法，其只能使用 break、goto 或 return 陳述式來結束。

_11.算術溢出（整數溢出）：_

在電腦領域裡所發生的溢位條件是，執行單項數值計算時，當計算產生出來的結果是非常大的，大於暫存器或記憶體所能儲存或表示的能力限制。





