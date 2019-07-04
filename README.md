# Disco-GAN-Tensorflow
***
This repositroy shows fashion items data orientated Disco-GAN implementation by using tensorflow.
***
  -Original Research Paper: [Leraning to Discover Cross-Domain Relations with Generative Adversarial Networks](https://arxiv.org/pdf/1703.05192.pdf)<br>
  -Related github Repo: [SKTBrain/Disco-GAN](https://github.com/SKTBrain/DiscoGAN)
![Disco-GAN](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/Disco-GAN-explain.jpeg)
***

#### For more detail infos such as prerequisites, code descriptions, params setting, db setting, followed [this](https://github.com/HyeongminLEE/Tensorflow_DiscoGAN) link.

# 1. Train
```bash
python3 train.py --train_A <directory-first-database> --train_B <directory-second-databse --epochs <#> --batch_size <#>
```

# 2. Training Result
***

- First trial: using edges2handbags(first) and edges2shoes(second) - 2 and 26 Epochs

![hb-s-hs-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_hb_s_hb_EP002_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![hb-s-hb-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_hb_s_hb_EP026_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![hb-s-hb-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/hb-shoes-hb.gif)

![s-hb-s-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_s_hb_s_EP002_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-hb-s-img](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/output/output_s_hb_s_EP026_Batch000000.jpg)&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
![s-hb-s-gif](https://github.com/hogyun3709/Disco-GAN-Tensorflow/blob/master/docs/shoes-hb-shoes.gif)

- Second trial: using Top(first) and Bottom(second)
