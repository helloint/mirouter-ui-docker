# mirouter-ui-docker

## 介绍
这是[mirouter-ui](https://github.com/Mirouterui/mirouter-ui)的docker壳, 只是为了方便部署在群晖NAS上.  
功能介绍请看原作者的B站视频 https://www.bilibili.com/video/BV1BF411f79J/?spm_id_from=333.999.0.0  
其实只需要`docker-compose.xml`, 因为`config.json`是可以在第一次启动时被自动创建.  

## 使用方法
1. 在NAS docker目录下创建一个文件夹, 可以叫“mirouter”, 放入`docker-compose.xml`
2. 打开Container Manager, 创建项目(Create), 路径(Set Path)选择你刚才创建的目录.
3. 会提示你是否用该目录下的`docker-compose.xml`构建, 选“是”.
4. 项目名就填“mirouter”
5. 其他选项一路Next
6. 如果你之前没创建`config.json`, 第一次启动后会自动停止, 然后你需要手动更新`config.json`, 加上自己的路由器密码, 然后重启.

## 参数说明
* `maxsaved` 最多存储的记录条数
