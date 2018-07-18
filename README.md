# trusteeship

*利用conda进行virtual environment的管理*
```bash
# 创建python2.7虚拟环境
conda create -n webenv python=2.7

# 开启
source activate webenv

# 关闭
source deactivate webenv
```

**Mac下可能遇到的问题：**
*python-magic在使用过程中，报如下错误：*
```bash
raise ImportError('failed to find libmagic. Check your installation')
ImportError: failed to find libmagic. Check your installation
```

*解决方法：*
```bash
brew install libmagic
cd your/conda/path/envs/webenv/lib
ls -n /usr/local/Cellar/libmagic/5.33/libmagic.dylib libmagic.dylib
```

