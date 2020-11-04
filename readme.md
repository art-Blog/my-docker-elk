[架構]:./document/images/01.png
[APM-Server RUM]:https://partypeopleland.github.io/artblog/2019/07/09/APM-Server-RUM/
[ELK Stack on Docker]:https://partypeopleland.github.io/artblog/2019/06/27/ELK-Stack-on-Docker/
[elastic search 練習 audit log]:https://partypeopleland.github.io/artblog/2019/07/02/elastic-search-%E7%B7%B4%E7%BF%92-audit-log/
[Elastic stack (ELK) on Docker]:https://github.com/deviantony/docker-elk


## 架構

![][架構]

網站的IIS Log存放於` d:\IISLog\W3SVC1`，由`filebeat`讀取目錄文件傳送給`logstash`  

網站本身Layout加上`apm agent`，發送至`apm server`，轉發至`elasticSearch`，並由`kibana`的APM功能查看資料

## Blog

相關的ELK練習文章都是以這個docker-compose.yml為基礎而延伸的練習，也因為如此，文章內的東西很可能不會隨著更新，參考的話還是以`github`資料為主，文章為輔

1. [APM-Server RUM][APM-Server RUM]
1. [ELK Stack on Docker][ELK Stack on Docker]
1. [elastic search 練習 audit log][elastic search 練習 audit log]

## 參考

docker-compose的檔案內容是取自[Elastic stack (ELK) on Docker][Elastic stack (ELK) on Docker]，這個Github為想要接觸ELK技術的人提供了一個最簡易的途徑，降低了許多的門檻，很謝謝他，如果可以的話也請各位幫他點個Star
