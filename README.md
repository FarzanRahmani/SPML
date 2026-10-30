# Security and Privacy in Machine Learning

Graduate coursework on robustness, model security, and privacy, completed during the third semester of my M.Sc. in Computer Engineering, specializing in Artificial Intelligence, at Sharif University of Technology. Instructor: Dr. Amir Mahdi Sadeghzadeh. Author: Farzan Rahmani.

## Assignment Guide

| Directory | Topics |
| --- | --- |
| `HWs/HW0/` | Numerical/image-processing foundations: SVD and Gaussian filtering |
| `HWs/HW1/` | Adversarial examples: FGSM, Carlini-Wagner, DeepFool, and universal perturbations |
| `HWs/HW2/` | Adversarial training and defensive-distillation/zeroth-order attack exercises |
| `HWs/HW3/` | Backdoor and model-extraction exercises, with distillation reference material |
| `HWs/HW4/` | Differential privacy and federated learning |
| `sources/` | Supporting privacy reference material |

Assignment folders include statements, theory submissions, starter notebooks, completed versions, and selected papers. Files ending in `403210725.ipynb` identify my practical submissions.

## Practical Environment

Use Python with Jupyter or Google Colab. Neural-network exercises use PyTorch/torchvision with numerical and plotting libraries. The differential-privacy notebook also uses **Opacus**, scikit-learn, and modern `torch.func` APIs for per-sample gradients.

Select a compatible PyTorch/torchvision installation for your hardware, then install the additional libraries required by the chosen notebook. There is no single pinned environment for the whole repository.

## Running an Exercise

1. Read the assignment and select the submitted notebook or starter version.
2. Review imports, data-download cells, device selection, checkpoint paths, and training budgets.
3. Configure data/model access and run cells sequentially. A GPU is recommended for training and iterative attacks.
4. Compare metrics using the exact threat model or privacy-accounting assumptions described by the exercise.

For adversarial experiments, record perturbation norm/budget, step count, and evaluation settings. For DP experiments, interpret accuracy alongside epsilon, delta, clipping norm, sampling rate, and the accountant. The DP notebook includes RDP accounting, vectorized gradients, fine-tuning, and membership-inference evaluation.

## Scope and License

These are controlled coursework experiments and historical results, not production privacy guarantees or certified defenses. See [LICENSE](LICENSE) for repository license terms; papers, datasets, and teaching material retain their original terms and attribution.
