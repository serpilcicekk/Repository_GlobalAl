# Repository_GlobalAl

Proje Özeti
Bu proje, derin öğrenme tekniklerini kullanarak görüntü sınıflandırma üzerine odaklanmaktadır. Amacımız, belirli bir veri setindeki nesneleri etkili bir şekilde tanımlamak ve sınıflandırmaktır. Proje, 13500 eğitim örneği ve 4500 test örneği içeren bir veri seti kullanılarak gerçekleştirilmiştir. Modelimiz, VGG16 mimarisini temel alan bir transfer öğrenme yaklaşımı ile inşa edilmiştir. Eğitim sürecinde veri augmentasyonu ve dropout teknikleri kullanılarak modelin genel performansı artırılmıştır. Hiperparametre optimizasyonu ile en iyi sonuçlar elde edilmeye çalışılmıştır.

Model Performansının Değerlendirilmesi
Eğitim ve Doğrulama Metrikleri:

Eğitim Doğruluğu: %36.60 (son epoch'taki değer)
Doğrulama Doğruluğu: %49.78 (son epoch'taki değer)
Test Doğruluğu: %81.46
Confusion Matrix:
[[121   0   1   0  53   0   0   0   0   0  21   0   0   0  13   0  14   0]
 [  0  32   0   0   0  50   0  57   0   0   0   4   0  71   0  58   0   0]
 [  4   0  87   0   5   0  11   0 141   0   1   0   0   0   0   0   5   0]
 [  0   0   0 205   0   4   0   1   0  19   0  11   0   0   0   0   0   8]
 [  6   0   0   0 176   0   0   0  22   0   0   0  13   0   1   0  21   0]
 [  0   9   0   2   0 157   0  20   0   1   0  12   0  12   0  29   0  10]
 [  0   0   0   0   9   0 196   0  29   0   0   0  20   0   1   0   2   0]
 [  0  10   0   1   0  27   0 144   0   0   0   3   0  48   0  22   0   0]
 [  0   0  10   0   7   0   3   0 213   0   0   0   6   0   2   0   9   1]
 [  0   0   0  79   0   1   0   3   0 129   0   8   0   0   0   1   0   9]
 [ 22   0  55   0   0   0   3   0  69   0  64   0   2   0  14   0  39   0]
 [  0   2   0   9   0  33   0  21   0   3   0 153   0   4   0  14   0   9]
 [  0   0   0   0  70   0   5   0   1   0   1   0 159   0   7   0   0   0]
 [  0   7   0   0   0   3   0  34   0   0   0   1   0 163   0  30   0   0]
 [  3   0   9   0  78   0   2   0  65   0   5   0  14   0  40   0  36   0]
 [  0  11   0   0   0  26   0  48   0   0   0   6   0  70   0 104   0   0]
 [ 11   0  80   0  21   0   0   0 110   0   1   0   0   0   0   0  27   0]
 [  1   0   0 101   0  19   0   0   0  28   0  29   0   0   0   7   0  70]]

Classification Report:
              precision    recall  f1-score   support

           0       0.72      0.54      0.62       223
           1       0.45      0.12      0.19       272
           2       0.36      0.34      0.35       254
           3       0.52      0.83      0.64       248
           4       0.42      0.74      0.53       239
           5       0.49      0.62      0.55       252
           6       0.89      0.76      0.82       257
           7       0.44      0.56      0.49       255
           8       0.33      0.85      0.47       251
           9       0.72      0.56      0.63       230
          10       0.69      0.24      0.35       268
          11       0.67      0.62      0.64       248
          12       0.74      0.65      0.70       243
          13       0.44      0.68      0.54       238
          14       0.51      0.16      0.24       252
          15       0.39      0.39      0.39       265
          16       0.18      0.11      0.13       250
          17       0.65      0.27      0.39       255

    accuracy                           0.50      4500
   macro avg       0.53      0.50      0.48      4500
weighted avg       0.53      0.50      0.48      4500

