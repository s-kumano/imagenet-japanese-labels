# ImageNet日本語ラベル
以下もご参考になさってください．

- [1] 英語ラベル https://gist.github.com/yrevar/942d3a0ac09ec9e5eb3a
- [2] 日本語ラベル https://gist.github.com/PonDad/4dcb4b242b9358e524b4ddecbee385e9
- [3] 日本語ラベル https://github.com/starpentagon/python_scripts/blob/master/dataset/ILSVRC2012_class_name/ILSVRC2012_class_name.csv

本レポジトリは[1]と[3]を基に作成されました．

# 読み込み例

## Python
```python
def read_labels(path: str) -> list[str]:
    with open(path, 'r') as f:
        labels = [label.replace('\n', '') for label in f.readlines()]
    return labels
```
