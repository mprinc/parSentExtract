```sh
git clone https://github.com/mprinc/parSentExtract
```

requirements.txt

https://pypi.org/project/tensorflow/#history
https://pypi.org/project/numpy/#history
https://pypi.org/project/scikit-learn/#history
https://pypi.org/project/scipy/#history

```sh
pyenv install 3.7.2
pyenv virtualenv 3.7.2 python3.7.2_env
pyenv local python3.7.2_env

# https://github.com/tensorflow/tensor2tensor/issues/1754#issuecomment-565844926
python -m pip install tensorflow==1.14.0
python -m pip install numpy==1.15.2
python -m pip install scipy==1.1.0
python -m pip install scikit-learn==0.19.2
# import sklearn


python train.py --source_train_path ../data/train.en --target_train_path ../data/train.fr --source_valid_path ../data/valid.en --target_valid_path ../data/valid.fr --checkpoint_dir ../tflogs
```