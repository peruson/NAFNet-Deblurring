# NAFNet-Deblurring
- NAFNet을 이용한 Deblurring 작업 파이프라인 구축 및 튜닝
  
* Dataset
    * GoPro Dataset
    * train : 2103 장 / test : 1111 장 (차후 validation : test = 1 : 1 비율로 나누어 테스트 예정)
    * image shape : 1280 x 720

* Default Configs
    * device : Cuda (GPU T4 x 2)
    * image_resize : 256x256
    * num_workers = 4
    * batch_size = 16

## 진행 사항

- 12/02
  * learning rate : 1e-3
  * epoch = 5
  * param : set 1
  * optimizer : Adam
  * scheduler : None
 
  * result : {Avg Loss: 70.1300, Avg PSNR: 29.8700, Avg SSIM: 0.9269}, {Val Loss: 71.0571, Val PSNR: 28.9429, Val SSIM: 0.9219}
