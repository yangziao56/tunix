<p align="center">
  <img src="assets/readme-banner.svg" width="100%" alt="Dynamic Trajectory Valuation — Value trajectories. Guide post-training." />
</p>

### Not All Rollouts Are Worth Learning: On Trajectory Valuation for Post-Training Reinforcement Learning

Xuesong Jia<sup>&#42;</sup>, **Ziao Yang**<sup>&#42;</sup>, Zhanhe Huang, and Hongfu Liu  
<sub>*Equal contribution.</sub>

**[PDF](https://arxiv.org/pdf/2609.35072)** · **[Paper](https://arxiv.org/abs/2609.35072)** · **[Explore code](#explore-the-research-code)**

---

Research code on the **`my-changes`** branch of our [Tunix fork](https://github.com/yangziao56/tunix/tree/my-changes), with gradient-based sample curation for GRPO and DPO.

## Explore the research code

| Workflow | Entry point |
| :--- | :--- |
| GRPO self-influence curation | [`tunix/rl/self_inf_trainer.py`](tunix/rl/self_inf_trainer.py) |
| GRPO experiment launcher | [`my_example/run_dbc_self_inf_batch.sh`](my_example/run_dbc_self_inf_batch.sh) |
| DPO recipes and curation variants | [`examples/dpo/README.md`](examples/dpo/README.md) |
| DPO implementation | [`tunix/sft/dpo/dpo_trainer.py`](tunix/sft/dpo/dpo_trainer.py) |
| SFT → DPO workflow | [`examples/ultrafeedback/README.md`](examples/ultrafeedback/README.md) |
| DeepScaler experiments | [`examples/deepscaler/README.md`](examples/deepscaler/README.md) |

## Getting started

```bash
git clone --branch my-changes --single-branch https://github.com/yangziao56/tunix.git
cd tunix
```

Choose a recipe from the table above for environment setup, model configuration, and launch commands. The DPO recipes support `baseline`, `outlier_l2`, and `self_inf_batch` comparisons.

## Built on Tunix

This research branch builds on [Google Tunix](https://github.com/google/tunix), a JAX-based library for LLM post-training. The original project introduction, installation guide, citation, and acknowledgements are preserved in the [Tunix README](README-tunix.md).

---

<details>
<summary><strong>Citation</strong></summary>

```bibtex
@misc{jia2026tunix,
  title = {Not All Rollouts Are Worth Learning: On Trajectory Valuation for Post-Training Reinforcement Learning},
  author = {Jia, Xuesong and Yang, Ziao and Huang, Zhanhe and Liu, Hongfu},
  year = {2026},
  eprint = {2609.35072},
  archivePrefix = {arXiv},
  url = {https://arxiv.org/abs/2609.35072}
}
```

</details>
