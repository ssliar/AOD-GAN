# AOD-GAN
AOD-GAN is based on **AOD-Net**:[An All-in-One Network for Dehazing and Beyond](https://arxiv.org/abs/1707.06543).
AOD-Net is a lightly model application to image dehaze.we extend the model and called AOD-GAN.

**Compare**

model    | Architecture |GAN Loss| MSE Loss |Perception Loss|
---------|--------------|--------|----------|---------------|
AOD-GAN  |    Only G    |   NO   |    Yes   |      NO       |
AOD-Net  |    G + D     |   Yes  |    Yes   |     Yes       |


**Environmention:**
- Python 3 
- Pytorch 0.4
- ubuntu 16.04

**Test On Image**
```
python TestImage.py --input input_image --output_image
```
**Test On Video**
```
python TestVideo.py --input input_video.mp4
```
**Results**
![input](imgs/1_input.jpg)![output](imgs/1_output.jpg)![detect](imgs/1_detect.jpg)
![input](imgs/2_input.jpg)![output](imgs/2_output.jpg)![detect](imgs/2_detect.jpg)
![input](imgs/3_input.jpg)![output](imgs/3_output.jpg)![detect](imgs/3_detect.jpg)
![input](imgs/4_input.jpg)![output](imgs/4_output.jpg)![detect](imgs/4_detect.jpg)
![input](imgs/5_input.jpg)![output](imgs/5_output.jpg)![detect](imgs/5_detect.jpg)

**References**
- [An All-in-One Network for Dehazing and Beyond](https://arxiv.org/abs/1707.06543).
  Boyi Li, Xiulian Peng, Zhangyang Wang, Jizheng Xu, Dan Feng.
- [Generative Adversarial Networks](https://arxiv.org/abs/1406.2661).
  Ian J. Goodfellow, Jean Pouget-Abadie, Mehdi Mirza, Bing Xu, David Warde-Farley, 
  Sherjil Ozair, Aaron Courville, Yoshua Bengio.
- [YOLOv3:An Incremental Improvement](https://pjreddie.com/media/files/papers/YOLOv3.pdf).
  Joseph Redmon, Ali Farhadi.
