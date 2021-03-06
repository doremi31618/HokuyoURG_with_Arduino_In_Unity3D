# [Unity]URG and Arduino control with light animation system

![image](https://github.com/doremi31618/HokuyoURG_with_Arduino_In_Unity3D/blob/master/Pic/ezgif.com-video-to-gif.gif). 

更新： 
========
1.新增動畫系統.  

2.新增動畫系統實作. 

![image](https://github.com/doremi31618/HokuyoURG_with_Arduino_In_Unity3D/blob/master/Pic/AnimationSystemDemo.gif).


專案說明：
========
使用Hokuyo URG(雷達眼)偵測周圍經過的體驗者，並利用Arduino + Relay（繼電器)同步控制日光燈管的開關。  

架構：Hokuyo(data input) -> Unity3D -> Arduino -> Relay -> LED

如何連接Hokuyo?
=============
mac.
----
step1插上網路線(或USB). 

step2設定電腦. 

  1. 打開網路偏好設定. 
  
  2. 調整以下設定. 
  
    1) 設定ipv4 -> 手動. 
    
    2) ip位置 -> 192.168.0.0to255(只要不是10都可以) 或者 192.168.1.0to255.  
    
    3) 子網路遮罩 -> 255.255.255.0. 
    
step3 設定完成. 

window 10:
----------
step1插上網路線(或USB).  

step2設定電腦. 

  1. 開啟網路和網際網路設定.
  
  2. 右邊欄位 進入 乙太網路. 
  
  3. 找到左邊欄位 進入 網路和共用中心. 
  
  4. 點選乙太網路. 
  
  5. 點選內容. 
  
  6. 在欄位(這個連線使用以下項目)中找到網際網路通訊協定第4版(TCP/IPv4)並點擊. 
  
  7. 點選 內容. 
  
  8. 調整以下設定. 
  
    1) 使用下列的ip位置 -> 勾選. 
    
    2) ip位置->192.168.0.0to255(只要不是10都可以)或者192.168.1.0to255. 
    
    3) 子網路遮罩 -> 255.255.255.0. 
    
step3 設定完成.

如何連接並設定Arduino?
==================
mac & window 10：  
----------------
step1插上USB線並連接你的Arduino.  

step2打開ArduinoIDE.  

  1. 確認開發板是否正確(工具->開發版). 
  
  2. 確認序列埠是否連接Arduino(工具->序列埠). 
  
  3. 打開 : 檔案 -> 範例 -> firmata -> standard firmata 並且上傳到Arduino 
  
step3 設定完成. 

專案內
---------
1. 打開專案. 

2. Scenes -> ArduinoWithURG 按下播放鍵. 

3. 連接Arduino（左上角有一個Connect鍵，然後喝杯咖啡這會花一點時間). 

4. 點擊中間第三個按鈕(Hokuyo的掃描範圍會及時同步在Scene視窗中). 

5.點擊左上角最右邊的按鈕。

6.完成！  
  
參考資料：
==============
Hokuyo Reference 1 
[https://github.com/curiosity-inc/urg-unity](https://github.com/curiosity-inc/urg-unity)  

Hokuyo Reference 2. 
[https://github.com/inoook/UnityURG](https://github.com/inoook/UnityURG)  

Unity With arduino asset. 
[http://www.uniduino.com](http://www.uniduino.com). 
