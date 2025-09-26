# Brain MRI Tumor Classification

Bu repo, beyin MR görüntülerinden tümör sınıflandırması yapmak için VGG16 tabanlı bir derin öğrenme modelini içermektedir. Veri artırma (rotation, flip, noise) teknikleri uygulanmış, eğitim süreci sırasında train/validation accuracy takip edilmiş ve Grad-CAM ile görselleştirme yapılmıştır.

# Giriş

Projede **Brain Tumor MRI Dataset** (glioma, meningioma, pituitary, no_tumor sınıfları) kullanılmıştır.  
Amaç, MRI görüntülerinden otomatik olarak tümör tipini sınıflandıran bir model geliştirmektir.  

Model mimarisi olarak **VGG16 (ImageNet ön-eğitimli)** kullanılmış ve son katman 4 sınıfa uyarlanmıştır.  
Ayrıca, veri artırma yöntemleriyle sınıf dengesizliği azaltılmıştır.  

# Metrikler

- Eğitim süresince train/validation loss ve accuracy takip edilmiştir.  
- Test setinde **accuracy, confusion matrix** ve **classification report** hesaplanmıştır.  
- Grad-CAM yöntemi ile modelin odaklandığı bölgeler görselleştirilmiştir.  

# Ekler

- Grad-CAM ile örnek MRI görüntülerinde hangi bölgelerin model kararını etkilediği analiz edilmiştir.  

# Sonuç ve Gelecek Çalışmalar

Elde edilen sonuçlar, VGG16’nın MRI sınıflandırmasında yüksek doğruluk oranı sağlayabildiğini göstermektedir.  
Gelecekte, daha hafif ve hızlı mimariler (ResNet, MobileNet) ile deneyler yapılabilir ve model gerçek zamanlı sistemlere entegre edilebilir. Ayrıca, farklı MRI datasetleri eklenerek genellenebilirlik artırılabilir.  

# Linkler

Proje ile ilgili Kaggle notebook: 
https://www.kaggle.com/code/azrahazan/brain-mri-classification-akbank-bootcamp-2025

Dataset: 
https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset

