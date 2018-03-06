## 注册github邮箱账号
$ git config --global user.name "leveno"  
$ git config --global user.email "857596898.com" 
### 生成ssh key 
cd ~/.ssh 
### 如果没有密钥： 
ssh-keygen -t rsa -C "857596898@163.com" 
### 把密匙复制到github  


## 把本地项目上传到github  
mkdir Test  
cd Test  
echo "# myweb" >> README.md  
git init  
git add README.md  
git commit -m "first commit"  
git remote add origin https://github.com/leveno/myweb.git  
git push -u origin master    
