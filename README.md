English [EN]
# Meta-Heuristic Feature Selection and Machine Learning Optimization for SONAR Signal Classification

## Abstract

This study examines the performance of meta-heuristic feature selection methods in the SONAR signal classification problem within an academic framework. The impact of feature selection on classification performance in high-dimensional datasets was evaluated using Ant Colony Optimization (ACO), Genetic Algorithm (GA), and Particle Swarm Optimization (PSO) methods. Experiments were conducted on an open-access SONAR dataset, and the study is for research and educational purposes only.

## Objective

The objective of this study is to reduce the features in the 60-dimensional SONAR dataset using meta-heuristic optimization algorithms and to analyze the mine–rock classification performance based on the selected feature subsets. In this context, the results obtained with the ACO, GA, and PSO algorithms were comparatively analyzed.

## Methodology

Three meta-heuristic optimization algorithms were employed for feature selection:

- **Ant Colony Optimization (ACO)**: Utilizes pheromone-based mechanism for well-balanced feature selection
- **Genetic Algorithm (GA)**: Employs crossover and mutation operations to maintain population diversity
- **Particle Swarm Optimization (PSO)**: Leverages swarm intelligence for rapid convergence

Selected features were evaluated using multiple machine learning classifiers including Random Forest, Support Vector Machine, and K-Nearest Neighbors.

## Key Findings

### 1. Classification Performance
- Model performance improved despite significant feature reduction
- In several cases, optimized feature subsets achieved superior results compared to the baseline (using all features)
- Best overall performance: **92.86% accuracy** with GA + Random Forest combination

### 2. Feature Reduction
- **ACO**: Reduced to 16 features (73.3% reduction) with 87.3% average accuracy
- **GA**: Reduced to 21 features (65.0% reduction) with best single-model performance
- **PSO**: Reduced to 30 features (50.0% reduction)
- Average feature reduction across all methods: **~63%**

### 3. Computational Efficiency
- Training times significantly reduced due to lower dimensionality
- Faster prediction times with optimized feature subsets
- Reduced model complexity without sacrificing accuracy

### 4. Algorithm Comparison
- **ACO**: Achieved highest feature reduction rate (73.3%) and best average accuracy (87.3%)
- **GA**: Produced best single-model performance (92.86% accuracy, 91.43% F1-Score with Random Forest)
- **PSO**: Demonstrated fast convergence characteristics with competitive results

## Results Summary

| Algorithm | Features Selected | Reduction Rate | Best Accuracy | Best Model |
|-----------|------------------|----------------|---------------|------------|
| ACO       | 16/60            | 73.3%          | 87.3% (avg)   | Various    |
| GA        | 21/60            | 65.0%          | 77.78% (avg)       | Random Forest |
| PSO       | 30/60            | 50.0%          | 76.98% (avg)            | Various    |

## Conclusion

This study demonstrates that meta-heuristic optimization algorithms can be effectively employed for feature selection in sonar signal classification tasks. The findings indicate that:

1. Intelligent feature selection improves both classification accuracy and model interpretability
2. Significant dimensionality reduction (up to 73.3%) can be achieved without performance degradation
3. The GA + Random Forest combination (92.86% accuracy with 65% feature reduction) shows particular promise for practical applications in naval defense systems
4. Meta-heuristic approaches offer a viable alternative to traditional feature selection methods in high-dimensional classification problems

## Dataset Configuration

To run this notebook locally or on Google Colab:
1. Upload the `sonar_data.csv` file to the `content` directory
2. Alternatively, update the file path in the **Dataset Loading and Exploratory Data Analysis** section

## Access Links

- **Dataset Source**: [Kaggle - SONAR Rock vs Mine Prediction](https://www.kaggle.com/code/shamkumar1307/sonar-rock-vs-mine-prediction)
- **Google Colab Notebook**: [Access Notebook](https://colab.research.google.com/drive/1azOs39m6OWtPX3pDxYO8jpTv0jh5kA4d?usp=sharing)

## Ethical and Academic Disclosure

- This study was prepared solely for academic and educational purposes
- All experiments were conducted using open-access (public) datasets
- This study does not represent any real-world, operational, or deployed system
- Results are intended for research and educational use only

## Contact Information

- **GitHub**: [MelihCan1115](https://github.com/MelihCan1115)
- **LinkedIn**: [Melih Can KÖK](https://www.linkedin.com/in/melih-can-k%C3%B6k-249a9b29b/)
- **Email**: mcan.kok.1115@gmail.com

## Keywords

Feature Selection, Meta-Heuristic Optimization, Ant Colony Optimization, Genetic Algorithm, Particle Swarm Optimization, SONAR Classification, Machine Learning, Dimensionality Reduction

*This research is open-source and available for academic use and collaboration.*

---
Türkçe [TR]
# SONAR Sinyal Sınıflandırması için Meta-Heuristik Özellik Seçimi ve Makine Öğrenimi Optimizasyonu

## Özet

Bu çalışma, akademik bir çerçeve içinde SONAR sinyal sınıflandırma probleminde meta-heuristik özellik seçimi yöntemlerinin performansını incelemektedir. Yüksek boyutlu veri kümelerinde özellik seçiminin sınıflandırma performansı üzerindeki etkisi, Karınca Kolonisi Optimizasyonu (ACO), Genetik Algoritma (GA) ve Parçacık Sürüsü Optimizasyonu (PSO) yöntemleri kullanılarak değerlendirilmiştir. Deneyler, açık erişimli bir SONAR veri seti üzerinde gerçekleştirilmiştir ve bu çalışma yalnızca araştırma ve eğitim amaçlıdır.

## Amaç

Bu çalışmanın amacı, meta-heuristik optimizasyon algoritmaları kullanarak 60 boyutlu SONAR veri setindeki özellikleri azaltmak ve seçilen özellik alt kümelerine dayalı olarak maden-kaya sınıflandırma performansını analiz etmektir. Bu bağlamda, ACO, GA ve PSO algoritmaları ile elde edilen sonuçlar karşılaştırmalı olarak analiz edilmiştir.
## Metodoloji

Özellik seçimi için üç meta-sezgisel optimizasyon algoritması kullanıldı:

- **Karınca Kolonisi Optimizasyonu (ACO)**: Dengeli özellik seçimi için feromon tabanlı mekanizmayı kullanır
- **Genetik Algoritma (GA)**: Popülasyon çeşitliliğini korumak için çaprazlama ve mutasyon işlemlerini kullanır
- **Parçacık Sürüsü Optimizasyonu (PSO)**: Hızlı yakınsama için sürü zekasını kullanır

Seçilen özellikler, Rastgele Orman, Destek Vektör Makinesi ve K-En Yakın Komşular dahil olmak üzere çoklu makine öğrenimi sınıflandırıcıları kullanılarak değerlendirildi.

## Önemli Bulgular

### 1. Sınıflandırma Performansı
- Önemli özellik azaltımına rağmen model performansı iyileşti
- Birkaç durumda, optimize edilmiş özellik alt kümeleri, temel modele (tüm özellikleri kullanarak) kıyasla üstün sonuçlar elde etti
- En iyi genel performans: GA + Random Forest kombinasyonu ile **%92,86 doğruluk**

### 2. Özellik Azaltımı
- **ACO**: 87,3% ortalama doğrulukla 16 özelliğe indirgenmiştir (73,3% azalma)
- **GA**: En iyi tek model performansı ile 21 özelliğe indirgenmiştir (65,0% azalma)
- **PSO**: 30 özelliğe indirgenmiştir (50,0% azalma)
- Tüm yöntemlerde ortalama özellik azaltma: **~%63**

### 3. Hesaplama Verimliliği
- Boyutların azalmasıyla eğitim süreleri önemli ölçüde azaldı
- Optimize edilmiş özellik alt kümeleriyle daha hızlı tahmin süreleri
- Doğruluktan ödün vermeden model karmaşıklığı azaltıldı

### 4. Algoritma Karşılaştırması
- **ACO**: En yüksek özellik azaltma oranı (%73,3) ve en iyi ortalama doğruluk (%87,3) elde edildi
- **GA**: En iyi tek model performansı elde edildi (doğruluk %92,86, Random Forest ile F1-Score %91,43)
- **PSO**: Rekabetçi sonuçlarla hızlı yakınsama özellikleri gösterdi

## Sonuç Özeti

| Algoritma | Seçilen Özelliklerin Sayısı | Azaltma Oranı | En İyi Doğruluk | En İyi Model |
|-----------|------------------|----------------|---------------|------------|
| ACO       | 16/60            | 73.3%          | 87.3% (ort)   | Çeşitli    |
| GA        | 21/60            | 65.0%          | 77.78% (ort)       | Random Forest |
| PSO       | 30/60            | 50.0%          | 76.98% (ort)            | Çeşitli    |

## Sonuç

Bu çalışma, meta-sezgisel optimizasyon algoritmalarının sonar sinyali sınıflandırma görevlerinde özellik seçimi için etkili bir şekilde kullanılabileceğini göstermektedir. Bulgular şunu göstermektedir:

1. Akıllı özellik seçimi, hem sınıflandırma doğruluğunu hem de model yorumlanabilirliğini iyileştirir.
2. Performans düşüşü olmadan önemli ölçüde boyut azaltma (73,3'e kadar) sağlanabilir.
3. GA + Rastgele Orman kombinasyonu (65 özellik azaltma ile %92,86 doğruluk), deniz savunma sistemlerinde pratik uygulamalar için özellikle umut vericidir.
4. Meta-sezgisel yaklaşımlar, yüksek boyutlu sınıflandırma problemlerinde geleneksel özellik seçimi yöntemlerine uygun bir alternatif sunar.

## Veri Kümesi Yapılandırması

Bu not defterini yerel olarak veya Google Colab'da çalıştırmak için:
1. `sonar_data.csv` dosyasını `content` dizinine yükleyin.
2. Alternatif olarak, **Veri Kümesi Yükleme ve Keşifsel Veri Analizi** bölümündeki dosya yolunu güncelleyin.

## Erişim Bağlantıları

- **Veri Kümesi Kaynağı**: [Kaggle - SONAR Kaya ve Maden Tahmini](https://www.kaggle.com/code/shamkumar1307/sonar-rock-vs-mine-prediction)
- **Google Colab Not Defteri**: [Not Defterine Erişin](https://colab.research.google.com/drive/1azOs39m6OWtPX3pDxYO8jpTv0jh5kA4d?usp=sharing)

## Etik ve Akademik Açıklama

- Bu çalışma yalnızca akademik ve eğitim amaçlı hazırlanmıştır.
- Tüm deneyler açık erişimli (halka açık) veri kümeleri kullanılarak gerçekleştirilmiştir.
- Bu çalışma gerçek dünyadaki, operasyonel veya kullanıma sunulan herhangi bir sistemi temsil etmemektedir.
- Sonuçlar yalnızca araştırma ve eğitim amaçlıdır.

## İletişim Bilgileri

- **GitHub**: [MelihCan1115](https://github.com/MelihCan1115)
- **LinkedIn**: [Melih Can KÖK](https://www.linkedin.com/in/melih-can-k%C3%B6k-249a9b29b/)
- **E-posta**: mcan.kok.1115@gmail.com

## Anahtar Kelimeler

Özellik Seçimi, Meta-Sezgisel Optimizasyon, Karınca Kolonisi Optimizasyonu, Genetik Algoritma, Parçacık Sürüsü Optimizasyonu, SONAR Sınıflandırması, Makine Öğrenimi, Boyutsallık Azaltma

---

*Bu araştırma açık kaynaklıdır ve akademik kullanım ve işbirliği için mevcuttur.*
