# QSBench

![QSBench Banner](https://i.imgur.com/VyLgYtf.png)

**High-quality synthetic quantum datasets for Quantum Machine Learning, noise robustness, and sim-to-real research.**

We build the missing bridge between ideal quantum simulation and real hardware behavior.

---

### 🌟 What is QSBench?

QSBench is an open-source ecosystem that generates **clean, reproducible, richly annotated quantum circuit datasets** with:

- Paired **ideal vs noisy** expectation values
- Advanced realistic noise models (thermal relaxation, readout, device-like, etc.)
- Comprehensive circuit metrics and structural features
- Deterministic train/val/test splits based on circuit hash
- Full metadata, schema, and human-readable data cards

Everything is designed for modern quantum machine learning research and benchmarking.

---

### ✨ Core Capabilities

- **Multiple circuit families** — HEA, RealAmplitudes, QFT, random, and mixed
- **Advanced noise models** — thermal relaxation (T1/T2), readout error, device-like (GenericBackendV2), phase damping, and more
- **Rich features** — adjacency matrix, gate entropy, Meyer-Wallach entanglement, full gate statistics
- **GPU-accelerated generation** with Qiskit Aer
- **Parquet + CSV** output with complete provenance
- **Reproducible splits** and full metadata for every release

---

### 📦 What We Provide

| Repository / Resource                    | Purpose |
|------------------------------------------|---------|
| **[QSBench-Generator](https://github.com/QSBench/QSBench-Generator)** | Main open-source generator (v5.1.0) — create your own datasets |
| **[Hugging Face Organization](https://huggingface.co/QSBench)** | Ready-to-use public datasets and demos |
| **Demo Releases**                        | Thermal, Device, Readout, Amplitude, Depolarizing, etc. |
| **Full Releases**                        | Core, Noise Pack, Hardware-mimic, Research Suite |

---

### 🚀 Quick Start

```bash
docker compose build --no-cache

docker compose run --rm quantum-gen \
  python3 generate.py \
  --n-qubits 8 \
  --depth 6 \
  --n-samples 2048 \
  --noise thermal_relaxation \
  --noise-params '{"t1": 50e-6, "t2": 30e-6}' \
  --dataset-name MyFirstQSBench
```

---

### Why Researchers Love QSBench

- **Realistic noise** — far beyond simple depolarizing channels

- **Reproducibility** — deterministic splits, fixed seeds, full provenance

- **Rich metadata** — every release comes with `data_card.md`, `schema.json`, `meta.json`

- **Ready for ML** — perfect for tabular regression, feature extraction, and sim-to-real tasks

- **Community-first** — fully open-source under permissive licenses

---

### Use Cases

- Noise robustness & error mitigation benchmarking

- Sim-to-real transfer learning

- Expectation value regression under realistic noise

- Circuit family classification

- Hardware-aware quantum ML

- Academic research and publications

---

### Join the Community

- ⭐ Star our repositories

- 🗣️ Open issues and feature requests

- 🧪 Generate and publish your own datasets

- 📬 Contact us for collaborations or custom releases

**We welcome contributions** from quantum researchers, QML engineers, and open-source enthusiasts.

---

### License

- Generator: **Apache 2.0** License

- Demo Datasets: **CC BY-NC 4.0** (research & personal use)

---

### Citation

```bibtex
@misc{qsbench2026,
  author       = {NikolaI Iankovich},
  title        = {QSBench: Synthetic Quantum Datasets for QML Benchmarking},
  year         = {2026},
  url          = {https://github.com/QSBench},
  note         = {Open-source quantum dataset generator and benchmark collection}
}
```

---

**Made with ❤️ for the quantum community**

[Website](https://qsbench.github.io) • [Hugging Face](https://huggingface.co/QSBench) • [Generator Repository](https://github.com/QSBench/QSBench-Generator)
