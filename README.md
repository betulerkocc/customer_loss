# customer_loss
Müşteri kaybını tahmin eden makine öğrenmesi projesi.

Bu proje, bir telekomünikasyon şirketinin müşteri verilerini analiz ederek hangi müşterilerin aboneliğini iptal etme (churn) eğiliminde olduğunu tahmin eden bir makine öğrenmesi modeli geliştirmeyi amaçlar.

## Proje Özeti
- **Veri Seti:** Kaggle Telco Customer Churn (7043 satır)
- **Model:** Random Forest Classifier
- **Başarı Oranı:** %78.89 Accuracy

## Uygulanan Adımlar
- **Veri Temizleme:** `TotalCharges` sütunundaki hatalı formatları sayısal tipe dönüştürdüm ve boş değerleri temizledim.
- **Encoding:** Kategorik değişkenleri (Gender, Contract vb.) `pd.get_dummies` ile makine öğrenmesine uygun sayısal formata getirdim.
- **Modelleme:** Veriyi %80 eğitim ve %20 test olarak ayırarak Random Forest algoritması ile eğittim.

## Önemli Bulgular
Yapılan analiz sonucunda; aylık sözleşme (month-to-month) tipine sahip olan ve aylık ödemesi yüksek olan müşterilerin ayrılma riskinin daha yüksek olduğu gözlemlenmiştir.
