$ mkdir  resume && cd resume    ;;创建一个目录来操作
$ git init     ;;创建一个git库
$ git config  --global  user.name "your name"   ;;创建库的ownner，可选
$ git config --global user.email "your email"   ;;创建库的ownner 的email联系方式，可选


$ wget http://labfile.oss.aliyuncs.com/courses/624/cv-template.zip     ;;下载模板简历
$ unzip cv-template
$ mv cv-template/* .
$ rm -rf cv-template* __MACOSX*
$ git add .                             ;;追踪resume目录下的所有文件
$ git commit -m 'xzy resume'            ;;提交文件到本地仓库，-m是指定此次提交的message信息，自己改写
$ git remote add origin 远程仓库地址      ;;远程仓库地址，在创建好空的库时可以看见，图三中的https://github.com/xzy256/resume.git
$ git push -u origin master             ;;提交到远程操作
