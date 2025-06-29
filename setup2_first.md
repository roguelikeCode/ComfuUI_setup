- Python 3.10で作成
```
conda create -n comfyui_wsl_poetry_py310_cu118_env python=3.10 -y
conda activate comfyui_wsl_poetry_py310_cu118_env
```

- 最初に忘れずに
- LinuxのパスはWindowsと逆であるため
- 必要であれば（cd "$(wslpath 'C:\Users\yoshi\OneDrive\Desktop\ComfyUI-master')"）
```
conda activate comfyui_wsl_poetry_py310_cu118_env
```

- 現在アクティブなConda環境のPython実行ファイルのパスを連携させる
```
cd ~/projects/comfyui-managed-env
poetry env use $(which python)
```

- 起動方法（Windows）
```
poetry run python "$(wslpath 'C:\Users\yoshi\OneDrive\Desktop\ComfyUI-master\main.py')"
```
- 起動方法（Linux）
```
poetry run python ~/ComfyUI-master/main.py
```

- poetry更新方法
```
cd ~/projects/comfyui-managed-env
poetry lock
poetry export -f requirements.txt --output requirements-lock.txt --without-hashes
cp requirements-lock.txt ../comfyui-docker/
```

- Docker起動方法
```
cd ~/projects/comfyui-docker
docker build -t comfyui-docker-image .
docker run -d -p 8188:8188 --gpus all --name comfyui-container comfyui-docker-image

```
