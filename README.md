# **PMaF: Deep Declarative Layers for Principal Matrix Features**
This is the official implementation of our paper on [arXiv](https://arxiv.org/abs/2306.14759) which is duplicated from [ddn/apps](https://github.com/anucvml/ddn/tree/master/apps/PMaF).

If you find this paper or code useful, please cite our work as follows,
```
@inproceedings{Xu:ICML23w,
  author    = {Zhiwei Xu and
               Hao Wang and
               Yanbin Liu and
               Stephen Gould},
  title     = {{PMaF}: Deep Declarative Layers for Principal Matrix Features},
  booktitle = {ICML Workshop on Differentiable Almost Everything: Differentiable Relaxations, Algorithms, Operators, and Simulators},
  year      = {2023}
}
```

# How to Use
We explore two differentiable deep declarative layers, namely least squares on sphere (LESS) and implicit eigen decomposition (IED), for learning the principal matrix features (PMaF) which refers to a single vector summarising a data matrix.

## Environment
We use PyTorch 1.12.0 on a single 3090 GPU.

## Least Squares on Sphere (LESS)
In LESS/test_least_squares_sphere.py, set "enable_viz_proj=True" for all figures (with 8 examples) in the paper;
set "enable_viz_proj=False" for the table in the paper.

Then, run
```
cd LESS
python test_least_squares_sphere.py
```
Results will be saved in LESS/results.

## Implicit Eigen Decomposition (IED)
Run IED/12_implicit_eigen_decomposition.ipynb.
One can change "enable_symmetric" for the symmetricity and non-symmetricity of the input matrix.

Results (Session "Statistics of precision" in the Jupyter notebook) with figures, tables, and .csv files will be saved in IED/results.

# Troubleshooting
For any enquires, please contact <zwxu064@gmail.com>.
