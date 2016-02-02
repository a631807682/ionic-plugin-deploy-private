兼容／非兼容二进制版本更新

使用方式: cordova plugin add https://github.com/a631807682/ionic-plugin-deploy-private.git

注意事项：

1.www.zip压缩的是platform目录下的www文件内容

2.二进制版本更新中ios/android的www文件是不同的

3.配合https://github.com/a631807682/ionic-service-deploy-private.git使用

后端数据格式：

1.更新检测地址: {{host}}/update/check/:app_id
2.请求数据格式：{ 
	  device_app_version: '',
	  device_deploy_uuid: '',
	  device_platform: '',
	  channel_tag: '' 
  }
3.返回数据格式{
     compatible_binary: true, //是否兼容二进制版本
     update_available: true, //是否有更新
     update: {
                uuid:'', 
                url: ''
             }
  }




