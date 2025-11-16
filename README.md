## CAD-Recode: Reverse Engineering CAD Code from Point Clouds

:hugs: Model [v1](https://huggingface.co/filapro/cad-recode), [v1.5](https://huggingface.co/filapro/cad-recode-v1.5), [cadrille](https://github.com/col14m/cadrille) :hugs: ZeroGPU Space [v1.5](https://huggingface.co/spaces/filapro/cad-recode) :hugs: Dataset [v1](https://huggingface.co/datasets/filapro/cad-recode), [v1.5](https://huggingface.co/datasets/filapro/cad-recode-v1.5) :globe_with_meridians: Project [Page](https://cad-recode.github.io/)

**News**:
 * :fire: June, 2025. CAD-Recode is accepted at ICCV 2025.
 * :rocket: March, 2025. We update CAD-Recode to v1.5. More details in [changelog](CHANGELOG.md).
 * :fire: December, 2024. CAD-Recode is state-of-the-art in three CAD reconstruction benchmarks: <br>
  DeepCAD [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/cad-recode-reverse-engineering-cad-code-from/cad-reconstruction-on-deepcad)](https://paperswithcode.com/sota/cad-reconstruction-on-deepcad?p=cad-recode-reverse-engineering-cad-code-from) <br>
  Fusion360 [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/cad-recode-reverse-engineering-cad-code-from/cad-reconstruction-on-fusion-360-gallery)](https://paperswithcode.com/sota/cad-reconstruction-on-fusion-360-gallery?p=cad-recode-reverse-engineering-cad-code-from) <br>
  CC3D [![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/cad-recode-reverse-engineering-cad-code-from/cad-reconstruction-on-cc3d)](https://paperswithcode.com/sota/cad-reconstruction-on-cc3d?p=cad-recode-reverse-engineering-cad-code-from)

This repository contains an implementation of CAD-Recode, a 3D CAD reverse engineering method introduced in our paper:

> **CAD-Recode: Reverse Engineering CAD Code from Point Clouds**<br>
> [Danila Rukhovich](https://github.com/filaPro),
> [Elona Dupont](https://scholar.google.com/citations?user=i9J6YFMAAAAJ),
> [Dimitrios Mallis](https://scholar.google.com/citations?user=Gfc5ZXoAAAAJ),
> [Kseniya Cherenkova](https://scholar.google.com/citations?user=VepvFBkAAAAJ),
> [Anis Kacem](https://scholar.google.com/citations?user=K3EWusMAAAAJ),
> [Djamila Aouada](https://scholar.google.com/citations?user=WBmJVSkAAAAJ) <br>
> Univesity of Luxembourg <br>
> https://arxiv.org/abs/2412.14042

### Inference Demo

CAD-Recode transforms point cloud to 3D CAD model in form of Python code ([CadQuery](https://github.com/CadQuery/cadquery) library). CAD-Recode is trained upon Qwen2-1.5B, keeping original tokenizer, and adding a single additional linear layer. 
In this repo we provide simple inference demo. Install python packages according to our [Dockerfile](Dockerfile) and run [demo.ipynb](demo.ipynb) in jupyter.

<p align="center">
  <img src="https://github.com/user-attachments/assets/8f127e71-628d-48f1-80f4-df4f645dd3fe" alt="CAD-Reocde scheme"/>
</p>
<p align="center">
  <img src="https://github.com/user-attachments/assets/90c06dbd-3563-45a5-968e-91fc5b768213" alt="CAD-Recode predictions"/>
</p>

### Citation

If you find this work useful for your research, please cite our paper:

```
@inproceedings{rukhovich2025cad,
  title={Cad-recode: Reverse engineering cad code from point clouds},
  author={Rukhovich, Danila and Dupont, Elona and Mallis, Dimitrios and Cherenkova, Kseniya and Kacem, Anis and Aouada, Djamila},
  booktitle={Proceedings of the IEEE/CVF International Conference on Computer Vision},
  pages={9801--9811},
  year={2025}
}
```
