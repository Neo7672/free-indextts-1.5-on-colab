# IndexTTS on Colab
use IndexTTS for free on google colab. 

这里将包含 IndexTTS 系列的 Google Colab 笔记本，最开始的一个版本是 1.5 。


## IndexTTS 2.0 固定版本（推荐）

[在 Colab 打开 IndexTTS 2.0 固定版](https://colab.research.google.com/github/Neo7672/free-indextts-1.5-on-colab/blob/main/index-tts-2.0-pinned-on-colab.ipynb)

选择「运行时 → 更改运行时类型 → T4 GPU」，然后从上到下运行。最后打开输出中的 `gradio.live` 链接使用。

原来的 2.0 笔记本默认下载官方最新提交，因此可能安装到 IndexTTS 2.5。这个新版本固定：

- 官方代码：[`v2.0.0` / `830f6f8f94a51fea23ab1d639027a86200075a4e`](https://github.com/index-tts/index-tts/tree/830f6f8f94a51fea23ab1d639027a86200075a4e)。
- 主模型：[`IndexTeam/IndexTTS-2` / `258515cc44cee99d5b9694a67ee194ffd8a3e618`](https://huggingface.co/IndexTeam/IndexTTS-2/tree/258515cc44cee99d5b9694a67ee194ffd8a3e618)。
- Python 3.11、uv 0.8.22、官方 `uv.lock` 中的依赖；默认 FP16，不启用 DeepSpeed 或自定义 CUDA 编译。

安装目录为 `/content/index-tts-2.0-pinned`，与旧目录隔离。辅助模型沿用官方首次启动下载逻辑。启动前自动检查代码版本、包版本、主模型版本及 GPU。

如果之前装过 2.5，先保存音频，再断开连接并删除旧运行时，用新运行时运行本笔记本。Colab 免费 GPU 的可用性、配额由 Google 决定；分享链接用完应关闭。

已完成静态检查，尚未在真实 Colab GPU 上完成端到端语音生成验证。

## 原有笔记本

[原版 IndexTTS 2 笔记本（随官方最新提交变化，不锁定 2.0）](https://colab.research.google.com/github/Neo7672/free-indextts-1.5-on-colab/blob/main/index-tts-2-on-colab.ipynb)

[在 Colab 上免费使用 IndexTTS 1.5](https://colab.research.google.com/github/Neo7672/free-indextts-1.5-on-colab/blob/main/index-tts-1.5-on-colab.ipynb)
