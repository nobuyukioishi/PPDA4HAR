# Simulation-enabled Physically Plausible Data Augmentation for Wearable IMU-based Human Activity Recognition
PhD Thesis, University of Sussex, 2025  
Author: Nobuyuki Oishi

## Abstract
Wearable devices equipped with inertial measurement units (IMUs) are widely used for human activity recognition (HAR), but effective HAR model training requires extensive annotated datasets, which are costly and challenging to collect. Signal transformation-based data augmentation (STDA) methods, adapted by common time-series augmentation techniques, aim to address this data scarcity. However, they often lack domain-specific realism and physical plausibility, limiting their effectiveness. Meanwhile, advances in video-based human pose estimation have made virtual IMU simulation increasingly accessible, creating promising opportunities for simulation-based augmentation via systematic parameter modifications. However, existing simulation approaches still face a substantial fidelity gap between simulated and real IMU signals, which limits their practical use. This thesis argues that PPDAs realised through physics-based virtual IMU simulation yield more effective data for training HAR models than conventional STDAs, provided the fidelity gap is addressed. To demonstrate this, we first explore simulation-based augmentations through a digit-drawing gesture recognition task, revealing promising benefits but also highlighting the fidelity gap as a critical limitation. To address this limitation, we introduce WIMUSim, a differentiable simulation framework designed to generate high-fidelity virtual IMU data by precise parameter identification through gradient descent, using concurrently recorded wearable IMU and motion data. Leveraging WIMUSim, we propose PPDA methods and systematically evaluate their effectiveness using three public datasets (REALDISP, REALWORLD, MM-Fit). Our evaluations in fully supervised learning scenarios demonstrate that PPDA enhances HAR classification accuracy and reduces the number of subjects required for effective model training compared to STDAs. Extending PPDA into self-supervised contrastive learning, we observe substantial improvements in downstream HAR performance and label efficiency. Collectively, these results support the central thesis that simulation-enabled physically plausible data augmentations provide more effective data for HAR than conventional STDAs. This data-centric approach incorporates domain knowledge into augmentations to mitigate data collection burdens and enables efficient and ethically responsible use of human-subject data, particularly relevant in contexts where data collection is especially challenging, such as research involving vulnerable populations.

## Code Access
- **Chapter 4 - WIMUSim: A Differentiable Framework for High-Fidelity Wearable IMU Simulation**  
https://github.com/STRCWearlab/WIMUSim

- **Chapter 5: Evaluating PPDA against STDA for Supervised Training of HAR Models**  
https://github.com/STRCWearlab/PPDA

- **Chapter 6: Evaluating PPDA against STDA for Self-Supervised Contrastive Learning on Wearable IMU Data**  
https://github.com/STRCWearlab/PPDA_Contrastive




