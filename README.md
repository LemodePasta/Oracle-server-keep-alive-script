# Oracle Server Keep-Alive Script 说明

fork 自 :contentReference[oaicite:0]{index=0}

实测 wget 网速没有效果，借助 AI coding 进行调试修改。

---

## 功能说明

- 选项 1：安装  
- 选项 2：卸载  
- 选项 3：更新安装引导脚本  
- 选项 4：退出脚本  

---

## 使用说明

- 安装过程中如果无脑回车，则所有可选占用功能都会开启  
- 如不需要占用功能，输入 `n` 再回车即可  
- 如果选择带宽占用，会提示选择：
  - 使用 speedtest-go 占用
  - 或使用 wget 占用  
  按提示选择即可  
- 是否需要自定义带宽占用参数：
  - 默认选项为 `n`（直接回车使用默认配置）
  - 输入 `y` 后按提示自定义参数  

---

## 带宽占用参数说明

- 参数代表实际消耗带宽
- AI 建议范围：5 ~ 20 Mbps
- 已加入随机波动机制：
  - 带宽：±50%
  - 周期：±10 分钟
  - 持续时间：±3 分钟

---

## 一键安装命令

```bash
curl -L "https://raw.githubusercontent.com/LemodePasta/Oracle-server-keep-alive-script/main/oalive.sh?v=4" -o oalive.sh && chmod +x oalive.sh && bash oalive.sh
