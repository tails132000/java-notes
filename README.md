# java-notes
Currently self-learning java. A place to place the notes and codes
1.System 類
>屬性: out (例: System.out)、  in (例: scanner.in)、 error


-System類代表系統，系統級的很多屬性和控制方法都放置在該類的內部。該類位於"java.lang包"
-由於該類的構造器是private，無法創建該類的對象。其內部的成員變量和成員方法都是static的，很方便調用
-成員變量 Scanner scan = new Scanner(System.in);
	-System類內部包含in, out, err三個成員變量，分別代表標準輸入流(鍵盤輸入)，標準輸出流(顯示器)和標準錯誤輸出流(顯示器)  

成員方法
    - native long currentTimeMillis():
	返回當前的計算機時間，時間格式是當前計算機時間和GMT時間1970年1月1號0時0分0秒所差的毫秒數

    - void exit(int status):
	退出程序。其中status的值為0代表正常退出，非零代表異常退出。使用該方法可以在圖形介面編成中實現程序的退出功能等

    - void gc():
	請求系統進行垃圾回收。至於系統是否立刻回收，則取決於系統中垃圾回收算法的實現，以及系統執行時的情況

    - String getProperty(String key):
	獲得系統中屬性名為key的屬性對應的值。系統中常見的屬性名以級屬性的作用

