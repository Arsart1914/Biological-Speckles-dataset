# Viable Bio-Speckle Dataset

This repository provides the dataset description and samples for the paper:

> **Linhao Li, Xia Wang, Yifan Deng, Peiyang Xing**, "Spectral-augmented learning for viable bio-speckle reconstruction," ***Optics Express* 34(20), 37554–37575 (2026)**.
> DOI: [10.1364/OE.612049](https://doi.org/10.1364/OE.612049) · [Full text](https://opg.optica.org/oe/fulltext.cfm?uri=oe-34-20-37554)

## Dataset overview

**Viable Bio-Speckle Dataset** contains **32,600 strictly paired target–speckle images** acquired by projecting target patterns onto a digital micromirror device (DMD) and recording the scattered intensity **through metabolically viable ex-vivo rat skin** (used within 4 h of excision, saline-treated only).

| Subset | Targets | Pairs | Split |
|---|---|---|---|
| `mnist_dataset` | Binarized MNIST digits (56×56) | **20,000** | train 14,500 / test 2,500 / val 3,000 |
| `vessel_dataset` | FIVES vessel-segmentation patterns (56×56) | **12,600** | train 9,000 / val 1,800 / test 1,800 |

- **Speckle images**: 1936 × 1464, 16-bit grayscale TIFF (~5.4 MB each); raw volume ≈ 172.3 GB
- **Targets**: 56 × 56 binary PNG
- **Pairing**: within each split, files are sequentially numbered from 0 and identically named — `speckle/00000.tiff` ↔ `target/00000.png`

## Samples

The [`samples/`](samples/) folder shows 10 example pairs (20 images) from both subsets and all splits — `*_speckle.png` are 8-bit downsampled previews of the recorded speckle, `*_target.png` are the corresponding targets (upscaled 4× for visibility). Original speckle files are 16-bit TIFF at full resolution.

## Directory structure of the full dataset

```
Viable_Bio-Speckle_dataset/
├── mnist_dataset/
│   ├── train/  speckle/ (14,500 tiff)  target/ (14,500 png)
│   ├── test/   speckle/ ( 2,500 tiff)  target/ ( 2,500 png)
│   └── val/    speckle/ ( 3,000 tiff)  target/ ( 3,000 png)
└── vessel_dataset/
    ├── train/  speckle/ ( 9,000 tiff)  target/ ( 9,000 png)
    ├── val/    speckle/ ( 1,800 tiff)  target/ ( 1,800 png)
    └── test/   speckle/ ( 1,800 tiff)  target/ ( 1,800 png)
```

## Obtaining the full dataset

The full dataset is approximately **172 GB uncompressed** and **94 GB compressed**. It is distributed as a three-part RAR5 archive with a recovery record and SHA-256 checksums.

**The full dataset is currently available by email request.** Due to the large file size and current transfer constraints, a complete public download is not available at this time. Please contact **[191676960@qq.com](mailto:191676960@qq.com)** to obtain the full dataset and arrange a suitable transfer method.

Example image pairs remain publicly available in the [`samples/`](samples/) folder. We apologize for any inconvenience.

## Citation

If you use this dataset, please cite:

```bibtex
@article{Li2026spectral,
  author  = {Li, Linhao and Wang, Xia and Deng, Yifan and Xing, Peiyang},
  journal = {Optics Express},
  title   = {Spectral-augmented learning for viable bio-speckle reconstruction},
  volume  = {34},
  number  = {20},
  pages   = {37554--37575},
  year    = {2026},
  doi     = {10.1364/OE.612049}
}
```

## License

The dataset and samples are released under **Creative Commons Attribution 4.0 (CC-BY-4.0)**.

## Contact

- Dataset requests & questions: **191676960@qq.com**
