---
weight: 3
title: "Süper Ekonomik Blog Sitesi"
date: 2020-03-04T16:29:41+08:00
draft: false
author: "Cem Celal Altınay"
authorLink: "https://cemcelalaltinay.dev"
description: "Hugo kullanımı basit temel web sitesi aracı olup statik siteler için harika bir çözümdür."
images: []
resources:
- name: "featured-image"
  src: "featured-image.png"

lightgallery: true
---

**Hugo** temel statik siteler yapmak için kullanılan veritabanı olmamaksızın çalışan web site tool aracıdır. **Hugo** kullanımı kolay açık kaynaklı ve tamamen ücretsizdir. Bu sayede uygun fiyatlı bir web site üretmek mümkündür. 
Github Pages + Hugo + Google Domains = Süper ekonomik web sitesi..

## Hugo Nasıl İndirilir Kurulur?
    
Daha önce hiç windows ile kurulum yapmadığım için Linux üzerinden anlatacağım. Hugo kurulumu çok basit.

https://gohugo.io/installation/linux/

Kurulum için git kullanmamız gerekiyor. Git kurulu değilse kurmanızı tavsiye ederim.

Debian Linux için;

sudo apt install hugo

Kodu ile kurulumumuzu yapıyoruz.

Daha sonra "https://gohugo.io/getting-started/quick-start/" olduğu gibi adımları takip ediyoruz.

```
hugo new site test-sitem
cd test-sitem
git init
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
echo "theme = 'ananke'" >> hugo.toml
hugo server
```

Artık"http://localhost:1313" adresinden yeni sitenizi görebilirsiniz. Sitenin config dosyası üzerinden düzenlemeleri yapabilir, content klasörü içerisinden içerikleri değişebilirsiniz.

Tüm işlemleriniz bittikten sonra Ctrl+C ile hugo server durdurmanız daha sonra sitenizin bulunduğu klasörde "hugo" komutu ile derlemeniz gerekmektedir.