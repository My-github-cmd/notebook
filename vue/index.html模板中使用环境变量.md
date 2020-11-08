# 在index.html文件中使用环境变量（可以查看vue-cli官方文档：HTML和静态资源文件 ==> index文件
    
![模板文件使用环境变量](./image/模板文件使用环境变量.png "模板文件使用环境变量")

* 首先在.env.XXX文件中定义一个变量：需要使用VUE_APP_为开头命名一个变量：如 VUE_APP_NAME

* 在vueindex.html模板文件中使用：<%= VUE_APP_NAME %>  如：<link href="<%= VUE_APP_NAME %>"></link> {boolen:<%= VUE_APP_NAME %>} (注意：这里只有一个等号)