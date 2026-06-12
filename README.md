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
    (.venv) uv sync
    ```
3. Login into Huggingface to download datasets and weights

Set the **HF_TOKEN** environment variable with your **HuggingFace** [token](https://huggingface.co/settings/tokens) (see [HuggingFace Authentication Setup](https://ispras-wibe.readthedocs.io/en/latest/quick_start.html#huggingface-authentication-setup) for details), then authenticate:

```console
(.venv) python huggingface_login.py
```

4. Launch the script

Specify the path to your `сonfiguration file` as a required parameter:

```console
(.venv) wibench --config configs/configs/test_lfm_metr.yml.yml
```
