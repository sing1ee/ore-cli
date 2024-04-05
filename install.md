# 下载代码
## 如果有 git，则
```shell
# 首先
git clone https://github.com/sing1ee/ore-cli.git
# 进入项目目录，执行切换分支
git checkout fast
```

## 如果没有 git，则
![image](https://github.com/sing1ee/ore-cli/assets/1057882/286fbf4c-5653-469b-959a-42828a4345a2)
1. 先切换到 fast 分支
2. 下载 zip

这样我们得到了源代码

# 编译

## 安装 rust

## mac & linux 
```shell
curl https://sh.rustup.rs -sSf | sh
```

## windows
[查看文档](https://juejin.cn/post/7219656530235670588)


## 进行编译
进入代码的目录，执行
```shell
# mac & linux & windows
cargo build --release

```

# 执行
可执行文件一在项目目录下的 ***target/release***，在 mac 和 linux 上是 ore，windows 是 ore.exe
```shell
bash run.sh "./ore --rpc rpc地址 --keypair id 文件路径 --priority-fee 1100 mine -t 4
我是多开的，同时用 run.sh 自动重启
# run.sh 代码如下：

https://github.com/sing1ee/ore-cli/blob/fast/run.sh
```

# 注意
1. 基本思路是：多多尝试，尝试越多，收益就越高。
2. 可以多开，一个程序对应一个 rpc
4. 因为实现思路和官方的不同，稳妥的还是跑官方的，想尝试下效率的，可以试试。
5. 官方的合约也会更新，不保证更新即时。

# 我的提交记录
![image](https://github.com/sing1ee/ore-cli/assets/1057882/0aca2a9d-1a33-407d-ba9e-0fc3c9f92a6d)

