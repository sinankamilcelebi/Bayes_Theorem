<a href="https://colab.research.google.com/github/sinankamilcelebi/Bayes_Theorem/blob/master/Bayes_Theorem.ipynb">
<img src="https://colab.research.google.com/assets/colab-badge.svg" width="150" height="50" alt="Open In Colab" title = "Bayes Theorem" align="center"/>
</a>

# Bayes Theorem

* @file     : Bayes_Theorem.ipynb
* @author   : Sinan KAMILCELEBI
* @version  : V1.0.0
* @date     : 11-April-2019
* @brief    : Thomas Bayes Theorem Example.

## __Örnek Soru:__   
Bir mühendis geliştirdiği bir sistem ile ürünleri test etmektedir. Bu sistem %99 oranında başarı ile bozuk ürünleri belirlemektedir. Bununla birlikte yapılan test işlemi %1 ihtimalle sağlam olan ürüne de bozuk demektedir. Tüm ürünlerin %X'i bozuk ise test sonucunda bozuk çıkan bir ürünün gerçekten bozuk olma olasılığı nedir? 

## __Çözüm:__  
A = Test edilen ürünün bozuk olma olasılığı.  
B = Sonucun pozitif (bozuk) olma olasılığı.  
X = Tüm ürünlerin bozuk yüzde değeri.

P(A|B) = (P(B|A) * P(A)) / (((P(B|A) * P(A)) + (P(A|B) * P(B)))

P(A|B) = ((0.99) * (X / 100)) / (((0.99) * (X / 100)) + ((0.01) * (1 - (X / 100))))

## __Açıklamalar:__   
Yukarıdaki soruda bizden istenildiği üzere, sonucun bozuk olma olasılığı gerçekleştiğinde test edilen ürünün de bozuk olma olasılığını hesaplayacağız. (P(A|B))  

İlk önce yukarıdaki formülde belirtildiği gibi pay kısmında test edilen ürünün bozuk olma olasılığı gerçekleştiğinde sonucun bozuk olma olasığı (0.99) ile test edilen ürünün bozuk olma olasılığını (X / 100) çarpıyoruz (P(B|A) * P(A)). 

Daha sonra ise payda kısmında tüm durum için yani hem test edilen ürünün bozuk olma olasılığı gerçekleştiğinde sonucun bozuk olma olasılığını (P(B|A) * P(A)) hem de test işleminin sonucu bozuk olduğunda test edilen ürünün bozuk olma olasılığını (P(A|B) * P(B)) hesaplıyoruz.   

Son olarak da pay ve payda da elde ettiğimiz sonuçlarını birbirine oranladığımızda soruda bizden istenilen olasılık değerini elde etmiş oluyoruz. 
