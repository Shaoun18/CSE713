
---

# Flood Impact Detection on Roads Using U-Net

This project leverages the U-Net deep learning architecture for flood impact detection on roads using satellite or aerial imagery. The system provides pixel-level segmentation to identify flood-affected areas accurately, enabling efficient emergency response and infrastructure management.

## Features
- **High-Resolution Image Segmentation**: Achieves accurate flood impact detection with pixel-level precision.
- **Deep Learning Architecture**: Utilizes the U-Net framework for robust and scalable image segmentation.
- **Data Augmentation**: Employs techniques such as flipping, zooming, and rotation to enhance model generalization.
- **Evaluation Metrics**: Uses IoU, Dice Coefficient, and F1 Score for performance evaluation.

## Project Structure
```
├── data/                      # Contains input images and masks
├── src/                       # Core project code
│   ├── preprocessing.py       # Data preprocessing scripts
│   ├── model.py               # U-Net architecture implementation
│   ├── train.py               # Model training script
│   ├── evaluate.py            # Model evaluation script
│   ├── utils.py               # Helper functions
├── notebooks/                 # Jupyter notebooks for experiments
├── results/                   # Evaluation metrics, plots, and results
├── requirements.txt           # List of Python dependencies
└── README.md                  # Project documentation
```

## Methodology
1. **Data Preprocessing**: 
   - Resize and normalize images.
   - Apply data augmentation techniques to enhance model robustness.

2. **Model Architecture**: 
   - U-Net with encoder-decoder design and skip connections for accurate segmentation.

3. **Training and Validation**:
   - Train the model using binary cross-entropy and Dice loss.
   - Monitor performance using validation data.

4. **Evaluation**:
   - Calculate IoU, Dice Coefficient, and F1 Score to measure model performance.

## Results
- **Accuracy**: Achieved a Dice Coefficient of 0.6 and IoU score of 0.8533.
- **Visualization**: Pixel intensity distribution and segmentation masks validate the model's efficacy.

## Limitations
- **Data Imbalance**: Flooded regions are often underrepresented.
- **High Computation Requirements**: Processing high-resolution images demands significant computational resources.

## Future Work
- Integration with IoT devices for real-time flood detection.
- Deployment on edge computing systems for low-latency analysis.
- Improved generalization using diverse geographical datasets.

## How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. Preprocess the data:
   ```bash
   python src/preprocessing.py
   ```
4. Train the model:
   ```bash
   python src/train.py
   ```
5. Evaluate the model:
   ```bash
   python src/evaluate.py
   ```

## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## Authors
- **Shaoun Chandra Shill** - BRAC University
- **Fahim Ahmed Ifty** - BRAC University
- **Effat Jahan** - BRAC University  
- **Tuhin Ahmed** - BRAC University  

## License
This project is licensed under the MIT License.

---