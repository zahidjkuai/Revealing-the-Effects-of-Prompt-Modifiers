# Revealing the Effects of Prompt Modifiers in Image Generation
This work presents a practical experiment platform for controlled textto-image generation and semantic embedding analysis. Images are generated via
a locally hosted Stable Diffusion model through the ComfyUI API, with fully controlled parameters — including seed, CFG scale, sampler, scheduler, and resolution.
Prompt modifiers such as happy, rich, or aggressive are applied with explicit numerical weighting using the syntax a (attribute:strength) subject, enabling systematic
sweeps of attribute intensity from 0.1 to 4.0. Multiple art styles can be layered with
independent strength parameters, providing fine-grained compositional control
over generated content. To compare images across different parameter settings and
prompts, all outputs are encoded into a shared 512-dimensional CLIP embedding
space. These embeddings are projected into 2D via UMAP, clustering images by
subject and batch origin to visually reveal how different prompt configurations
shift the latent distribution. For single-image analysis, alignment with semantic
modifiers is quantified using a bipolar softmax scoring mechanism over CLIP cosine similarities. Scores across all tracked attributes are rendered simultaneously
in a radar chart, aiming to reveal how the dominant prompt modifier correlates
with neighboring semantic attributes — exposing whether, for example, a happy
image inherently scores high on joyful and friendly. The key strength of this tool
lies in bridging prompt engineering and latent space interpretation: it empowers
researchers to systematically audit how diffusion models encode, entangle, and
respond to semantic attributes — making it a practical instrument for studying
prompt sensitivity, attribute interference, and embedding structure in generative
image models.

![Screenshot_2026_02_22-12](https://github.com/user-attachments/assets/9bbd77cb-40b7-46b2-82b5-cb7d59336f84)
![Screenshot_2026_02_22-9](https://github.com/user-attachments/assets/f9251f5b-9f3d-4943-bb2b-33a24e592b94)
![Screenshot_2026_02_22-7](https://github.com/user-attachments/assets/3613bc28-1a2b-4e0b-a11f-b08cb741849e)
![Screenshot_2026_02_22-5](https://github.com/user-attachments/assets/3892d21a-f057-4d33-b11f-fc8e2783f29e)
![Screenshot_2026_02_22-3](https://github.com/user-attachments/assets/1cd87ada-67d3-4d5f-97de-531f37c862a6)
![Screenshot_2026_02_22-1](https://github.com/user-attachments/assets/8532bd9e-f814-4360-9aa6-32347c45be39)
