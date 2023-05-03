# Python GPT4All

This package contains a set of Python bindings that runs the `llmodel` C-API.


# Installation Instructions

TODO: Right now instructions in main README still depend on Qt6 setup. To setup Python bindings, we just need `llmodel` to be built which is much simpler. However, in the future, the below installation instructions should be sequentially organized such that we expect the main README's instructions were followed first.

1. Setup `llmodel`

```
git clone --recurse-submodules https://github.com/nomic-ai/gpt4all-chat
cd gpt4all-chat/llmodel/
mkdir build
cd build
cmake ..
cmake --build . --parallel
```
Confirm that `libllmodel.dylib` exists in `gpt4all-chat/llmodel/build`.

2. Setup Python package

```
cd ../../bindings/python_gpt4all
pip3 install --upgrade pip setuptools
pip3 install -r requirements.txt
python3 setup.py install
```

3. Test it out! In a Python script or console:

```python

import 


```
