# Chatbot Commit

Chatbot Commit是一个Git钩子，它使用ChatGPT根据提交中的更改生成提交消息。

## 使用方法

1. 将 `pre-commit` 文件复制到你的Git仓库的 `.git/hooks` 目录下。

2. 在提交更改时，使用 `git commit -m "任意文本"` 命令进行提交,脚本将替换`-m`内容且提供一个简短的描述更改的消息。Hook 将使用 ChatGPT 生成的消息。
  
3. 用于hoo 

## API

该项使用的是免费API，个人使用不会有问题。如果需要大量使用，请自行搭建云函数，并将`fvusmj86xf.hk.aircode.run`修改为自己的云函数地址。

### 云函数
项目中使用的云函数是基于[aircode](https://aircode.cool),点击[这里](https://aircode.cool/ut7f58ea34)搭建,请修改`Environments->OPENAI_KEY`.![git仓库chatcommit云函数key](https://jsdelivr.nodream.cf/gh/1802024110/GitHub_Oss@main/img/git仓库chatcommit云函数key.png)

## 许可

该项目基于 MIT 许可证。有关详细信息，请参阅 LICENSE 文件。

测试文本123