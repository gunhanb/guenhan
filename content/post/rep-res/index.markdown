---
title: Nasıl "reproducible research" yaparım?


# Summary for listings and search engines
summary: Nasıl "reproducible research" yaparım?

# Link this post with a project
projects: []

# Date published
date: "2016-04-20T00:00:00Z"

# Date updated
lastmod: "2016-10-27T00:00:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

authors:
- admin

tags:
- Academic

categories:
- R
---

Diyelim ki bir arkadaşınız yaklaşık bir sene önce tamamlamış olduğunuz bir *research* calışmanızdan birşey sordu. Calısmanıza dönüp analizleri tekrar gözden geçirmek, tablo ve figürleri *reproduce* edebilmeniz ne kadar vaktinizi alacaktır? Veya arkadaşınızı boşverin, sadece kendiniz 2 sene önce hazırlamış olduğunuz sunumdaki *result*larin tekrar elde etmeye calışsanız? Bu süreyi ve olası zahmeti azaltmanın (ve daha fazlası) metodu *reproducible research* yapmanız!


Eğer günlük hayattaki calışmalarınızda bir sekilde *data analysis* yapıyorsaniz, eski yontemler yerine *reproducible research* kullanmaniz belki biraz daha zahmetli ama uzun vadede kesinlikle daha faydali. 


Bir başka açıdan bakacak olursak, geleneksel rapor yazımında, sonuçları bir software de hesaplayip, sonra da hesaplamış oldugumuz sayılari elle sonuç bölümüne yazarız. Ama bu yöntem reproducible değil, data *software* e bağlı fakat sonuçlar yazdıgımız metne bağlı değil, dolayısıyla hata yapma ihtimali bir hayli yüksek. 


Bu konu tabiiki bayağı geniş ve kapsamlı, ayrica niyetim bir *manual* yazmak değil. Bu yazıda amacım kendi tecrübelerimden faydalanarak tamamen pratik açıdan reproducible research'u kısaca anlatmaya calişmak ([daha ayrıntılı bilgi için tıklayin](http://reproducibleresearch.net)). Turkce yazmamın amacı da bu konulardaki Türkçe materyallerin eksikliği. 


Ilk olarak data analysis'i hangi *software* de yapacagim sorusu karsimiza geliyor. Bir istatistikci oldugum icin buna verecegim cevap tabiki [**R**](https://www.r-project.org) (since **R** is made by statisticians for statisticians!). Ikinci olarak *typesetting* programimizi belirlememiz gerekiyor, raporu/makaleyi/tezi yazacagimiz veya sunumu hazirlayacagimiz program. Buna cevabimiz ise *LaTeX* olabilir. Fakat diger guclu bir alternatif ise [*Markdown*](https://daringfireball.net/projects/markdown/). Markdown ile hem pdf, word veya HTML output elde edebiliyoruz. Bu yazida *Markdown* kullanacagiz, cünkü bize
Ve ucuncu olarak bize uygun bir *text editor* gerekli, bunun icin de **Rstudio** yu kullaniyoruz. Sonunda sihirli dokunusu yapacak yani reproducible research u mumkun kilacak olan program (aslinda bir **R** *package*): **knitr**. Tam burada **knitr** in babasi olan programi hatirlatmam gerekiyor, saygi geregi **Sweave**. 


Dolayisiyla **knitr** ile birlikte bu uc program, **R** + Markdown + **Rstudio**, bize reproducible research yapabilmemiz icin yeterli ve bu arada hepsi de free software. Kisacasi bir tek *document* a hem LaTeX kodu hem de **R** kodunu yaziyorsunuz (.Rmd file) ve sonrasinda *compile* edip PDF inize kavusmus oluyorsunuz. Aslina bakarsaniz, **knitr** kullanarak reproducible research yapabilmemiz icin bu uc programin hicbiri farz degil, alternatif kombinasyonlara en sonda deginecegim. Rstudio nun sagladigi en onemli fayda ise *compile to PDF* adimini sadece tek bir tusa indirgiyor olusu.

## Basit bir ornek

*Base R* dan *cars* adli *dataset* i kullanacagiz. Bu dataset farkli arabalarin hizlari (*speed variable*) ve her bir arabanin durmak icin gerekli mesafelerini (*dist variable*) iceriyor. Bu datayi analiz etmek icin *linear regression* kullaniyoruz ve gerekli **R** kodu asagidaki gibi gosterebiliriz.



```r
fit <- lm(dist ~ speed, data = cars) # linear regression 
```


Tabii sonuclari -mesela bu ornekte *coefficients*- bir tabloda gostermek isteyebiliriz. Bunun icin de **xtable** (bir **R** package) bize yardimci olacak. Asagidaki **R** kodu bize gerekli HTML kodu veriyor, ve compile ettikten sonra da Tablo 1'i elde ediyoruz.




```r
library(knitr)
coefs <- matrix(coef(fit))
rownames(coefs) <- c("Intercept", "speed")
kable(coefs, label = "tab:coefs",
      digits = 2,
      row.names = TRUE, 
      col.names = "Estimate")
```



|          | Estimate|
|:---------|--------:|
|Intercept |   -17.58|
|speed     |     3.93|



Normal sartlarda tabloyu yaratan **R** kodu okuyucuya gostermeye gerek yok fakat ben ornek olmasi acisindan gosteriyorum.

Simdi ise *data visualization*. Asagidaki **R** kod ile Figure 1'i elde ediyoruz.


```r
library(ggplot2)
ggplot(cars, aes(x = speed, y = dist)) + geom_point() +
  geom_abline(intercept = coef(fit)[1], slope = coef(fit)[2])
```

<img src="{{< blogdown/postref >}}index_files/figure-html/figure-1.png" width="384" />

Bu ornekte damaginiza **knitr** kullanimindan bir tat calmayi amacladim.  

Benim ugrastigim problemlerde **knitr** in saglamis oldugu cok onemli diger bir fayda ise *cache* ozelligi. Simdi farz edin ki analiziniz yukaridaki gibi bir simple linear regression degil, mesela simulasyon yapiyorsunuz veya *bootstrapping*. Dolayisiyla islem saatler surebilir. Bu durumda **knitr** in cache ozelligini kullanabilirsiniz, ilk compilation da analiz yapilir (artik ne kadar suruyorsa) ve **knitr** sizin icin outputu kaydeder. Sonraki compilationlarda ise knitr kaydedilmis outputu kullanir!

Bu arada **knitr**'i her turlu farkli LaTeX *documentclass* icin kullanabilirsiniz, mesela rapor yazarken veya sunumunuzu hazirlarken. Diyelim ki sunumunuzdaki bir analizde kucuk bir degisiklik yapmak istiyorsunuz, artik cok kolay ve pratik bir sekilde bunu yapabilirsiniz.



## Kapanis

Daha once soyledigim gibi **knitr** bayagi flexible. Mesela LaTeX kullanmak istemiyorsaniz, **R** + **Markdown** + **Rstudio** da gayet guzel bir alternatif sizin icin. Boylece HTML ve ya Word output da elde edebilirsiniz, PDF in yaninda (ozellikle  LaTeX bilmiyorsaniz). Veyahut **R** yerine **Phyton**, **SAS**, **Ruby** kullanabilirsiniz, **Rstudio** yerine **LyX**, **Texmaker** veya **Emacs** kullanabilirsiniz. Fakat bence **Rstudio** dan sasmamak en mantiklisi cunku Rstudio knitr icin *build-in support* a sahip. Muhtemelen bunun onemli bir nedeni **knitr** in yaraticisinin bir **Rstudio** calisani olmasi. Hepsi ve daha fazlasi icin [**knitr** in websitesine bakabilirsiniz](http://yihui.name/knitr/). Son olarak, bu yazinin kendisi de **knitr** kullanarak reproducible research'e bir ornek, source code'a [buradan ulasabilirsiniz](https://raw.githubusercontent.com/gunhanb/blog/gh-pages/_source/2016-10-27-reproducible-research.Rmd).

