# Qiskit Project on Raspberry Pi 5

This project demonstrates the implementation of quantum circuits using Qiskit on a Raspberry Pi 5. It compares the execution of a bit flip code on a classical computer (Pi 5) with its performance on a real quantum computer.

## Project Overview

1. **Setup**: Install Qiskit and other necessary packages on your Raspberry Pi 5. Use the  `01-step` file for installation.

2. **Development Environment**: Use Visual Studio Code on your local laptop for SSH connection to the Raspberry Pi 5.

3. **Classical Simulation**: Run a bit flip code (using NOT gate, bit-flip gate) on the Raspberry Pi 5 with a circuit depth of 127, followed by measurement (main section of code takes about 10.5s, screenshot attached in media folder, on pi5 all containers are running already (pihole, jellyfin, portainer etc). For my laptop running Arch linux, it takes around 7.3s). It gives you the flavour of computing power of Pi 5 chip. Although it's not absolute, but in perepective.

4. **Quantum Measurement**: Implement a bit flip code using CNOT gate (more known as 'X' gate or bit-flip gate) and measure it using the Pauli Z operator to obtain the <Z> expectation value.

5. **Comparison**: Compare the results from the Raspberry Pi 5 simulation with those from a real quantum computer. This comparison highlights the imperfections in real qubits and the need for error correction techniques.

6. **Project Files**: 
   - Use the `02-step` file for Raspberry Pi 5 operations.
   - Use the `03-step` for quantum computer operations using Pi 5.

7. **IBM Quantum Setup**:
   - Obtain a token from the IBM Quantum website.
   - Create a `.qiskit` folder in your home directory.
   - Place the token in a JSON file within the `.qiskit` folder (template provided here).
   - This project uses Visual Studio for IBM Quantum access instead of a web browser.

## Why This Project Matters

This Qiskit project offers a hands-on experience in quantum computing. By comparing classical simulations with real quantum hardware results, you'll gain insights into:

- The challenges of working with real quantum systems
- The importance of error correction in quantum computing
- Current research focuses in quantum computing, particularly in error mitigation

## Getting Started

1. Set up your Raspberry Pi 5 with the necessary software (refer to installation instructions).
2. Clone this repository to your Raspberry Pi 5.
3. Follow the step-by-step instructions in the provided files to run the experiments.
4. Compare and analyze the results from classical simulation and quantum hardware.

## Contributing

We welcome contributions to this project! If you have suggestions for improvements or have developed additional experiments, please feel free to open an issue or submit a pull request.

## Resources

For more information on Qiskit and quantum computing, check out the following resources:

- [Qiskit Documentation](https://qiskit.org/documentation/)
- [IBM Quantum](https://quantum-computing.ibm.com/)
- [Quantum Computing at NASA](https://www.nasa.gov/directorates/spacetech/strg/quantum/)

---

Happy quantum computing!
