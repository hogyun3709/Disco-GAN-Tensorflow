# Disco-GAN-Tensorflow
***
This repositroy shows fashion items data orientated Disco-GAN implementation by using tensorflow.
***
  -Original Research Paper: [Leraning to Discover Cross-Domain Relations with Generative Adversarial Networks](https://arxiv.org/pdf/1703.05192.pdf)<br>
  -Related github Repo: [SKTBrain/Disco-GAN](https://github.com/SKTBrain/DiscoGAN)
![Disco-GAN](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/Disco-GAN-explain.jpeg)
***
### Paper-summary
- Labeling and paring datas are costful and labor intensive
- By given 'unpaired data' GAN finds relations btw two diff domains
- No pre-trained model required
- Two diff GAN coupled together



#### For more detail infos such as prerequisites, code descriptions, params setting, db setting, followed [this](https://github.com/HyeongminLEE/Tensorflow_DiscoGAN) link.

# 1. Train
```bash
python3 train.py --train_A <directory-first-database> --train_B <directory-second-databse --epochs <#> --batch_size <#>
```

# 2. Training Result
***

- First trial: using edges2handbags(first) and edges2shoes(second) - around 49,000 imgs(SHOES) - 130,000 imgs(HBG) - 30 epoch

![hb-s-hs-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_hb_s_hb_EP002_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![hb-s-hb-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_hb_s_hb_EP026_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![hb-s-hb-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/hb-shoes-hb.gif)

![s-hb-s-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_s_hb_s_EP002_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-hb-s-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_s_hb_s_EP026_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-hb-s-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/shoes-hb-shoes.gif)

- Second trial: using clutch bag(first) and sandals(second) - around 1,300 - 1,400 images per items - 200 epochs - 19 steps

![cb-s-cb](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_EP200_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![cb-s-cb](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/cb-s-cb.gif)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-cb-s](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_EP198_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-cb-s](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/s-cb-s.gif)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

- Third trial: using brand logo(first) and soccer shoes(second) - around 5,700 images(shoes) - 8,000(brand logo)
![logo-shoes](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_EP199_Batch000000_Logo_Shoes.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![logo-shoes-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/logo-shoes.gif)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![shoes-logo](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_EP189_Batch000000_Shoes_Logo.jpg)&nbsp;&nbsp;
![shoes-logo-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/shoes-logo.gif)
