
## Overview
This project performs various computations on transition probability matrices, eigenvalue decomposition, and Principal Component Analysis (PCA) on images. The goal is to analyze the long-run behavior of Markov chains and apply PCA for dimensionality reduction of images.

## Dependencies
Ensure you have the required Python libraries installed before running the scripts.
```sh
pip install numpy matplotlib scipy opencv-python
```

## Files
- `main.py`: The main script that contains all computations and analysis.
- `utils.py`: Utility functions for loading and processing images.
- `data/`: Directory containing images for PCA analysis.
- `w4_unittest.py`: Unit tests for validation.

## Features
1. **Markov Chains Analysis**
   - Computes steady-state probabilities using eigenvalue decomposition.
   - Simulates transitions over multiple steps.
2. **Eigenvalue & Eigenvector Computation**
   - Extracts the dominant eigenvector.
   - Verifies eigenvector correctness.
3. **Image Processing with PCA**
   - Loads and centers images.
   - Computes the covariance matrix.
   - Performs PCA for dimensionality reduction.
   - Reconstructs images using different numbers of principal components.
   - Plots explained variance.

## Usage
Run the script to execute all computations:
```sh
python main.py
```

## Outputs
- Eigenvalues and eigenvectors of the transition matrix.
- Long-run probabilities of being at each webpage.
- Images reconstructed from various principal components.
- Explained variance plots.

## Example Results
- **Transition Matrix Eigenvalues:**
  ```
  Eigenvalues of P:
  [ 1.         -0.7037  0.0054 -0.0827 -0.2190]
  ```
- **Long-run Probabilities:**
  ```
  [[0.3938]
   [0.1339]
   [0.1141]
   [0.0851]
   [0.2731]]
  ```
- **PCA Explained Variance:**
  ![Explained Variance Plot](./results/explained_variance.png)

## License
This project is open-source and available under the MIT License.

