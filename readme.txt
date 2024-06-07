1,首先确认GitHub是否开启Action。开启方法Setting=>Action=>General=>选择Allow all actions and reusable workflows然后Save
2,在secrets添加变量。Setting=>Secrets and variables=>Actions=>New repository secret
	GITEE_PRIVATE_KEY : Gitee ssh 共有密钥对应的私有密钥也就是.ssh/id_ras文件里面的内容
	GITEE_TOKEN : Gitee私人令牌 设置=>私人令牌 生成新令牌（复制关闭后不能再查看，最好保存起来）
	GITEE_USER : Gitee用户名，就是个人主页昵称下面@后面的内容
3,在.github/workflows/目录下创建sync2gitee.yml文件，将本仓库下的yml内容复制到sync2gitee.yml文件，提交就ok了