# Sublime Text3配置Node环境 #
## 在以下网址可以下载到sublim text3 node js的插件：[https://github.com/tanepiper/SublimeText-Nodejs。 ](https://github.com/tanepiper/SublimeText-Nodejs "node插件")  ##

## 使用方式如下: ##
* 解压zip文件， 务必重命名文件夹为“Nodejs”。 
 
* 在sublime的preferences->browse packages目录下放置刚才改名后的Nodejs文件夹。 

* 打开Nodejs文件夹，找到文件“Nodejs.sublime-build“，修改”encoding”: “cp1252”,为”encoding”: “utf-8”。
 
* 要用sublime打开文件“Nodejs.sublime-settings” 或者 设置preference ->package settings ->Nodejs ->setting-default 打开文件并 更改成以下代码    

    	{
    	// save before running commands
    	"save_first": true,
    	// if present, use this command instead of plain "node"
    	// e.g. "/usr/bin/node" or "C:\bin\node.exe"
    	"node_command": "D:\\nodejs\\node.exe",
    	// Same for NPM command
    	"npm_command": "D:\\nodejs\\npm.cmd",
    	// as 'NODE_PATH' environment variable for node runtime
    	"node_path": true,
    	"expert_mode": false,
    	"ouput_to_new_tab": false
    	}
**安装成功后，新建一个js文件，输入concole.log(“hello”)；然后使用Ctrl+b运行测试。如果在sublime的控制台输出hello则表示环境安装成功。**