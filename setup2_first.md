# Python 3.10で作成（mssについて、3.10でないとインストールできないため）
```
conda create -n comfyui_wsl_poetry_py310_cu118_env python=3.10 -y
conda activate comfyui_wsl_poetry_py310_cu118_env
```

# 最初に忘れずに
# LinuxのパスはWindowsと逆であるため
# 必要であれば（cd "$(wslpath 'C:\Users\yoshi\OneDrive\Desktop\ComfyUI-master')"）
```
conda activate comfyui_wsl_poetry_py310_cu118_env
```

# 現在アクティブなConda環境のPython実行ファイルのパスを連携させる
```
cd ~/projects/comfyui-managed-env
poetry env use $(which python)
```

# 起動方法
```
poetry run python "$(wslpath 'C:\Users\yoshi\OneDrive\Desktop\ComfyUI-master\main.py')"
```
