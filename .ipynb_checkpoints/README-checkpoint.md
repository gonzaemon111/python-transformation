# Python 透視投影用リポジトリ

様々なバージョン

|ライブラリ|バージョン|
|:---:|:---:|
|pyenv|anaconda-3.5.1|
|opencv|4.1.2|

---

久しぶりにこのリポジトリを訪れた場合の動かし方

```bash
$ jupyter lab
```

qiita-traff.ipynbを山椒のように

```python

%matplotlib inline
import cv2
import matplotlib.pyplot as plt

img = cv2.imread('./data/traff3.jpeg', cv2.COLOR_BGR2RGB) #imreadの第2引数に0を指定するとグレースケールで読み込み

print(cv2.COLOR_BGR2RGB) # 4
# plt.gray() #matplotlibでグレースケールを使用する場合はグレースケールで読み込むように指定
plt.imshow(img) # cv2.imshowメソッドよりもmatplotlibのimshowメソッドで画像を表示する方が良い。

```


README

## 開発環境構築

```bash
$ git clone git@github.com:gonzaemon111/python-transformation.git
$ cd python-transformation
https://waseda.app.box.com/folder/96315617308にアクセスしてdev_images.zipをダウンロード
$ jupyter lab
```