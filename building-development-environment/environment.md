# 安装完linux之后要做的事情


## 1.替换软件源
https://mirrors.tuna.tsinghua.edu.cn/help/ubuntu/

C和C++ 环境搭建：
Ubuntu默认并没有安装开发环境（也就是没有gcc和g++），所以我们需要自己装。
但是一个个装比较麻烦，幸好Ubuntu提供了一个build-essential软件包，这个软件包中就又gcc和g++，还有make，可以满足我们的需要。
build-essential软件包的安装方法是，打开命令终端，输入如下命令：
sudo apt-get install build-essential


## 2.安装新得立软件包管理器（Synaptic）
http://people.ubuntu.com/~happyaron/udc-cn/lucid-html/ch06s07.html
(替换软件源)


## 3.安装网页浏览器Chromium


## 4.安装oh-my-zsh，配置 ~/.zshrc
简单介绍：https://learnku.com/laravel/t/5790/ultimate-terminal-zshautojump

https://www.bilibili.com/video/av8079095?from=search&seid=2017415412797081005 (Getting Started with ZSH (and oh my zshell) on Ubuntu)
https://www.bilibili.com/video/av24622273?from=search&seid=2017415412797081005 (ubuntu配置ZSH ，美化terminal 。)


## 5.安装搜狗输入法for linux

## 6.安装截图软件Shutter


## 7.编辑器：
 1. https://www.sublimetext.com/3    Linux repos   （按照自己常用的插件和配置来配好）
 2. https://code.visualstudio.com/#alt-downloads   （按照自己常用的插件和配置来配好,比如code runner插件）



## 8.python 环境搭建：
https://www.anaconda.com/distribution/
(在~/.zshrc配置环境变量，之后 source ~/.zshrc)


## 9.Java环境搭建：
ubuntu安装Oracle Java
(在~/.zshrc配置环境变量，之后 source ~/.zshrc)

## 10.Git环境：
https://gist.github.com/derhuerst/1b15ff4652a867391f03#file-linux-md
sudo apt-get update
sudo apt-get upgrade
sudo apt-get install git

Git可视化客户端：
https://www.syntevo.com/smartgit/download/



## 11.Mysql数据库:
https://blog.sunriseydy.top/technology/server-blog/server/ubuntu-18-04-install-mysql/
可视化Mysql数据库客户端：mysql workbench ubuntu


## 12.笔记软件
应该选择哪一个呢？




# 后续的思考：
## 1.如何在 VSCode 里面安装code runner插件？
## 2.如何在 VSCode 里面使用code runner插件来运行下述的C++代码(斐波那契数列)？

``` C++
#include <iostream>
 
int main()
{
        unsigned int a = 1, b = 1;
        unsigned int target = 48;
        for(unsigned int n = 3; n <= target; ++n)
        {
                unsigned int fib = a + b;
                std::cout << "F("<< n << ") = " << fib << std::endl;
                a = b;
                b = fib;
        }
 
        return 0;
}
```



## 3. 如何在 VSCode 里面使用code runner插件来运行下述的Python代码(斐波那契数列)？

``` Python
x,y=0,1

while y<10000:
    print(y)
    x,y = y,x+y
```



## 4.如何在 VSCode 里面使用code runner插件来运行下述的Java代码(斐波那契数列)？
(或者使用其他的eclipse之类的)


``` Java
public class FibonacciList {

  public static void main(String[] args) {
    for (int i = 0; i < 30; i++) {
      System.out.println(recFibN(i));
    }
  }

  public static long recFibN(final int n) {
    return (n < 2) ? n : recFibN(n - 1) + recFibN(n - 2);
  }
}
```
