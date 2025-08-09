  
## Dual-Perception Prompt Learning: Illumination-Adaptive and Semantic-Aware Guidance for Backlit Image Enhancement (Under Review)


### 📌 TODO
- Our Code is coming soon！


## 🔎 Overview framework
![Network](/figs/Figures_Framework.png)
![Framework](/figs/Figures_network7.png)

## ⚙️ Method Setup
In our proposed **Dual-Perception Prompt Learning** framework, we jointly leverage *illumination-adaptive guidance* and *semantic-aware guidance* to tackle the backlit image enhancement problem.

### 📚 Datasets
We train and evaluate our model on multiple publicly available datasets, including **BAID**, **MIT**, **SICE**, and **MSEC**.  


### 🛠 Preprocessing
All input images are resized to **960×720** during training.  
Standard data augmentation techniques (random crop, horizontal/vertical flip, rotation) are applied to improve robustness.

### ⚡ Training Details
- **Optimizer**: AdamW, initial learning rate = `2e-4`  
- **Batch size**: `8`  
- **Iteration**: *50+250k* (varies by dataset size)  
- **Learning rate schedule**: Cosine annealing decay  
- **Hardware**: 1 × NVIDIA RTX 4090 GPUs

## 📷 Quantitative comparison results
![Comparison results of BAID Dataset.](/figs/Figures_BAID4.png)
![Comparison results of MIT Dataset.](/figs/Figures_mit3.png)
![Comparison results of SICE Dataset.](/figs/Figures_app_low.png)
![Comparison results of MSEC Dataset.](/figs/Figures_app_over.png)


