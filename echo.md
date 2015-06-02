# echo

## 语法

```sh
echo [short-option]... [string]...
```

## 用途

输出文本

## 主要选项

`-n` 末尾不输出**新行符（newline）**，默认情况下是输出的

`-e` 开启转义字符，默认情况下是不进行转义的

## 行为模式

echo 将各个参数打印到标准输出，参数之间以一个空格隔开，并以新行符（换行符）结束。

它会解释各个字符串里的**转义序列（escape sequences）**。转义序列可用来表示特殊字符，以及控制其行为模式。

## 警告

无

## 例子

** 正常输出 **

```sh
$ echo hello world
hello world
$ echo 'hello world'
hello world
```

** 开启转义输出 **

```sh
$ echo 'hello\n world\n'
hello\n world\n
$ echo -e 'hello\n world\n'
hello
 world

$ 
```
