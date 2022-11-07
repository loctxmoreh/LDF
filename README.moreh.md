# [Moreh] Running LDF on HAC service
![](https://badgen.net/badge/Nvidia-A100/pass/green)

## Prepare

### Code
```bash
git clone https://github.com/loctxmoreh/LDF
cd LDF
```

### Download word embedding
Download the `glove.6B.50d.json` embedding using [this ggdrive
link](https://drive.google.com/file/d/1vCm_X2vrSSwLICwmm4NW2-dXfNtV8TFg/view?usp=sharing)
and put it in `./word_embedding` directory.

### Environment
Use `a100env.yml` to create a `conda` environment:
```bash
conda env create -f a100env.yml
conda activate ldf
```

## Run
Use the `a100-train` script:
```bash
./a100-train
```
