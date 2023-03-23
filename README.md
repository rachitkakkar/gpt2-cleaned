# gpt2-cleaned
Just a cleaned up and stripped down version of the gpt2 model for personal use. Easy to set up and well documented, and I am not responsible for anything this model creates.

# Requirements 
Listed in requirements.txt

# Runtime
Runs python-3.6.8

# How To Use
Install requirements and use the `predict({prompt})` or `sample_model()` in textgen.py

You will have to use download_model.py to download the models. It works the same way it works in the original gpt2 repo.

Predict:
Used to generate text with a prompt, pass in a prompt and optionally change any of the parameters.

```python
def predict(
    model_prompt,
    model_name='124M',
    seed=None,
    nsamples=1,
    batch_size=1,
    length=None,
    temperature=1,
    top_k=0,
    top_p=1,
    models_dir='models/'
):
```
Sample Model:
Used to generate text without a prompt, nothing you have to pass in but you can optionally change any of the parameters.

```python
def sample_model(
    model_name='124M',
    seed=None,
    nsamples=0,
    batch_size=1,
    length=None,
    temperature=1,
    top_k=0,
    top_p=1,
    models_dir='models/',
):
```

# License
I kept it under the same license gpt-2 uses, because I didn't change much code, just shuffled and renamed some things.

# Original Code
https://github.com/openai/gpt-2/
