Dark Channel Haze Removal
=========================

MATLAB implementation of "[Single Image Haze Removal Using Dark Channel Prior][1]"

	Single Image Haze Removal Using Dark Channel Prior
	Kaiming He, Jian Sun and Xiaoou Tang
	IEEE Transactions on Pattern Analysis and Machine Intelligence
	Volume 30, Number 12, Pages 2341-2353
	2011

<img src="https://raw.githubusercontent.com/sjtrny/Dark-Channel-Haze-Removal/master/forest.jpg" width="200px"/>
&nbsp;
<img src="https://raw.githubusercontent.com/sjtrny/Dark-Channel-Haze-Removal/master/forest_recovered.jpg" width="200px"/>


CUDA acceleration implemented by Tom Heaven, hanlin_tan@nudt.edu.cn. To use CUDA mex function, you need to 

+ edit mex_CUDA_*.xml properly for WIN, LINUX or MAC platform. Example configuration files for vs2013+cuda7.5 and xcode8.0+cuda8.0 are provided.
+ compile cuGetDarkChannel.cu with 
```
mex -v cuGetDarkChannel.cu
```
or
```
mexcuda -v cuGetDarkChannel.cu
```
for Matlab2015b or later.
+ set `useGPU = true` in demo_fast.m.



[1]: http://research.microsoft.com/en-us/um/people/kahe/cvpr09/ 
