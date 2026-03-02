# Breast_Cancer_Classification

🚀 Kullanılan Teknolojiler

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-Learn

🤖 Kullanılan Algoritma
Logistic Regression

Bu projede Logistic Regression algoritması tercih edilmiştir.

Neden Logistic Regression?

Problem ikili sınıflandırma problemidir.

Tıbbi veri setlerinde yorumlanabilirlik önemlidir.

Küçük ve orta ölçekli veri setlerinde hızlı ve etkilidir.

Aşırı karmaşık olmadığı için overfitting riski düşüktür.

Lineer ayrılabilir veri setlerinde yüksek performans gösterir.

🔄 Proje Adımları
1️⃣ Veri Ön İşleme (Data Preprocessing)

Gereksiz sütunlar kaldırıldı (id, Unnamed: 32)

Hedef değişken sayısallaştırıldı:

M → 1

B → 0

Veri eğitim ve test olarak ayrıldı (%80 - %20)

2️⃣ Feature Scaling

StandardScaler kullanılarak veriler ölçeklendirildi.

Neden?

Logistic Regression mesafe/katsayı temelli çalışır.

Farklı ölçeklerdeki değişkenlerin modeli etkilememesi için standartlaştırma yapılmıştır.

3️⃣ Model Eğitimi
from sklearn.linear_model import LogisticRegression

model = LogisticRegression()
model.fit(X_train, y_train)
4️⃣ Tahmin
y_pred = model.predict(X_test)
📊 Model Değerlendirme Metrikleri

Model aşağıdaki metriklerle değerlendirilmiştir:

Confusion Matrix

Accuracy

Precision

Recall

F1-Score

🔎 Önemli Nokta (Tıbbi Uygulama)

Tıbbi problemlerde özellikle Recall (Sensitivity) çok önemlidir.

Çünkü:

False Negative (Kanserli hastayı kaçırma) ciddi sonuçlara yol açabilir.

Bu nedenle model performansı sadece Accuracy ile değil Recall ile de değerlendirilmiştir.

📈 Sonuç

Model yüksek doğruluk oranı elde etmiştir.

Precision ve Recall değerleri dengelidir.

F1-Score değeri modelin genel performansının güçlü olduğunu göstermektedir.

Logistic Regression bu veri seti için uygun ve etkili bir seçim olmuştur.

📂 Proje Yapısı
Meme_Kanseri_Teshis.ipynb
README.md
meme_kanseri.csv
