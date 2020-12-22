第一次作业

GitHub存储库给用户提供的功能有很多，例如：项目代码托管、创建工作流、仓库安全、仓库配置等。我们小组主要对项目代码托管和仓库配置模块建立了功能用例图模型，以下是该用例模型的详细描述：
	
一、该用例模型的参与者有两个：user（用户）和system administrator（系统管理员）。

二、该用例模型的主要元素有两大块：Code（代码托管）和Settings（仓库配置）：

 Code

1.Code包含Add file（添加文件）、Update file（更新文件）、delete file（删除文件）、Go to file（查找本仓库文件）、search files（搜索网站源代码文件）、Fork（建立分支）、Pull requests（拉取请求）、Download file（下载文件）。

2.Add file又包含create new file（创建新文件）和Upload files（本地上传文件）；

3.Update file、delete file、Go to file又同时包含Add file；

4.Fork和Download又包含search files；

5.Pull requests又包含Fork；

6.Merge files（合并文件）又拓展于Pull requests；

Settings

1.Settings包含Create new repository（创建新的仓库）、Rename（重命仓库名）、GitHub Pages（GitHub页面管理）、Change repository visibility（变更仓库可见性）、Transfer ownership（转让所有权）、Archive repository（存档此仓库）、Delete repository（删除仓库）。

2.Rename、GitHub Pages、Change repository visibility、Transfer ownership、 Archive repository、Delete repository又同时包含Create new repository；

3.GitHub Pages又包含change theme（更换主题）、Custom domain（自定义域名）；

4.Change repository visibility又可以泛化为Make public（变为公共的）和Make private（变为私有的）两个子用例；
第二次作业

主要类图说明：
类名：Login
属性：username（用户名）和password（密码）
方法：login（登录）
功能：教师登录

类名：课件
属性：属性：课件名、主题、内容和作者
方法：发布课件、更新课件、删除课件、查看课件
功能：教师对课件进行操作，供学生查看学习

教师参与者共有六个类，其中课件类、视频类、教学心得类三个类分别依赖于登录类（login），关联与教师类。
