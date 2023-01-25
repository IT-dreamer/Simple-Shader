[English Overview](/README_En.md)
# 紹介
このシェーダはモデルの簡単なシェーディングができる。ノーマルシェーダー、phongシェーダー、UVテクスチャシェーダー、バンプマップ、ディスプレースメントマップがあります。


# 要件

ライブラリや他の配置を行う必要はありません。実行可能ファイルが事前に用意したので、そのままで実行してもokですよ。*Rasterize.exe*をクリックして、カラフルな子牛が出て来ます。AとSを押すとモデルが回転されます。ESCがプログラムを終了させます。モデルファイルとテクスチャファイルがあらかじめ用意されていますが、他のモデルやテクスチャを使用することもできます。

# 使用方法

- Normal Shader(デフォルト)

```
.\Rasterizer.exe normal
```
![avatar](/doc/picture/normal.png)
- Phong Shader

```
.\Rasterizer.exe phong
```
![avatar](/doc/picture/phong.png)
- Texture Shader

```
.\Rasterizer.exe texture
```
![avatar](/doc/picture/texture.png)
- Bump Shader
```
.\Rasterizer.exe bump
```
![avatar](/doc/picture/bump.png)
- Displament Map
```
.\Rasterizer.exe displacement
```
![avatar](/doc/picture/displacement.png)
- **A** : モデルを左に回転
- **D** : モデルを右に回転させます
- **Esc** : プログラムを終了します



