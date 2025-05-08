# Quantum Fraud Detection using Grover's Algorithm

This project implements **Grover's Quantum Search Algorithm** to detect fraudulent transactions in a financial dataset.  
It was developed as a group project for **CYS 536: Quantum Computation and Quantum Security** at Imam Abdulrahman Bin Faisal University.

## Test Descriptions

The project simulates three test scenarios:

- **Test 1 (Fixed Marked State):**  
  Always selects the first fraudulent transaction as the marked state to test deterministic amplification.

- **Test 2 (Random Marked State):**  
  Randomly selects one fraudulent transaction as the marked state in each run to demonstrate the probabilistic nature of Grover’s algorithm.

- **Test 3 (No Fraud Present):**  
  Simulates the case when no fraudulent transactions are present in the sample to avoid unnecessary computations.

The provided scripts implement Test 1 and Test 2. Test 3 is automatically handled if no fraud is detected.

## Files

- `grover_fraud_detection_random.ipynb`
- `grover_fraud_detection_fixed.ipynb`
- `FraudSample.csv`: **Modified version of the "Fraudulent Transactions Prediction" dataset from Kaggle**, used as input data for the project.

## Dataset License and Modifications

This project uses a **modified version** of the ["Fraudulent Transactions Prediction" dataset](https://www.kaggle.com/datasets/vardhansiramdasu/fraudulent-transactions-prediction) by **vardhansiramdasu** on Kaggle, licensed under the [Open Data Commons Open Database License (ODbL) v1.0](https://opendatacommons.org/licenses/odbl/1-0/).

**Modifications:**
- Randomly sampled 100 rows from the original dataset.
- Edited values in the `isFraud` column to ensure multiple fraudulent transactions are present in the 100-row sample.
- The notebook further samples 16 rows from this uploaded 100-row dataset for quantum circuit execution.

See [LICENSE_DATA.txt](LICENSE_DATA.txt) for license and attribution details.

## Requirements

- Python 3.x
- Jupyter Notebook
- Qiskit
- Pandas
- Matplotlib
- Pillow
- scikit-learn
- NumPy

## How to Run

1. Ensure that `FraudSample.csv` is in the same directory as the notebook files.
2. Open either notebook using Jupyter Notebook.

For random marked state (Test 2 and Test 3), open `grover_fraud_detection_random.ipynb`.

For fixed marked state (Test 1), open `grover_fraud_detection_fixed.ipynb`.

3. Run all cells in the notebook to execute the code.

## Contributors
- Sarh Alnemer
- Zahra Alakrawi
- Reham AlGhamdi
- Hawra Al-Basheer
- Dana AlOtaibi
- Razan Alfahad

## License

The source code in this repository is licensed under the MIT License.
See [`LICENSE`](LICENSE) for details.

The dataset (`FraudSample.csv`) is licensed under the Open Data Commons Open Database License (ODbL) v1.0.
See [`LICENSE_DATA.txt`](LICENSE_DATA.txt) for the full license notice.