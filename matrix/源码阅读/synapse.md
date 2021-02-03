#####synapse开发环境搭建
1.synapse 开发语言 python/twisted


##### pycharm调试环境搭建
- 运行下面语句生成配置文件
````
# Create the homeserver.yaml config once
python -m synapse.app.homeserver \
  --server-name my.domain.name \
  --config-path homeserver.yaml \
  --generate-config \
  --report-stats=[yes|no]

# Start the app
python -m synapse.app.homeserver --config-path homeserver.yaml
````
- pycharm如何传入命令行参数
  入口在synctl.py 文件，在这个文件下右键，调试。点edit configuratios-->Parameters 输入start

###synape 项目工程遇到的问题
1. 安装 twistd 包遇到 系统平台不支持的错误，解决：export ARCHFLAGS="-arch x86_64"
2. yaml 包安装 pip install pyyaml