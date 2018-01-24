# Under Construction

# Robust FFT-Based Image Registration Tools for Python
This program provides robust image registration method using "Phase Correlation" technique.

With this toolbox, you can estimate 
Translation, Rotation and Scaling between two images.

Output form is supported: Affine Matrix, each parameter
If you used this programs, please cite our paper below:

>  Y. Ri, H. Hiroshi Fujimoto. : \`\`Practical Phase-Only Correlation Algorithm for Robust and Accurate Image Sencing'', <i> Now Under Review </i> Vol. X, pp.XX. (20XX) 

# Getting started 
## Requirements
- Python3.X (3.5 is recommended)
- Opencv3.X
- Numpy

For windows and Linux users, **anaconda** is one of the choise to install both of this.

## Install

```
pip install imregpoc
```

## Running the tests


# LICENSE
BSD license

## Citation
Currently please refer [following paper](http://hflab.k.u-tokyo.ac.jp/papers/2017/SAMCON2017_ri.pdf)
:
> Y. Ri and H. Fujimoto, “Image Based Visual Servo Application on Video Tracking with Monocular Camera Based on Phase Correlation Method,” The 3rd IEEJ international workshop on Sensing, Actuation, Motion Control, and Optimization, 2017.

This paper will be updated sooner.

# Short description
## 1. Phase-Correlation based Translation Estimate (POC)
Image translation can be detected with the cross correlation of 2D FFT spectrum of spacial frequency.

$$
\begin{eqnarray}
 R(k_1,k_2)=\frac{F(k_1,k_2)\overline{G(k_1,k_2)}}{|F(k_1,k_2)\overline{G(k_1,k_2)}|}
\end{eqnarray}
$$

## 2. Phase-Correlation based Rotation and Scaling Estimate (RIPOC)
Using log-polar trasformation, rotation and scaling can also detected with phase correlation technique.


$$
\begin{eqnarray}
	(\delta_x,\delta_y)=(N\theta/\pi,-N\log_N \kappa)
\end{eqnarray}
$$

## Other related links

>  K. Takita, T. Aoki, Y. Sasaki, T. Higuchi and K. Kobayashi. : \`\`High-Accuracy Subpixel Image Registration Based on Phase-Only Correlation'', <i> IEICE Transactions on Fundamentals of Electronics, Communications and Computer Sciences </i> Vol. E86-A, pp. 1925-1934. (2003) 
