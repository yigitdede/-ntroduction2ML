# introduction2ML
## Regresyon Modelleri ile Veri Analizi ve Tahmini

## Giriş

Bu projede, veri seti üzerinde farklı regresyon algoritmaları kullanılarak hedef değişkenin tahmini yapılmıştır. Veri seti üzerinde öncelikle veri temizliği ve ön işleme işlemleri gerçekleştirilmiş, ardından çeşitli regresyon modelleri eğitilmiştir. Kullanılan modeller arasında Linear Regression, Ridge, Decision Tree, Random Forest ve Gradient Boosting yer almaktadır. Model performansları farklı hata metrikleri ve R² skoru ile karşılaştırılmıştır.

## Veri Seti

Bu proje kapsamında kullanılan veri seti, ABD nüfus sayımı verilerine dayanmaktadır ve çeşitli demografik özellikleri içermektedir. Veri setinde bireylere ait yaş, cinsiyet, eğitim durumu, medeni hal, meslek, ırk, gelir seviyesi gibi pek çok değişken bulunmaktadır. Amaç, bu demografik bilgiler kullanılarak belirli hedef değişkenlerin (örneğin gelir seviyesi) tahmin edilmesidir. Veri seti içerisindeki bağımsız değişkenler ve hedef değişken (y) ile modelleme süreci gerçekleştirilmiştir.

## Kullanılan Algoritmalar

- **Linear Regression:** Temel doğrusal regresyon modeli.
- **Ridge Regression:** L2 regularizasyonlu doğrusal regresyon.
- **Decision Tree Regressor:** Karar ağaçları temelli regresyon.
- **Random Forest Regressor:** Birden fazla karar ağacından oluşan ansambl yöntemi.
- **Gradient Boosting Regressor:** Ardışık öğrenme yöntemiyle model hatalarını azaltmaya çalışan ansambl yöntemi.

## Model Performans Değerlendirmesi ve Seçimi

Projede farklı regresyon modelleri kullanılarak model performansları çeşitli hata metrikleri (MSE, RMSE, MAE) ve R² skoru ile değerlendirildi. Yapılan değerlendirmeler sonucunda:

- **Random Forest** ve **Gradient Boosting** modelleri, verideki karmaşıklığı ve ilişkileri daha iyi yakalayarak en iyi sonuçları verdi.
- **Ridge** regresyon modeli makul performans sergiledi fakat ansambl yöntemlerin gerisinde kaldı.
- **Decision Tree** modelleri, ansambl modellere kıyasla daha düşük performans gösterdi.
- **Linear Regression** modeli, veri setindeki olası sorunlar ve doğrusal varsayımların sağlanmaması nedeniyle beklenmedik ve kötü sonuçlar ortaya koydu.

Bu sonuçlar, karmaşık veri yapılarında ansambl yöntemlerin doğrusal modellere kıyasla daha başarılı olduğunu göstermektedir. Bu sebeple modelleme sürecinde **Random Forest** modeli tercih edilmiş ve sonraki adımlarda bu modelin hiperparametre optimizasyonu, veri ön işleme ve özellik mühendisliği ile performansının artırılması hedeflenmiştir.

## Kullanılan Değerlendirme Metrikleri

Model doğruluğunu ölçmek için kullanılan metrikler:

- **Mean Squared Error (MSE):** Hataların karesinin ortalaması.
- **Root Mean Squared Error (RMSE):** MSE’nin karekökü, hata birimlerinin orijinal skala ile ifade edilmesini sağlar.
- **Mean Absolute Error (MAE):** Hataların mutlak değerlerinin ortalaması.
- **R² Score (Determination Coefficient):** Modelin hedef değişkenin varyansını açıklama oranı.

## Sonuç ve Gelecek Çalışmalar

Bu çalışma kapsamında, Random Forest modeli en iyi performansı gösterdiğinden sonraki aşamalarda bu model üzerine yoğunlaşılmıştır. Model performansının arttırılması için:

- Hiperparametre optimizasyonları yapılabilir (ör. GridSearchCV, RandomizedSearchCV).
- Veri ön işleme ve özellik mühendisliği teknikleri geliştirilebilir.
- Modelin genelleme yeteneği artırmak için farklı ansambl yöntemler ve derin öğrenme algoritmaları denenebilir.
- Proje ilerleyen dönemlerde bir kullanıcı arayüzü (web veya masaüstü uygulaması) ile son kullanıcıya sunulabilir.
- Veri toplama aşaması dinamikleştirilip gerçek zamanlı hale getirilebilir.

## Linkler

Projede kullanılan veri setleri ve kaynaklar:

- [Kaggle Veri Seti Linki](https://www.kaggle.com/datasets/muonneutrino/us-census-demographic-data) 

- [Proje Not Defteri (Notebook)](https://www.kaggle.com/code/yigitdede/introml-project)

---

*Bu proje,Yiğit Dede tarafından 23.05.25 tarihinde hazırlanmıştır.*
