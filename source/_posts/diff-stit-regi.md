---
title: >-
  Image Stitching 과 Image Registration 의 차이 (the difference between image
  stitching and image registration)
tags:
  - image processing
  - computational photography
  - image stiching
  - image registration
categories:
  - image processing
date: 2019-08-02 21:59:21
---

Image Stitching 과 Image Registration 의 차이를 알아보자. 

### 1. Image registration 
>Image registration is the process of transforming different sets of data into one coordinate system. [[1]](https://en.wikipedia.org/wiki/Image_registration)  
> 설명 : 이미지 여러장(different sets of data)을 같은 좌표계로 변환해주는 과정

### 2. Image stitching 
>Image stitching or photo stitching is the process of combining multiple photographic images with overlapping fields of view to produce a segmented panorama or high-resolution image. [[2]](https://en.wikipedia.org/wiki/Image_stitching#Registration)  
>설명 : 서로 겹치는 여러 이미지들을 가지고 파노라마 같은거 만드는 과정 
---
아래와 같은 파노라마 영상을 만드는 테스크는 **image stitching**의 일종이라고 할 수 있습니다. **image stitching**은 일련의 과정들을 거치는데 그 과정 중 하나가 **image registration** 입니다.  가령, 여러 이미지에서 key points(feature vector) 를 추출하고 이들 간의 유사도를 기반으로 homography transformation matrix를 계산합니다 (이 또한 한 과정입니다) 그 다음 수행하는 작업이 **image registration** 이라고 할 수 있겠습니다.

결론 : **image registration** 은 **image stitching** 의 sub process 이다.

![image](https://user-images.githubusercontent.com/15168540/62371683-6b240c80-b570-11e9-8b69-e7b5304b5c99.png)


**References**  
[1] https://en.wikipedia.org/wiki/Image_registration  
[2] https://en.wikipedia.org/wiki/Image_stitching#Registration