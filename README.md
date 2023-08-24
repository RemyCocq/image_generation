
# How to install

## 1. Install Pytorch, better with GPUs

Use the command adapted to your setup from here : https://pytorch.org/get-started/locally/

For instance:
`pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118`

Verify the installation by running `python` and the following lines:

```python
import torch
x = torch.rand(5, 3)
print(x)
```

Should return something like:
```python
tensor([[0.3380, 0.3845, 0.3217],
        [0.8337, 0.9050, 0.2650],
        [0.2979, 0.7141, 0.9069],
        [0.1449, 0.1132, 0.1375],
        [0.4675, 0.3947, 0.1426]])
```

And running this with GPUs:
```python
import torch
torch.cuda.is_available()
```

Which should return `True`

## 2. Install other requirements

Run `pip install -r requirements.txt`

## 3. Run jupyter lab

Run `python -m jupyterlab`

# See more

You can find other usages here:
https://huggingface.co/docs/diffusers/api/pipelines/stable_diffusion/stable_diffusion_xl
