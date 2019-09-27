

https://marketplace.visualstudio.com/items?itemName=nonoroazoro.syncing


1、Settings Sync是vscode中同步设置和安装插件的小工具，在老电脑和新电脑的vscode的扩展商店中搜索并安装它
2、在老电脑上登陆Github>Your profile> settings>Developer settings>personal access tokens>generate new token，随便输入一个名称， 比方叫A，勾选Gist，提交
3、保存Github Access Token
4、打开老电脑上的vscode，Ctrl+Shift+P打开命令框，输入sync，找到update/upload settings，输入Token（就是在github上生成的那串字符），上传成功后会返回Gist ID，保存此Gist ID.
5、若想在新电脑上同步老电脑的vscode配置，同样，在新电脑中，Ctrl+Shift+P打开命令框，输入sync，找到Download settings，会自动跳转到Github的Token编辑界面，点Edit，regenerate token，保存新生成的token，在vscode命令框中输入此Token，回车，再输入之前在老电脑上操作生成的的Gist ID（之前老电脑操作完成可以在老电脑的 vscode的setting中看到一个配置叫sync.gist，我们复制它的值就可以了，不要引号），即可同步插件和设置。
