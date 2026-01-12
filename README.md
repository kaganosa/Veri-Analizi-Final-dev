Veri Analizi Dönem Projesi: Kredi Onay Tahmini (Loan Prediction)

Projenin temel amacı, müşterilerin demografik ve finansal bilgilerini kullanarak kredi başvurularının onaylanıp onaylanmayacağını tahmin eden bir **Makine Öğrenmesi (Sınıflandırma) modeli geliştirmektir.

 Proje Hakkında

Bankalar için kredi onay süreci, risk yönetimi açısından kritiktir. Bu projede, tarihsel kredi verileri analiz edilmiş ve "Kredi Verilmeli mi?" sorusuna otomatik yanıt veren bir karar destek sistemi oluşturulmuştur.

* *Problem Tipi:* Sınıflandırma (Binary Classification)
* *Kullanılan Algoritma:* Lojistik Regresyon (Logistic Regression)
* *Başarı Oranı (Accuracy):* %79.73

 Veri Seti Özellikleri

Projede kullanılan veri seti, müşterilere ait aşağıdaki özellikleri içermektedir:

| Özellik | Açıklama |
| :--- | :--- |
| *Gender* | Cinsiyet (Male/Female) |
| *Married* | Medeni Hal (Yes/No) |
| *Dependents* | Bakmakla yükümlü olunan kişi sayısı |
| *Education* | Eğitim Durumu (Graduate/Not Graduate) |
| *Self_Employed* | Serbest Meslek Sahibi mi? (Yes/No) |
| *ApplicantIncome* | Başvuru sahibinin geliri |
| *LoanAmount* | Talep edilen kredi miktarı |
| *Credit_History* | Kredi Geçmişi (1.0: İyi, 0.0: Kötü) - En belirleyici özellik |
| *Property_Area* | Mülk/Yaşam Alanı (Urban/Semiurban/Rural) |
| *Loan_Status* | *Hedef Değişken* (Y: Onay, N: Red) |

 Uygulanan Yöntemler

Proje sürecinde aşağıdaki veri bilimi adımları izlenmiştir:

1.  *Veri Keşfi (EDA):* Veri setinin yapısal analizi yapılmış, eksik veriler tespit edilmiştir.
2.  *Veri Ön İşleme (Preprocessing):*
    * Eksik veriler (Null values), sayısal sütunlarda ortalama (mean), kategorik sütunlarda mod (mode) yöntemiyle doldurulmuştur.
    * Kategorik veriler Label Encoding yöntemi ile sayısal değerlere dönüştürülmüştür.
3.  *Model Kurulumu:* Sınıflandırma problemi için endüstri standardı olan *Logistic Regression* algoritması seçilmiştir.
4.  *Değerlendirme:* Modelin başarısı %20'lik test veri seti üzerinde ölçülmüştür.

 Sonuçlar

Modelin test verisi üzerindeki performansı:

* *Accuracy:* %79.73
* *F1-Score:* Modelin özellikle kredisi onaylanacak kişileri (Positive class) tespit etmede yüksek başarı gösterdiği gözlemlenmiştir.

> *Önemli Bulgu:* Analizler sonucunda kredi onayını etkileyen en kritik faktörün *Kredi Geçmişi (Credit History)* olduğu görülmüştür.

----- Hazırlayanlar ----
TAHA KAĞAN AŞĞA 23430070020
AHMET AKA 23430070040
