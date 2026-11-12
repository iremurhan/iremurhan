# Beyza İrem Urhan

I work on multimodal representation learning. MSc in Computer Engineering, Boğaziçi University (2026).

My research looks at how pretrained vision–language models can be adapted to new data and tasks, and at how to tell whether an apparent improvement holds up under stricter evaluation. So far I have mostly studied contrastive image–text models on cross-modal retrieval: controlled fine-tuning interventions, compositional generalization, cross-dataset transfer, and diagnostics beyond aggregate Recall@K.

**Broader interests:** computer vision, natural language processing, domain generalization, machine learning for biomedical data.

## Current research code

**[clip-adaptation-limits](https://github.com/ALLab-Boun/clip-adaptation-limits)**: controlled fine-tuning interventions for CLIP image–text retrieval on Flickr30k and MS-COCO. A single configurable pipeline compares the following under matched settings:

- training objectives (InfoNCE, SigLIP) and partial unfreezing of the vision encoder
- intra-modal regularization with augmented image views and caption rewrites
- syntactic hard-negative captions and COCO object-class auxiliary supervision
- segment-aware and SAM-feature fusion

Evaluation covers in-domain retrieval, cross-dataset transfer, and compositional probing with SugarCrepe.

## MSc thesis (archived)

*Cross-Modal Retrieval: Interventions, Diagnostics, and Representational Limits*. Boğaziçi University, defended June 2026.

[clip-retrieval-lab](https://github.com/iremurhan/clip-retrieval-lab) contains the thesis code in its final state (tag `thesis-final`). It is archived and no longer maintained. Beyond the fine-tuning interventions, the thesis uses ViT-B/16 and ViT-L/14-336 backbones and adds diagnostics: MMVP-VLM, missing-positive analysis, alignment and uniformity of the embedding space, and cross-dataset transfer. For current work, see `clip-adaptation-limits` above.

## Selected projects

- [clip-product-image-text-matching](https://github.com/iremurhan/clip-product-image-text-matching): detecting mismatched product image–title pairs by fine-tuning CLIP with a cross-entropy pair classifier and with a margin-based contrastive loss. Uses image-disjoint splits to prevent leakage and compares against zero-shot CLIP with ROC-AUC.
- [pan19-authorship-attribution](https://github.com/iremurhan/pan19-authorship-attribution): cross-domain authorship attribution on PAN-19. Training and test texts come from different fandoms, so topic cues do not transfer. Uses character n-gram SVM ensembles with a reject option for unknown authors (team project).
- [cancer-biomarker-feature-selection](https://github.com/iremurhan/cancer-biomarker-feature-selection): ranking candidate biomarker genes in CuMiDa microarray data with L1-regularized logistic regression and random forests, scored by how consistently each gene is selected across cross-validation folds (BSc senior project).

## Tools

PyTorch, Hugging Face (Transformers, PEFT), scikit-learn, Weights & Biases · Python, Docker, SLURM, Git, Linux

## Contact

[LinkedIn](https://www.linkedin.com/in/iremurhan/)
