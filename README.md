# Caffe SegNet cuDNN5
**This is a modified version of [Caffe](https://github.com/BVLC/caffe) which supports the [SegNet architecture](http://mi.eng.cam.ac.uk/projects/segnet/)**

As described in **SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation** Vijay Badrinarayanan, Alex Kendall and Roberto Cipolla [http://arxiv.org/abs/1511.00561]

Please refer to Alex Kendalls caffe-segnet for tutorial and a guide how to use it (https://github.com/alexgkendall/caffe-segnet).

Since the original caffe-segnet supports just cuDNN v2, which is not supported for new pascal based GPUs, it was possible to decrease the inference time by 25 % to 35 % with caffe-segnet-cudnn5 using Titan X Pascal.

## Installation

Ensure you have [CUDA](https://developer.nvidia.com/cuda-toolkit) and [cudNN](https://developer.nvidia.com/cudnn) installed. This has only been tested up to CUDA v9.2.

To install all depedencies, follow the instructions located at the top of the [Ubuntu 16.04 Installation Guide](https://github.com/BVLC/caffe/wiki/Ubuntu-16.04-Installation-Guide). This installation guide goes on to discuss installation using the Makefile, which is recommended for Python users.

### Makefile

Follow the remaining instructions from the [Ubuntu 16.04 Installation Guide](https://github.com/BVLC/caffe/wiki/Ubuntu-16.04-Installation-Guide).

Some of the necessary changes to the Makefile have already been made, however, the above guide does provide a good reference for installation dependencies and build steps.

## Publications

If you use this software in your research, please cite their publications:

http://arxiv.org/abs/1511.02680
Alex Kendall, Vijay Badrinarayanan and Roberto Cipolla "Bayesian SegNet: Model Uncertainty in Deep Convolutional Encoder-Decoder Architectures for Scene Understanding." arXiv preprint arXiv:1511.02680, 2015.

http://arxiv.org/abs/1511.00561
Vijay Badrinarayanan, Alex Kendall and Roberto Cipolla "SegNet: A Deep Convolutional Encoder-Decoder Architecture for Image Segmentation." arXiv preprint arXiv:1511.00561, 2015. 

## License

This extension to the Caffe library is released under a creative commons license which allows for personal and research use only. For a commercial license please contact the authors. You can view a license summary here:
http://creativecommons.org/licenses/by-nc/4.0/
