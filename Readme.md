# BB84 Quantum Key Distribution Simulation

This project simulates the BB84 Quantum Key Distribution (QKD) protocol using Qiskit.

## Features
- Alice generates random bits and bases
- Optional eavesdropping (Eve) affecting the key
- Bob randomly chooses measurement bases
- Sifting process to extract shared key
- QBER (Quantum Bit Error Rate) calculation

## Requirements
- Python 3.x
- Qiskit
- Jupyter Notebook

### Install
```bash
pip install qiskit jupyter
```

## Usage
```bash
jupyter notebook bb84_simulation.ipynb
```
Run the notebook step-by-step. Set `eavesdrop=True` in `simulate_bb84()` to simulate an attack.

## Example Output
```
No Eve
Alice: [0, 1, 1, 0]
Bob:   [0, 1, 1, 0]
QBER: 0.0

With Eve
Alice: [0, 1, 1, 0]
Bob:   [1, 0, 1, 0]
QBER: 0.5
```

## License
MIT
