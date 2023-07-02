---
weight: 3
title: "Recon Nedir?"
date: 2020-03-04T16:29:41+08:00
draft: false
author: "Cem Celal Altınay"
authorLink: "https://cemcelalaltinay.dev"
description: "Recon; siber güvenlikte hedef hakkında temel bilgi/istihbarat edinme eylemlerinin tümüne denir."
images: []
resources:
- name: "featured-image"
  src: "featured.jpg"

lightgallery: true
---
Hedef üzerinde sessizce veya sesli şekilde yapılan araştırma ve gözlemlere kısace Recon denir. Burada bulunan bilgiler bana göre terimler olup kendime göre yorumlar yapıyorum. Daha doğru bilgiler için aradığınız kaynak burası değil..

### 1 İstihbarat Nedir?
  Hedef hakkında elde edilmiş ve henüz işlenmemiş veriler bütünü olarak adlandırabiliriz. Örneğin hedefin kullandığı güvenlik yazılımları, API yazılımları, yazılım dili ve Host ediş yöntemi bunlara bir örnektir. Bu veriler ile bilinen zaafiyet araştırmaları veya bruteforce denemeleri bu elde edilen verilerin işlenmesidir.


### 2 Sessiz Recon Nedir?
İnternet üzerinden veya çeşitli kaynaklardan hedef ile hiç bir temasa geçmeden - PING v.b. - yapılan araştırmalardır. Bunların en temeli Google Dork. Ayrıca bakınız: 


### Sessiz Recon Toolları
    ```whois
    whois cemcelalaltinay.dev
    # Sorugusu ile hedef domain temel bilgileri öğrenilir
    ```
    ```dig
    dig cemcelalaltinay.dev A
    #domain adı ve görmek istediğiniz server tiplerinin bilgisini getirir
    ```



### 3 Sesli recon nedir?
Hedef sistem ile doğrudan iletişime geçerek olandır.Örn bruteforce ile subdomain bulunması yada kullanılan apileri anlamak için bilgi toolları çalıştırılması. Bu süreden sonra karşı taraf artık sizden haberdardır.


 ### Sesli Recon Toolları
  **recon-ng** (https://medium.com/@ahmet1birkan/web-tabanl%C4%B1-bilgi-toplama-recon-ng-4695d2c780a5) - Karmaşık -


**fuff**   -ffuf -w /dosyayolu -u hostname.com -h FUZZ.hostname.com -fc 403
    Çok işlevsel bir tool kesinlikle kurdu olunması lazım


**subfinder** - bakmam lazım - 

**shadon** - bakmam lazım -
  
**gobuster** -gobuster -u cemcelalaltinay.dev -w SecList/Discovery/DNS/top100.txt
Kullanımı harika kolay subdomain v.b. için fazlaca işlevsel tool. 

**netcat** - bakmam lazım yani kullandım ama ezbere copy+paste kullandım daha tam çözemedim.

**nmap** 
**nikto**
**tee**