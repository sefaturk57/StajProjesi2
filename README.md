
OpenHermes-2.5-Mistral-7B ile Fitness Sohbet Uygulaması

Bu proje, teknium/OpenHermes-2.5-Mistral-7B adlı 7 milyar parametreli büyük bir dil modelinin (LLM), 4-bit kuantizasyon tekniği kullanılarak kaynak kısıtlı ortamlarda (örneğin Google Colab) nasıl çalıştırılabileceğini ve chibbss/fitness-chat-prompt-completion-dataset veri seti üzerinde nasıl test edilebileceğini gösteren bir uygulamadır.



<img width="468" height="333" alt="image" src="https://github.com/user-attachments/assets/7f3c3c2d-86ac-4eb2-964b-31492502f871" />
<img width="461" height="336" alt="image" src="https://github.com/user-attachments/assets/a5551a4a-cd33-44c1-a58b-1e30152543a2" />


Proje Özeti
Bu proje, açık kaynaklı büyük dil modellerinin pratik uygulamalarını keşfetmeyi ve bu modellerin optimizasyon teknikleriyle daha erişilebilir hale getirilmesini amaçlamaktadır. Özellikle, 4-bit kuantizasyonun, büyük modellerin bellek ayak izini önemli ölçüde azaltarak daha yaygın donanımlarda çalışabilmesine olan etkisi incelenmiştir. Proje kapsamında, fitness alanında sohbet yeteneğine sahip bir LLM test edilmiş ve performans metrikleri elde edilmiştir.

Kullanılan Teknolojiler
Model: teknium/OpenHermes-2.5-Mistral-7B (Hugging Face Hub)

Veri Seti: chibbss/fitness-chat-prompt-completion-dataset (Hugging Face Hub)

Kütüphaneler:

transformers (Hugging Face)

datasets (Hugging Face)

accelerate (Hugging Face)

bitsandbytes (Hugging Face)

torch (PyTorch)

Ortam: Google Colaboratory

Kurulum
Bu projeyi çalıştırmak için aşağıdaki adımları izleyin:

Google Colab'ı Ziyaret Edin: https://colab.research.google.com/

Not Defterini Açın: Eğer kodunuzu bir Colab not defterinde geliştirdiyseniz, bu not defterini açın. Eğer henüz yüklemediyseniz, yukarıdaki []( [BURAYA COLAB NOT DEFTERİNİN LİNKİNİ EKLEYİN] ) bağlantısını kullanarak doğrudan Colab'da açabilirsiniz.

Çalışma Zamanı Ayarları: Menüden Çalışma zamanı -> Çalışma zamanı türünü değiştir seçeneğine gidin ve Donanım hızlandırıcı olarak GPU'yu seçin. Kaydedin.

Gerekli Kütüphaneleri Yükleyin: Not defterinin ilk hücresine aşağıdaki kodu ekleyin ve çalıştırın:

```python
!pip install transformers datasets accelerate bitsandbytes torch
```

Modeli ve Veri Setini Yükleyin: Not defterindeki ilgili kod hücrelerini çalıştırarak modeli ve veri setini yükleyin.

Kullanım
Not defterini açıp kurulum adımlarını tamamladıktan sonra, not defterindeki kod hücrelerini sırayla çalıştırarak:

Fitness veri setinden örnek istemleri (prompt) yükleyebilirsiniz.

OpenHermes-2.5-Mistral-7B modelini 4-bit kuantizasyonu ile yükleyebilir ve çalıştırabilirsiniz.

Modeli örnek istemlerle test edebilir ve çıktılarını gözlemleyebilirsiniz.

Test sonuçlarını (üretilen cevaplar ve performans metrikleri, eğer hesaplandıysa) görüntüleyebilirsiniz.

Not defterindeki kod, modelin metin üretme yeteneklerini farklı parametrelerle (örneğin temperature, max_new_tokens) nasıl etkilediğini anlamanıza yardımcı olacak şekilde düzenlenmiştir.

Sonuçlar
Proje sonucunda, OpenHermes-2.5-Mistral-7B modelinin 4-bit kuantizasyonu ile Google Colab gibi sınırlı kaynaklara sahip ortamlarda bile başarılı bir şekilde çalıştırılabildiği gösterilmiştir. Modelin, fitness
odaklı sohbet veri seti üzerindeki testlerinde anlamlı ve bağlama uygun cevaplar üretebildiği gözlemlenmiştir. Elde edilen BLEU ve ROUGE gibi metrikler (eğer hesaplandıysa buraya ekleyin) modelin performansını nicel olarak değerlendirmeye olanak sağlamıştır.


<img width="929" height="453" alt="image" src="https://github.com/user-attachments/assets/44708972-7104-41a8-975f-cb2598a4da5d" />
<img width="650" height="134" alt="image" src="https://github.com/user-attachments/assets/4f6f8089-0510-49e3-a805-2c5b2b539f5f" />






Katkıda Bulunma
Bu proje kişisel bir çalışma olup şu anda dış katkılara açık değildir. Ancak, modelin farklı veri setleri üzerinde denenmesi, farklı optimizasyon tekniklerinin uygulanması veya performans analizlerinin derinleştirilmesi gibi fikirleriniz varsa benimle iletişime geçebilirsiniz.
