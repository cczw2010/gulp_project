##前端工程自动化

本资源是利用gulp实现的前端资源压缩合并的集成包，没有自己发布npm包，直接修改的gulp包生成环境，方便自己做前端工程使用。

下载完成压缩包解压后，在压缩包根目录下（package.json所在目录）执行：`npm install` 安装所有依赖包（好像不少。。）

安装完成后直接运行：`gulp`执行默认测试工程（demos中是测试工程目录结构），配置自己的工程可以修改`gulpfile.js` 当然也可以建立多个`gulpfilexxxx.js`工程文件，运行`gulp --gulpfile gulpfilexxxx.js`来执行指定的工程


##目录结构

		目录说明（一下的目录如果不是默认的，那么请修改gulpfile.js中各自的目录地址）
		+ src 目录为所有的源码目录
				↳ html 静态html文件目录
				↳ css css源码文件目录
					↳ concat 要合并压缩的css文件全放在这个目录，其下所有文件将生成一个文件
					...
				↳ js	 js源码文件目录
					↳ concat 要合并压缩的js文件全放在这个目录 ，其下所有文件将生成一个文件
					...
				↳ json	 json文件源码目录（一般用于接口测试json）
				↳ image	通用图片目录（会进行简单的压缩）
		+ dist 目录为默认处理过的文件目录
				↳ html 处理过的html目录
				↳ js 处理过的js目录
				↳ css 处理过的css目录
				↳ json 处理过的json目录
				↳ image 处理过的image目录

