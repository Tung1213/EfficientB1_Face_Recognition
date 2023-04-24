# 前提
近年爆發新冠肺炎疫情，為了避免染上疫情，無時無刻戴著口罩，口罩戴法分三種情況: 1.沒有戴、2.沒有戴好、3.有戴好，若利用手機進行解鎖，在口罩沒戴好和完全戴好口罩情況，有些手機可能會有辨識錯誤的情況，導致無法解鎖，須整張臉才進行辨識，相當不便，也可能脫了口罩影響到自己或其他人，本研究進行再不脫口罩或口罩戴一半時進行人臉辨識。

利用EfficientNet-B1模型開發門禁管制辨識系統，門的部分利用MG996R伺服機模擬作為門打開和關閉的動作並製作出簡易門禁模型。身份辨識錯誤時，利用MQTT推播機制將推播訊息推播到監控網頁，讓使用者可在監控網頁上看到推播的通知並可以開啟相機即時查看門外情況和從資料庫讀取人臉影像照片並儲存到本地檔案裡，身份辨識成功，大門開啟並提醒或警告口罩是否戴好

# 【人臉辨識流程】

![image](https://user-images.githubusercontent.com/58096503/233927348-7c5d42c8-ada8-4c14-b413-83876530763b.png)


# 【門禁辨識流程】

![image](https://user-images.githubusercontent.com/58096503/233926814-d325cd05-9006-4d81-a5ec-b7302932ee10.png)



# 【門禁監控系統網頁設計】
使用 1. HTML、2. CSS3、3. JavaScript、4. Bootstrap3、5. jQuery進行網頁開發 

![image](https://user-images.githubusercontent.com/58096503/233923276-8e69bda6-ad7e-4fa0-a208-2f449e6dbdb8.png)

# 【門禁監控系統網頁功能】

主要分為三大功能

1. 防盜系統功能-此功能打開，當有不明人士進行人臉解鎖時，會將警告訊息推播到網頁，當使用者看到會立馬報警處理或進行其他處理。

2. 查看影像功能-當有不明人士進行人臉解鎖時，會將使用者的影像拍攝下來並儲存到本地端電腦，即使當下沒看到人，也可以查看儲存下來的影像。

3. 及時觀看功能-當有不明人士進行人臉解鎖時，看到推播的警告訊息時，能夠開啟相機及時查看當前門外狀況。



# 【模擬環境】


![image](https://user-images.githubusercontent.com/58096503/233928356-ba09ead5-9013-479f-adb8-00aad46d0a3a.png)
