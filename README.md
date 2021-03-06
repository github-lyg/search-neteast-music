 # 用NodeJS实现网略爬虫抓取网易云音乐用户评论

### 项目说明
(http://www.jianshu.com/p/6923210ce8ee/)

### 平台介绍
- win10（我用的是win10，当然win7等应该也是可以的）

- Node版本是6.10.0（可以到Node中文网去下载最新的稳定版本     (http://nodejs.cn/)  安装方式如下：
    + 方法1：下载之后直接傻瓜式的“下一步”就好了。
    + 方法2：采用nvm在线安装，这需要你先安装nvm（node版本管理工具，安装它时需要配置环境变量）打开命令行输入`nvm install 6.10.0 `它就会自动在线安装了。安装完成之后输入命令`nvm use 6.10.0`这时就切换到6.10.0版本了。此时你输入`node -v`和`npm -v`命令后如果都能通过就表示你已经成功安装并能正常使用了。这种方式虽然麻烦但是可以同时安装不同版本的Node，只需要使用`node use x.x.x`就可以在不同版本中切换了。同时你也可以使用`node list`打印出你电脑上的所有的node版本。这里不再赘述，相关资料网上很多。

- 控制台，要执行我们的代码需要在控制台输入命令，我这里使用的是win10自带的powershell，在项目根目录下按住shift再点击鼠标右键你就会看到它了。当然你也可以用cmd命令行，不过你要定位到项目根目录。（这里发现一个小问题，powershell可输出的行数是有一定的限制的，行数太多就不能输出了，不知道是不是因为我电脑是win10预览版的原因）

- 确保你的网络畅通，没网你玩个什么

- 代码里要做很多错误优先处理函数，我都没做，不可能保证健壮性。只是玩玩。遇到问题就直接`Ctrl + c`退出就好了。

### 使用步骤

1. 将项目克隆到本地（需要git环境，没有你就直接下载压缩包吧）命令行输入：
    ```bash
    git clone https://github.com/havenxie/webcrawler-neteast-music.git webcrawler-neteast-music 
    
    cd webcrawler-neteast-music
    ```
    上面的webcrawler-neteast-music就是你项目的名称，你可以自己换一个，不过不建议用中文。

2. 在项目根目录下打开控制台

3. 控制台输入命令
    ```bash
    node neteast-music.js
    ```
    这样程序就跑起来了，结束之后会在项目根补录下生成data.json文件。这就是抓到的数据。如果你想在控制台直接看到所有数据就把代码的第9行`const logSwitch = false;`的false改为true就好了。

4. 切记不要干坏事，这个Demo用来玩一下就好了。

5. 对了你用`cls`命令可以清空控制台。

## 许可

[MIT](./LICENSE) &copy; [havenxie](http://github.com/havenxie)
