
## git submodule

#### 为项目添加 git submodule

    git submodule add git@example.com:bar.git  [foo/bar]  //默认放到 /submodule项目名 下

#### clone一个带git submodule的项目

    git clone 主项目路径
    
    git submodule init
    git submodule update
    
> 这两条命令可以合并为

    git submodule update --init
  
#### 更新submodule代码
    
    git submodule update
    
#### 移除submodule

  删除比较麻烦
  
    vim .git/config   //删掉submodule部分
    
    git rm -rf --cached foo/bar
    rm -rf foo/bar
    rm .gitmodules
