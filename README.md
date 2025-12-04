# Dataset for AIAA 2024: Optimizing Diffusion to Diffuse Optimal Designs
Now on Hugging Face! : https://huggingface.co/datasets/IDEALLab/airfoil_2d_v0

(although the additional intermediate airfoils are only available here for now)

Provides the RANS-optimized airfoil dataset mentioned in the paper. The dataset is stored in .pkl files in the `data` folder. Alternatively, you can use only the optimized airfoils and associated performance values in the 'data\optimized_data' folder (read the readme in that folder for more information).To be updated with more processed data and examples as needed. 

Contact cdiniz@ethz.ch for any questions.

Please cite the paper if you use this dataset in your research:

Diniz, Cashen, and Mark Fuge. "Optimizing Diffusion to Diffuse Optimal Designs." AIAA SCITECH 2024 Forum. 2024.

@inproceedings{diniz2024optimizing,
  title={Optimizing Diffusion to Diffuse Optimal Designs},
  author={Diniz, Cashen and Fuge, Mark},
  booktitle={AIAA SCITECH 2024 Forum},
  pages={2013},
  year={2024}
}

## Abstract
Generative models offer the possibility to accelerate and potentially substitute parts of the often expensive traditional design optimization process. However, current implementations of these models often ignore aspects of the optimization process that, among other benefits, could be used to improve model accuracy and design feasibility. We implement a latent denoising diffusion model (DDM) capable of generating airfoil geometries conditioned on flow parameters and an area constraint. Additionally, we create a novel, diverse dataset of optimized airfoil designs that better reflects a realistic design space than has been done in previous work. The model is applied to this dataset, and key metrics are assessed both statistically and with an open-source computational fluid dynamics (CFD) solver to determine the performance of the generated designs. Our final contribution is the implementation of a diffusion model with a variance schedule based on the statistical changes in design variables along the aggregate optimization trajectories of our data. We find this model produces better-performing airfoils and improves design feasibility. We acknowledge that the verification and reasons behind this improvement remain unclear, but hope to present an initial step towards further investigations of optimization-informed generative models.
