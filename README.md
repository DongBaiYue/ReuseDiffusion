## 下载模型参数
以cogvideox为例
```
# 下载模型，模型参数位于 ./models/cogvideox
python3 down_models.py --mode download --models cogvideox --save_dir ./models
# 测试模型，生成内容为 ./results/cogvideox/test.mp4
python3 down_models.py --mode test --models cogvideox --save_dir ./models
```
## 运行模型
```
# original
python3 generate.py --model cogvideox --model_dir ./models --mode original --benchmark --gpu 0
# reuse
python3 generate.py --model cogvideox --model_dir ./models --mode reuse --benchmark --gpu 0
```
