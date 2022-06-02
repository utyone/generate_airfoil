# generate_airfoil

## About This repo
This repository consists of sourse codeds for the following paper:
Title: Inverse Airfoil Design Method for Generating　Varieties of Smooth Airfoils Using Conditional　WGAN-GP  
Link: https://assets.researchsquare.com/files/rs-618399/v1_covered.pdf?c=1624375613
For more details, please refer to this slide (Japanese only)(https://github.com/miyamotononno/generate_airfoil/issues/13) .

## setup
You need to install [pytorch](https://pytorch.org/).
You also need to install XFoil (https://github.com/KikeM/xfoil-python) to run "calc_cl.py." 
If you have difficulties installinf XFoil from the repository above, please refer to [here](https://github.com/miyamotononno/generate_airfoil/issues/14). Or, you can use other xfoil implementations. 

## run

```
Train the conditional GAN model: 
python3 -m normal.train

Ecaluate the conditional GAN model
python3 -m normal.eval

Train the conditional wgan-gp model: 
python3 -m wgan_gp.train

Evaluate the conditional wgan-gp model: 
python3 -m wgan_gp.eval
```
