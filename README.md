# HLuseEditor

#### 介绍
HLuseEditor是一款基于Bootsrap所见即所得富文本web编辑器，支持手机触屏，具有轻量，使用便利，易扩展，多语言支持，注重用户体验等特点。
HLuseEditor是 **HLuse** 的一个小功能，独立出来开放使用，得益于Bootsrap的支持，全程序只有两个JS文件共约 **20K** 。


#### 使用前提
1. Bootsrap5环境；
2. 引入Bootsrap图标[https://icons.getbootstrap.com/](https://icons.getbootstrap.com/)；
3. 需支持 **Popper** 
#### 安装教程

1.  引入JS：
`<script src="HLuseEditor.min.js"></script>`
2.  初始化：
`HLE.init('editorid')`
3.  在需要地方创建HTML模板：

```
<textarea name="editorid" id="editorid"  style="display: none;" >初始化文本</textarea>
<div id="editorid_editor"><div><div id="editorid_editor_menu"><div class="btn-group btn-group-sm me-1 my-1">自定义工具(非必须可省略)</div></div></div></div>
```

#### 使用说明

1.  获取HTML: HLE.getHtml();
2.  获取文本: HLE.getText();
3.  插入HTML：HLE.insertText(html);

#### 关于自定义

1.  自定义工具按钮的样式参考 Bootstarp 的 btn-group组件；
2.  点击自定义按钮触发你自定义的事件，然后组织成你想要插入或者替换的html,最后调用HLE.insertText(html);

#### 特色

1.  所有功能支持手机触屏操作，但是由于手机上无法完成选择字段所以有些功能不太方便（建议手机上只开启必须功能）；
2.  大部分功能（包括你自定义）支持源码模式下编辑；
3.  支持EXCEL片段转表格（合并在表格功能）；
4.  未额外引用一个任何style文件，所以你所编辑几乎是99%实际表现；
5.  脱程式自定义，你无需关心程序本身，只需要明确你要插入/替换什么；最后调用HLE.insertText(html);
6.  更多使用方法见文档中心：[https://doc.hl05.com/hluseeditor](https://doc.hl05.com/hluseeditor)
