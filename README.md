# aygaz_machine_learning_project
# IMDb Film Yorumları ve Sentiment Analizi Projesi (Projem Master branch içerisinde.)
kaggle linkim=https://www.kaggle.com/code/azizalperengrm/aygaz-machine-learning-project
## Proje Hakkında
Bu proje, IMDb'den alınan 50.000 film eleştirisi ve bu eleştirilerin duygu (sentiment) etiketlerini kullanarak makine öğrenmesi algoritmalarını test etmeyi amaçlamaktadır. Projede iki farklı öğrenme türü olan denetimli (supervised) ve denetimsiz (unsupervised) öğrenme algoritmaları aynı veri seti üzerinde çalıştırılmıştır. Bu sayede, veri setinin her iki yöntem açısından nasıl performans gösterdiği incelenmiştir.

## Kullanılan Algoritmalar
1. **Denetimli Öğrenme (Supervised Learning):**
   - Bu yöntemde, veri seti üzerinde etiketlenmiş (duygu etiketleri) veriler kullanılarak algoritmalar eğitilmiştir. Özellikle Logistic Regression, Random Forest ve Support Vector Machines (SVM) gibi algoritmalar kullanılarak sentiment tahminleri yapılmıştır.
   
2. **Denetimsiz Öğrenme (Unsupervised Learning):**
   - Bu yöntemde ise veri seti üzerinde herhangi bir etiket olmadan kümelenme (clustering) algoritmaları çalıştırılmıştır. Projede özellikle KMeans algoritması kullanılarak yorumlar kümelemiştir.

## Sonuçlar
- **Denetimli Öğrenme Sonuçları:** 
  Denetimli öğrenme algoritmaları, etiketli veri setini kullanarak oldukça başarılı sonuçlar vermiştir. Özellikle sentiment (olumlu/olumsuz) tahmini için kullanılan Logistic Regression ve SVM algoritmaları, yüksek doğruluk oranları elde etmiştir. Veri setindeki etiketlerin varlığı, bu yöntemlerin başarı oranını artırmıştır çünkü denetimli öğrenme, verilerin geçmiş bilgilerine dayalı olarak model öğrenmesine olanak tanır.
  
- **Denetimsiz Öğrenme Sonuçları:**
  KMeans gibi denetimsiz öğrenme algoritmaları ise etiketlerin olmadığı bir senaryoda verileri kümeler halinde gruplamaya çalışmıştır. Bu yöntem, yorumların benzerliğine dayalı olarak kümeler oluşturduğundan, sentiment sınıflandırma kadar başarılı sonuçlar vermemiştir. Özellikle veri setindeki karmaşık metin yapıları ve anlamsal farklılıklar, kümelenme işlemlerinde bazı yanlış gruplamalara yol açmıştır. Ancak, KMeans yine de veri seti içindeki temel yapıları anlamada faydalı olmuştur.

## Değerlendirme
Veri seti, denetimli öğrenme algoritmaları için daha uygun görünmektedir. Bunun temel nedeni, veri setinde etiketli (olumlu/olumsuz) duygu bilgileri bulunmasıdır. Bu tür problemler, denetimli öğrenme algoritmalarının iyi performans göstermesi için idealdir çünkü algoritmalar geçmiş verilere dayanarak tahmin yapma yeteneğine sahiptir.

Denetimsiz öğrenme ise etiketlerin olmadığı veri setleri için daha uygundur, ancak bu projede kullanılan IMDb veri seti etiketli olduğundan, denetimsiz öğrenme algoritmaları beklenen performansı gösterememiştir. KMeans algoritması, benzer yorumları bir araya getirme konusunda temel kümeler oluşturmuş olsa da, sentiment analizi gibi net sınıflandırma gerektiren problemler için yeterince etkili olmamıştır.

## Sonuç Olarak
Bu projede elde edilen sonuçlar, etiketli veri setleri kullanıldığında denetimli öğrenme algoritmalarının daha etkili olduğunu göstermektedir. Bununla birlikte, denetimsiz öğrenme algoritmaları da veri keşfi ve kümeleme için faydalı olabilir, ancak sentiment analizi gibi spesifik sınıflandırma problemleri için ideal değildir.
