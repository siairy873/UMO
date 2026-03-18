# UMO: Unified In-Context Learning Unlocks Motion Foundation Model Priors

[![Website](https://img.shields.io/badge/Website-UMO-orange)](https://oliver-cong02.github.io/UMO.github.io/) [![Paper](https://img.shields.io/badge/arXiv-PDF-b31b1b)](https://arxiv.org/pdf/2603.15975) [![arXiv](https://img.shields.io/badge/arXiv-2603.15975-red)](https://arxiv.org/abs/2603.15975)

> **UMO: Unified In-Context Learning Unlocks Motion Foundation Model Priors** <br>

> [Xiaoyan Cong](https://oliver-cong02.github.io/)\*, [Zekun Li](https://kunkun0w0.github.io/)\*, [Zhiyang Dou](https://frank-zy-dou.github.io/), [Hongyu Li](https://lhy.xyz/), [Omid Taheri](https://otaheri.github.io/), [Chuan Guo](https://ericguo5513.github.io/), [Abhay Mittal](https://scholar.google.com/citations?hl=en&user=BwE_L4MAAAAJ&view_op=list_works&sortby=pubdate), [Sizhe An](https://sizhean.github.io/), [Taku Komura](https://i.cs.hku.hk/~taku/), [Wojciech Matusik](https://cdfg.mit.edu/wojciech), [Michael J. Black](https://is.mpg.de/ps/person/black), [Srinath Sridhar](https://srinathsridhar.com/) <br>

## Abstract

<img src="./assets/teaser.png"/>

Large-scale foundation models (LFMs) have recently made impressive progress in text-to-motion generation by learning strong generative priors from massive 3D human motion datasets and paired text descriptions. However, how to effectively and efficiently leverage such single-purpose motion LFMs, i.e., text-to-motion synthesis, in more diverse cross-modal and in-context motion generation downstream tasks remains largely unclear. Prior work typically adapts pretrained generative priors to individual downstream tasks in a task-specific manner. In contrast, our goal is to unlock such priors to support a broad spectrum of downstream motion generation tasks within a single unified framework. To bridge this gap, we present UMO, a simple yet general unified formulation that casts diverse downstream tasks into compositions of atomic per-frame operations, enabling in-context adaptation to unlock the generative priors of pretrained DiT-based motion LFMs. Specifically, UMO introduces three learnable frame-level meta-operation embeddings to specify per-frame intent and employs lightweight temporal fusion to inject in-context cues into the pretrained backbone, with negligible runtime overhead compared to the base model. With this design, UMO finetunes the pretrained model, originally limited to text-to-motion generation, to support diverse previously unsupported tasks, including temporal inpainting, text-guided motion editing, text-serialized geometric constraints, and multi-identity reaction generation. Experiments demonstrate that UMO consistently outperforms task-specific and training-free baselines across a wide range of benchmarks, despite using a single unified model. Code and models will be publicly available.

## TODO

- [x] Project page
- [x] arXiv paper
- [ ] Code release (coming soon)
- [ ] Model release (coming soon)

## Citation

Please cite our paper if you find this repository useful:

```bibtex
@misc{cong2026umounifiedincontextlearning,
      title={UMO: Unified In-Context Learning Unlocks Motion Foundation Model Priors},
      author={Xiaoyan Cong and Zekun Li and Zhiyang Dou and Hongyu Li and Omid Taheri and Chuan Guo and Abhay Mittal and Sizhe An and Taku Komura and Wojciech Matusik and Michael J. Black and Srinath Sridhar},
      year={2026},
      eprint={2603.15975},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2603.15975},
}
```
