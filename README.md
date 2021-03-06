# MFF-GAN
Code of paper MFF-GAN: An unsupervised generative adversarial network with adaptive and gradient joint constraints for multi-focus image fusion.
````
@article{zhang2021mff,
  title={MFF-GAN: An unsupervised generative adversarial network with adaptive and gradient joint constraints for multi-focus image fusion},
  author={Zhang, Hao and Le, Zhuliang and Shao, Zhenfeng and Xu, Han and Ma, Jiayi},
  journal={Information Fusion},
  volume={66},
  pages={40--53},
  year={2021},
  publisher={Elsevier}
}
````
#### Recommended Environment:<br>
 - [ ] python = 2.7
 - [ ] tensorflow-gpu = 1.9.0
 - [ ] numpy = 1.15.4
 - [ ] h5py = 2.9.0
 - [ ] scipy = 1.2.0
 - [ ] opencv = 2.4.11
 

#### Prepare data :<br>
Run "main.m" (the first function) to convert source images from RGB color space to YCbCr.

#### To train :<br>
Put training image pairs (Y channel) in the "Train_near" and "Train_far" folders, and run "CUDA_VISIBLE_DEVICES=0 python main.py" to train the network.

#### To test :<br>
Put test image pairs (Y channel) in the "Test_near" and "Test_far" folders, and run "CUDA_VISIBLE_DEVICES=0 python test.py" to test the trained model.
You can also directly use the trained model we provide.

#### Restore the output of networks to RGB space :<br>
Run "main.m" (the second function) to restore the output of networks to RGB color space.
