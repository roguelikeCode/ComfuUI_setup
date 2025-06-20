# 準備
# mambaをインストール（Condaと互換性のあるパッケージマネージャー）
# condaより高速（入れていないと1日経ってもインストールが終わらない）
```
conda install mamba -n base -c conda-forge -y
```
# WSLのLinux環境（例: Ubuntu）をセットアップした直後は、C++のコンパイルに必要なビルドツール群がインストールされていない
# 基本的なビルドツールであるg++ (GNU C++ Compiler), gcc (GNU C Compiler), make, cmakeをインストールする

# パッケージリストの更新
```
sudo apt update
```
# build-essential パッケージのインストール
```
sudo apt install build-essential -y
```
# cmake のインストール
```
sudo apt install cmake -y
```
