# 2025/06/20
- ComfyUI-KJNodes, comfyui-manager, ComfyUI-VideoHelperSuite, rgthree-comfyについて、poetry.tomlに記述完了

# 2025/06/19
- ComfyUI, ComfyUI_essentials, ComfyUI_MagicClothingについて、poetry.tomlに記述完了

# 2025/06/15 ~ 2025/06/18
- 依存関係を解決中
- poetryのセットアップ

# 2025/06/11 ~ 2025/06/14
- ComfyUI_MagicClothingの__init__とnodesのコードの理解

# 2025/06/10
- mssをmambaでインストールを検証中

# 2025/06/08
- ComfyUIおよびcoustom_nodesのrequirements.txtを全て、mamba・conda・pipに整理完了

# 2025/06/05
- Poetryのインストール（依存関係管理）
- ComfyUI_MagicClothingのrequirements.txtの中で、conda-forgeのものを選別する -> mamba(or conda)で1つずつインストールしていく

# 2025/06/04
- Poetryのインストール（依存関係管理）
- ComfyUI_MagicClothingのrequirements.txtの中で、conda-forgeのものを選別する -> mamba(or conda)で1つずつインストールしていく

# 2025/06/03
- tritonのインストール（すでにインストール済み）

# 2025/06/02
- WSL (Ubuntu) 環境でMambaをインストール
- ComfyUIのセットアップ
    - 使用するライブラリをmamba（condaより高速）とcondaでインストール
    - mambaにないものを選別して、pipでインストール

# 2025/06/01
- wslでLinux環境で全て作り直す（やり直し）
- wsl上のLinuxディストリビューション（ubuntuターミナル）にanaconda（miniconda3）をインストール
- 仮想環境の設定（comfyui_wsl_env）

# 2025/05/31
- minicondaのインストール
- 2025/05/30の続き

# 2025/05/30 
ComfyUI: Changed from portable version to ZIP version
- conda環境で仮想環境を構築する
- conda環境でinsightfaceをインストールする
- Reinstall everything

# 2025/05/29 
ComfyUI: Install custom nodes from GitHub, Install Cython, Install Visual Studio C++ BuiInstall 
- Cython
- ComfyUI_MagicClothing
- ComfyUI_MagicClothing\requirements.txtを修正（バージョンが古いためコメントアウト）
    - #torch==2.1.1+cu118
    - #torchvision==0.16.1+cu118
- Visual Studio C++ Build Tools
  
# 2025/05/28
ComfyUI: Install LoRA, Model from PixAI
- Street art style（LoRA）
- Aüngir（Model）
  
# 2025/05/27
ComfyUI: Install custom nodes from GitHub
- ComfyUI_essentials
- ComfyUI-VideoHelperSuite
- ComfyUI-KJNodes
- rgthree-comfy
  
# 2025/05/25
ComfyUI: Install custom nodes from GitHub, install xformers
- Pytorchをアンインストール→再インストール（CPU版をGPU版にするため）
- xformersをCUDA 12.8を指定してインストール
- Comfyui-managerインストール




