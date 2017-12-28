# Tensorflow Tutorials

Bu repository Türkçe Tensorflow eğitimlerini içermektedir. Bu eğitimler temel olarak Tensorflow [resmi tutorialları](https://www.tensorflow.org/tutorials/), Aurelien Geron'un scikit-learn ve tensorflow [kitabı](https://www.amazon.com/Hands-Machine-Learning-Scikit-Learn-TensorFlow/dp/1491962291/ref=sr_1_3?ie=UTF8&qid=1514449071&sr=8-3&keywords=tensorflow) ve Hvass'ın tutorial [serisinden](https://github.com/Hvass-Labs/TensorFlow-Tutorials) esinlenilmiştir. 

Bu repository'deki kodlar en basitten başlayarak kompleks modellere gidecek şekilde hedeflenmiştir. Eklememi istediğiniz başka konular olursa lütfen bana [e-mail](aelvanaydemir@gmail.com), [twitter](https://twitter.com/L1_norn) veya [linkedin](https://www.linkedin.com/in/aelvangunduz/) yoluyla ulaşın.

Tutorialları kaynak göstermek koşuluyla, serbestçe kullanabilirsiniz.

## Kurulum

Tutorialları çalıştırabilmek için Python 3 ile Tensorflow, Numpy, Scikit-learn, Pillow (PIL), Scikit-Image, pandas gibi paketlere ihtiyacınız olacak. Tensorflow'u kullanmanın en kullanıcı dostu şekli [Anaconda](https://www.anaconda.com/download/#macos) Python 3'ü edinip, sanal ortamda çalışmanızdır. Kendi işletim sisteminiz için Anaconda Python 3'ü edindikten sonra aşağıdaki kodları çalıştırarak ortamınızı oluşturabilirsiniz. Eğer Anaconda Python (versiyondan bağımsız olarak) bilgisayarınızda kuruluysa yeniden indirmenize gerek yok ancak sıfırdan kuracaksanız Python 3.x versiyonunu kurmaya özen gösterin.

- Sanal Ortam Oluşturma:
```shell
conda create -n tensorflow python=3.6 # En son Python versiyonunu kullanın
source activate tensorflow
```

- Paketleri yükleme (Tensorflow, Numpy'ı otomatik yüklediği için onu açıkça yüklemeye gerek yok):
```shell
# Eğer tensorflow gpu yüklemek istiyorsanız tensorflow yerine tensorflow-gpu yazın. MacOS'ta GPU support yok.
pip install --upgrade tensorflow 

conda install pandas
conda install scikit-learn
conda install pillow
conda install scikit-image

#Jupyter notebookları tensorflow sanal ortamında çalıştırmak için gerekli
pip install ipykernel
python -m ipykernel install --user --name tensorflow --display-name "TF" 

# Sanal ortamı kapatmak için
source deactivate tensorflow
```

- Jupyter Notebook çalıştırma:
```shell
# Sanal ortamı aktive ediyoruz
source activate tensorflow

# Notebookları oluşturacağımız veya notebookların bulunduğu klasör
cd /path/to/notebooks
jupyter notebook # Kernel'ı değiştirmeyi unutmayın
```

Tensorflow-GPU Nvidia GPUlarla çalışmak üzerine tasarlandı. GPU desteğini aktifleştirmek için Tensorflow [dökümanında](https://www.tensorflow.org/install/) belirtildiği versiyonlarıyla CUDA ve cuDNN yüklemek gerekebilir. Lütfen GPU desteğiyle kurulum yapmak için dökümanı takip edin. Kendi işletim sisteminiz için olan komutları uygulayın.

Bu repo'daki Jupyter notebooklarını açtığınız zaman 'Kernel' menüsünden 'Change Kernel' diyip, 'TF' kernel'ını seçmeyi unutmayın. Eğer ana ortamınızda tensorflow yoksa, bu kernel'ı seçmediğiniz taktirde kodlar çalışmayacaktır.


This project is licensed under the terms of the MIT license.

## İçerik

Bu reponun planlanan içeriği aşağıdaki gibidir:

- Doğrusal Regresyon
- Multi-layer Perceptron
- Convolutional Neural Networks
- Recurrent Neural Networks
- Autoencoders
- Reinforcement Learning

