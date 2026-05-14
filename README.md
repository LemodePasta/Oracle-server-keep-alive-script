fork自https://github.com/LemodePasta/Oracle-server-keep-alive-script
实测wget网速没有效果，借助AI coding进行调试修改。
说明
选项1安装，选项2卸载，选项3更新安装引导脚本，选项4退出脚本
安装过程中无脑回车则全部可选的占用都占用，不需要什么占用输入n再回车
如果选择带宽占用，会询问使用speedtest-go占用还是使用wget占用，按照提示进行选择即可
有询问是否需要带宽占用的参数自定义，这时候默认选项就是n，回车就使用默认配置，输入y再回车则需要按照提示自定义参数
带宽占用参数代表实际消耗的带宽，AI建议5~20（单位Mbps）即可，另外加入了周期随机±10min波动，持续时间±3min波动，下载速度±50%波动。
curl -L "https://raw.githubusercontent.com/LemodePasta/Oracle-server-keep-alive-script/main/oalive.sh?v=4" -o oalive.sh && chmod +x oalive.sh && bash oalive.sh

