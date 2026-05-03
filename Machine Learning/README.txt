# Boston Housing Regression Models

## 📌 Proje Hakkında
Bu proje, **Boston Housing** veri seti üzerinde farklı regresyon algoritmalarının performanslarını karşılaştırmak amacıyla hazırlanmıştır. Kullanılan algoritmalar:
- DecisionTreeRegressor
- Support Vector Regression (SVR)
- K-Nearest Neighbors (KNN)

Ek olarak:
- **GridSearchCV** ile hiperparametre optimizasyonu yapılmıştır.
- Sonuçlar **matplotlib** ve **seaborn** ile görselleştirilmiştir.

---

## ⚙️ Kullanılan Adımlar
1. **Veri Hazırlığı**
   - Boston Housing veri seti yükleme
   - Eksik değer kontrolü
   - Train-Test Split

2. **Modeller**
   - DecisionTreeRegressor (default parametreler)
   - DecisionTreeRegressor (GridSearchCV ile optimize edilmiş parametreler)
   - SVR
   - KNN Regressor

3. **Hyperparameter Tuning**
   - GridSearchCV ile parametre arama
   - En iyi parametrelerin seçilmesi

4. **Karşılaştırma**
   - R², MAE, MSE skorları
   - Grafiksel karşılaştırmalar (bar chart, scatter plot)

---

## 📊 Sonuçlar

### DecisionTreeRegressor Karşılaştırması
| Model                          | R² Skoru | MAE   | MSE   |
|--------------------------------|----------|-------|-------|
| DecisionTreeRegressor (Default)| 0.55     | 3.16  | 31.5  |
| DecisionTreeRegressor (GridSearchCV)| 0.67| 3.22  | 24.7  |

### Diğer Algoritmalar
| Algoritma               | R² Skoru | MAE   | MSE  |
|-------------------------|----------|-------|------|
| SVR (GridSearchCV)      | 0.65     | 2.95  | 26.3 |
| KNN (GridSearchCV)      | 0.75     | 2.77  | 18.8 |

