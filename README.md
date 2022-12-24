## The Legend of Mir 2
The Legend of Mir 2 is a sprite-based isometric three dimensional massively multiplayer online role-playing game. Players have the option of playing different professions. Taoist, healers who use magical abilities to summon pets to assist in battle, poison targets and heal allies. Warriors, who have the highest defense and attack attributes of all classes. Wizards depend on magic and can kill multiple monsters with ease using spells. Assassins have taken over as the primary melee damage dealing class but have much weaker defense attributes than warriors. Archers are a class of great accuracy and strength, using their powerful skills with bows to deal extraordinary damage from range.

## Crystal Source
The Legend of Mir 2 Crystal Source is a public repository hosted on GitHub that aims to develop a server and game client written in the programming language of C Sharp (C#).

## Installation
1. Install Microsoft Visual Studio with .NET Packages.
2. Download the latest source (https://github.com/Suprcode/mir2/releases).
3. Open the project and configure NuGet packages.

## Contributing
1. Fork the project hosted on GitHub (https://github.com/Suprcode/mir2).
2. Fix a bug or implement a new feature within your forked source.
3. Submit a pull request comparing to your forked source (https://github.com/Suprcode/mir2/compare).

## Guidance
For further information about server and game files visit the Legend of Mir Wikipedia (https://www.lomcn.org/wiki/index.php/Main_Page).

## Community
Legend of Mir Community Network (https://www.lomcn.org/forum/forumdisplay.php?633) is a forums website dedicated to everything related to The Legend of Mir. If you have a question related to running or developing a Legend of Mir server this is the best place to ask.

## Credits
- Far (Developer)
- Jamie (Developer)
- Public Contributions (https://github.com/Suprcode/mir2/graphs/contributors)

## License
Currently, there's no license for this project.

## 怎么运行
 1. 使用vs2019+ 编译
 2. 在Build\Client目录运行一下Client.exe 。如果无法运行，查看Error.txt里面提示: System.IO.FileNotFoundException: 未能加载文件或程序集“Microsoft.Web.WebView2.WinForms
    那么下载 https://github.com/Suprcode/mir2/releases 的 Stable.Release.2022.06.12.00.zip，把DirectX目录拷贝过来
 3. 运行一次之后，会在目录下产生配置文件 Mir2Test.ini, 修改里面 Host=http://mirfiles.com/mir2/cmir/patch/  为 Host=http://mirfiles.co.uk/resources/mir2/crystal/patch/ 
 4. 运行Client.exe，等待下载几个G的更新资源，完成后就可以运行客户端了
 5. 修改Mir2Test中的[Network]部分，UseConfig=True，下面添加
	IPAddress=127.0.0.1
	Port=7000
	主要是和本地服务器端口一致即可

 6. 客户端启动黑屏，安装directx sdk
	https://www.microsoft.com/en-US/download/confirmation.aspx?id=6812

 如果连接 https://github.com/Suprcode/mir2 的服务器那么需要注意，在服务器添加一些东西: 1) 需要添加Monster列表，否则无法启动 2)需要添加一个什么ore的道具，否则无法启动。参考 https://www.youtube.com/watch?v=jqEEkfj95-A
 如果连接 mirgo 服务器，使用本仓库修改过的mirgo代码即可，然后并下载 mir2ServerRelease， 新建 config.toml, 文件内容 DataPath="服务端资源绝对路径(mir2ServerRelease)" ，其他无需修改

