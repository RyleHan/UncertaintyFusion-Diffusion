# UncertaintyFusion-Diffusion
Uncertainty Estimation Fusion for Optimizing Diffusion Model Inference

This project aims to explore and implement a fusion framework for uncertainty estimation methods in the inference phase of diffusion models. The goal is to improve model stability and generalization while optimizing the sampling strategy without increasing training costs.

## 🔍 Background

In diffusion generative models, the inference process is typically fixed, lacking an awareness of the uncertainty at key stages of the sampling process. This project combines two mainstream uncertainty estimation techniques:

1. **Last Layer Laplace Approximation (LLLA)**: Used for modeling the posterior distribution of the model output.
2. **Monte Carlo Sampling Variance (MC)**: Multi-sample noise estimation at a critical time step during inference, used to estimate the variance.

We propose a **fusion framework** that dynamically adjusts the sampling path by linearly combining the uncertainty estimates from these two methods.

## 🔧 Project Structure


## ✅ Current Progress

- [x] Implemented Last Layer Laplace Approximation module
- [x] Implemented Monte Carlo Sampling module
- [x] Validated both methods independently
- [x] Built fusion framework and conducted initial tests
- [ ] Tuning the fusion strategy (ongoing)
- [ ] Evaluation on generative tasks (planned)

## 💡 Next Steps

- Investigating a learnable weight or dynamic control mechanism for fusion weights;
- Scaling the method for larger models like Stable Diffusion;
- Exploring combinations with active sampling or attention mechanisms.

## ✍️ Author

Graduate student working on uncertainty estimation and inference optimization in generative models.

Feel free to reach out for collaboration or discussion.
