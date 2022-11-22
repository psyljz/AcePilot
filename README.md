# Orbiter 脚本

这个仓库包含一个在[Orbiter](https://www.orbiter.finance/)上进行跨链转账的脚本。

# 开始

## 环境准备

- [git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)
  - 安装完成后，可以尝试运行 `git --version` 正确安装的情况可以看到以下输出 `git version x.x.x`
- [Nodejs](https://nodejs.org/en/)
  - 安装完成后，尝试以下命令:
    - `node --version` 可以得到这样的输出: `vx.x.x`
- [Yarn](https://classic.yarnpkg.com/lang/en/docs/install/)
  - 可以尝试以下命令:
    - `yarn --version` 可以得到这样的输出: `x.x.x`
    
## 快速入门

```bash
git clone https://github.com/psyljz/orbiter-script
cd orbiter-script
yarn
```


# 运行脚本

1. 设置好环境变量

需要设置 `PRIVATE_KEY` ,`OP_RPC_URL` `BSC_RPC_URL`这3个环境变量.  在`.env.example`填写完毕后，把文件名更改为`.env`

- `PRIVATE_KEY`: 你账户的私钥 (比如[metamask](https://metamask.io/))。
  - 你可以在这里查看[如何在小狐狸钱包导出私钥](https://metamask.zendesk.com/hc/en-us/articles/360015289632-How-to-Export-an-Account-Private-Key)。
- `OP_RPC_URL`:  注册[Alchemy](https://alchemy.com/?r=0ede4fdf6cd368f9)获得Optimism的节点URL。
- `BSC_RPC_URL`:  在[QuickNode](https://www.quicknode.com/)获得BNB Smart Chain的节点URL。

2. 确保你在orbiter-script目录下
3. 执行 ./AceOpBSC.sh 10 60  
  - *第一个参数 **10** 代表执行的次数。* 
  - *第二个参数 **60** 代表两次转账之间间隔时间(单位为秒)。*




