[![arXiv](https://img.shields.io/badge/arXiv-2610.02010-b31b1b.svg)](https://arxiv.org/abs/2610.02010)

# Latent Frequency Masking Attack

Official implementation of "Exploring Weaknesses of Generative Image Watermarks against Latent Frequency Masking"


This repository builds upon code from the WIBE repository  https://github.com/ispras/wibe

## Reproduce

1. Update the submodules:

    ```console
    git submodule update --init --recursive
    ```

2. Install base virtual environment:

    ```console
    (.venv) uv sync --extra base
    ```
3. Login into Huggingface to download datasets and weights

Set the **HF_TOKEN** environment variable with your **HuggingFace** [token](https://huggingface.co/settings/tokens) (see [HuggingFace Authentication Setup](https://ispras-wibe.readthedocs.io/en/latest/quick_start.html#huggingface-authentication-setup) for details), then authenticate:

```console
(.venv) python huggingface_login.py
```

4. Launch the script

Specify the path to `сonfiguration file` as a required parameter:

```console
(.venv) wibench --config configs/test_lfm_metr.yml
```

## Citation
```
@misc{aistov2026exploringweaknessesgenerativeimage,
      title={Exploring Weaknesses of Generative Image Watermarks against Latent Frequency Masking}, 
      author={Kirill Aistov and Khaled Abud and Irina Serzhenko and Egor Kovalev and Aleksey Yakushev and Aleksandr Akimenkov and Dmitry Obydenkov and Yury Markin and Sergey Lavrushkin and Dmitriy Vatolin and Anastasia Antsiferova},
      year={2026},
      eprint={2610.02010},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2610.02010}, 
}
```