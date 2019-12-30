# fabric-vue

vue中调用fabric.js模块

通过webpack引用,npm 安装 git 仓库的协议：

        <protocol>://[<user>[:<password>]@]<hostname>[:<port>][:][/]<path>[#<commit-ish> | #semver:<semver>]


####引用方式webpack
1. pachage.json的dependencies中添加依赖
2. 依赖具体写法，以下两种
      - "fabric": "git://github.com/fabricjs/fabric.js.git#v2.7.0"
      - "fabric": "2.7.0"
      
      
####webpack 安装测试  

- npm install -g cnpm --registry=http://registry.npm.taobao.org   
- cnpm install -g node-gyp 
- cnpm i git+https://username:password@github.com/fabricjs/fabric.js.git#v2.7.0
- cnpm i git+https://username:password@github.com/mvphjx/fabric-vue.git#master
    
 cnpm install执行结果

    √ All packages installed (1107 packages installed from npm registry, 
    2 packages installed from git, 
    used 9m(network 9m), speed 3.96kB/s, json 960(2.16MB), tarball 0B)

 npm install执行结果
 
    偶尔成功过一次，很慢，无测试结果
 
    
    

