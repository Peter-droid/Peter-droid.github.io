# Hexo工作目录

## 如何使用

写作命令
新建分页：hexo new page 名称
新建文章：hexo new 名称或hexo n 名称
新建草稿：hexo new draft 名称或hexo n draft 名称
草稿生成文章：hexo publish 名称或hexo p 名称
草稿生成分页：hexo publish page 名称或hexo p page 名称
操作命令
清除已生成文件：hexo clean
运行本地服务器（预览）：hexo s
运行本地服务器（预览草稿）：hexo s --drafts
生成静态文件：hexo g
部署到服务器：hexo d
生成并部署文件：hexo g -d或hexo d -g
常见事项
多标签：

tags: 
- 标签1
- 标签2
或tags: 【标签1,标签2】

设置阅读全文
方法一：在文章中使用<!-- more -->手动进行截断，Hexo 提供的方式（推荐）
方法二：在文章的 front-matter 中添加 description，并提供文章摘录
方法三：自动形成摘要，在 主题配置文件 中修改：

auto_excerpt:
  enable: true
  length: 150
默认截取的长度为 150 字符，可以根据需要自行设定

建议使用<!-- more -->（即第一种方式），除了可以精确控制需要显示的摘录内容以外， 这种方式也可以让 Hexo 中的插件更好的识别。
