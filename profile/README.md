# QSBench

![QSBench Banner](https://i.imgur.com/VyLgYtf.png)

**High-quality synthetic quantum datasets for Quantum Machine Learning, noise robustness, and sim-to-real research.**

We build the missing bridge between ideal quantum simulation and real hardware behavior.

---

### 🌟 What is QSBench?

QSBench is an open-source ecosystem that generates **clean, reproducible, richly annotated quantum circuit datasets** with:

- Paired **ideal vs noisy** expectation values
- Advanced realistic noise models (thermal relaxation, readout error, device-like noise via GenericBackendV2, phase damping, etc.)
- Rich structural metrics (adjacency matrix, gate entropy, Meyer-Wallach entanglement, gate statistics)
- Deterministic train/val/test splits based on circuit hash
- Full metadata, schema, and human-readable data cards

Everything is designed for modern quantum machine learning research and benchmarking.

---

### ✨ Core Capabilities

- Multiple circuit families (HEA, RealAmplitudes, QFT, random, mixed)
- GPU-accelerated generation with Qiskit Aer
- Advanced noise models closest to real quantum hardware
- Parquet + CSV output with complete provenance
- Reproducible splits and full metadata for every release

---

### 📦 What We Provide

- **[QSBench Generator](https://github.com/QSBench/QSBench-Generator)** — open-source tool to create your own datasets
- Public datasets and demos on **[Hugging Face @QSBench](https://huggingface.co/QSBench)**

---

### Use Cases

- Noise robustness & error mitigation benchmarking
- Sim-to-real transfer learning
- Expectation value regression under realistic noise
- Hardware-aware quantum ML
- Academic research and publications

---

### Join the Community

- ⭐ Star our repositories
- 🗣️ Open issues and feature requests
- 🧪 Generate and publish your own datasets
- 📬 Contact us for collaborations

**We welcome contributions** from quantum researchers, QML engineers, and open-source enthusiasts.

---

### License

- Generator: **Apache 2.0**
- Datasets: **CC BY-NC 4.0** (research & personal use)

---

### 💰 Support QSBench

You can support the project directly on this Giveth page:  

- [Giveth](https://giveth.io/project/qsbench)
- USDT (TRC20): `TQcgRru2yjPjCtqDkHYMr5vsRcejbpk1zG`
- TON: `UQCPgjp_yK9c-Wn_708xDR_DZ6Pi6DnfqXfQRqQcc9W7xD0f`

Your donations help us generate larger datasets, cover GPU costs, and continue developing new realistic noise models.

---

**Made with ❤️ for the quantum community**

[Website](https://qsbench.github.io) • [Hugging Face](https://huggingface.co/QSBench) • [Generator Repository](https://github.com/QSBench/QSBench-Generator) • [Support on Giveth](https://giveth.io/project/qsbench)
