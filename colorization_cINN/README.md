Compiling the Joint Bilateral Filter
--------------------------------------

Simply run
```
python setup.py build_ext --inplace
```

Checkpoints
--------------------------------------

* Model checkpoint used for the paper:

  `https://drive.google.com/open?id=1gpHHtT7EcCoEqTzaUmDImp_tyB7vSKIN`

* Pretrained cond. net (only necessary if you want to train yourself, but not do the pretraining):

  `https://drive.google.com/open?id=1YQkOf03kK7-ZNDGJmVFloF_hZvnmjc0_`


--------------------------------------

## Docker build command (from the root directory of the repository):
`docker build -t anaglyph .`

## Docker run command:
`docker run -it --rm -p 8888:8888 -v /mnt/data/robin_grun/data:/workspace/data --runtime nvidia --gpus all --ipc=host --name anaglyph_container anaglyph`
