# Disco-GAN-Tensorflow
***
This repositroy shows fashion items data orientated Disco-GAN implementation by using tensorflow.
***
  -Original Research Paper: [Leraning to Discover Cross-Domain Relations with Generative Adversarial Networks](https://arxiv.org/pdf/1703.05192.pdf)<br>
  -Related github Repo: [SKTBrain/Disco-GAN](https://github.com/SKTBrain/DiscoGAN)
***

#### For more detail infos such as prerequisites, code descriptions, params setting, db setting, followed [this](https://github.com/HyeongminLEE/Tensorflow_DiscoGAN) link.

# 1. Train
```bash
python3 train.py --train_A <directory-first-database> --train_B <directory-second-databse --epochs 30 --batch_size 64
```

# 2. Result
***

- First trial: using edges2handbags(first) and edges2shoes(second) - 26 Epochs
