# Neural POS Tagging

This project implements Part-of-Speech (POS) tagging using two different neural network architectures: Feed Forward Neural Network (FFNN) and Recurrent Neural Network (RNN). The project compares different model configurations and analyzes their performance on development and test sets.

## Models

### 1. Feed Forward Neural Network (FFNN)

#### Hyperparameters
- Hidden layer size
- Number of layers
- Embedding dimensions
- Activation functions (ReLU, Tanh)

#### Key Findings
1. Lower complexity models (single layer, smaller hidden size, smaller embedding dimension) showed better performance
2. ReLU activation function generally performed better than Tanh
3. Increasing model complexity (more layers, larger hidden size) did not necessarily improve performance
4. Test set performance aligned well with development set, indicating good generalization

### 2. Recurrent Neural Network (RNN)

#### Hyperparameters
- Hidden layer size
- Bidirectional configuration
- Embedding dimensions
- Activation functions

#### Key Findings
- Configuration 3 (lower complexity, bidirectional LSTM) achieved the best performance
- Tanh activation function worked better in the best-performing configuration
- Bidirectional LSTM helped capture better contextual information
- Higher complexity models showed lower performance

## Results

### FFNN Results
- Development set accuracies for all configurations
- Test set accuracy for the best model
- Analysis of context window size vs. development set accuracy

### RNN Results
- Development set accuracies for all configurations
- Test set accuracy for the best model
- Epoch-wise accuracy plots for:
  - Best model (test set)
  - Model 1 (dev set)
  - Model 2 (dev set)
  - Model 3/Best model (dev set)
