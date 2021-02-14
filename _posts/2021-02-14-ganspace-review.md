---
layout: post
title: "Ganspace: Discovering interpretable gan controls 리뷰"
date: 2021-02-14 01:00
author: choyi0521
tags: [machine-learning]
---

# 소개
&nbsp;&nbsp;&nbsp;&nbsp;GANs는 이미지 스타일 변화 테스크에서 굉장한 성능을 보여주고 있습니다. 특히, StyleGAN, BigGAN과 같은 최신 모델은 이미 실제와 구분이 힘들정도로 자연스러운 이미지를 생성합니다. 유저가 아웃풋 이미지를 원하는 형태로 조절하는 연구 또한 많이 진행되었으나 대부분 추가적인 라벨을 사용해서 모델을 학습하는 것에 초점을 맞추고 있습니다. 이런 라벨이 있는 학습 데이터를은 만드는 데 큰 비용과 시간을 요구합니다.

&nbsp;&nbsp;&nbsp;&nbsp;"Ganspace: Discovering interpretable gan controls"는 NIPS 2020에 accept된 논문으로 latent space에서 PCA를 해서 모델의 이미지 생성을 조작하는 방법을 소개합니디. 이 방법은 추가적인 supervision을 사용하지 않고 간단한 연산으로 이미지를 조작합니다.

# PCA

# GANs의 생성 모델

# Principal feature direction 찾기

## StyleGAN

## BigGAN

# Layer 별로 조작하기

# 결과

# 의견

&nbsp;&nbsp;&nbsp;&nbsp;논문의 방법이 잘 적용되기 위해서는 PCA를 적용할 latent space에서 semantic label을 공유하는 점들이 연속적인 위치에 배치되어야 할 것 같습니다. StyleGAN을 비롯한 대부분의 최신 모델들은 학습시 피쳐를 disentangled하게 만드는 과정이 있어서 괜찮아 보이지만 그렇지 않은 경우(ex. vanilla GANs)에는 논문의 방법이 잘 적용될지 확인해야 할 것 같습니다.

&nbsp;&nbsp;&nbsp;&nbsp;

# 참고문헌
* [<span style="color:blue">Ganspace:
Discovering interpretable gan controls</span>](https://arxiv.org/abs/2004.02546)