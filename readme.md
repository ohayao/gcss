# gcss 全局样式
> 使用less 生成
> 图标引用了 font awesome http://cdn.bootcss.com/font-awesome/4.7.0/css/font-awesome.min.css

### 色彩
1. default <font color="#ccc">默认灰色</font>
2. black  <font color="#000">黑色</font>
3. success  <font color="#28a745">绿色</font>
4. warn <font color="#ffc107">黄色</font>
5. danger <font color="#dc3545">红色</font>
* 可以定义前景色（font color g-txt-{color}）
* 可以定义背景色（background color g-bg-{color}）

### 通用
`.fl 左浮动 .fr 右浮动`

## 1.模块 g-block-{color}
``` css
display: block;
border: none;
padding: 5px 5px 5px 5px;
overflow: hidden;
```
``` html
<div class="g-block">
    Hello world
</div>
```
## 2. 栅格，宽度
> 默认为12等分
#### 1. 无边距 `表格:g-col-{1,12}  宽度:g-w{1,12}`
#### 2. 有边距 `表格:g-cols-{1,12}  宽度:g-ws{1,12}` 默认边距 `0.5%`
#### 3. 偏移 `无边距:g-col-offset-{1,12} 有边距:g-cols-offset-{1,12}`

## 3. 表单
> 单选框、复选框设置了颜色，其它暂无设置
- g-input 文本框
- g-textarea 多行文本框
- g-input-file 文件框
- g-select
- g-radio-{color} 单选框
- g-radio-{color} 复选框
``` html
<input class="g-input" type="text" placeholder="输入框" />

<input class="g-input" type="password" placeholder="密码输入框" />

<textarea class="g-textarea" placeholder="输入内容"></textarea>

<label class="g-input g-input-file"><input type="file" /></label>

<div class="g-input-file" style="border:solid 3px #eee;border-radius: 5px;width:100px;height:100px; text-align: center;padding-top:18px;color:#999">
    <i class="fa fa-upload" style="font-size:64px;width:64px;height:64px;"></i>
    <input type="file" />
</div>

<select class="g-select"><option value="0">请选择</option></select>
<!--单选框、复选框-->
<label class="g-check"><input type="checkbox" name="name1" value="0" />A</label>
<label class="g-check"><input type="checkbox" name="name1" value="1" />B</label>

<label class="g-check-danger"><input type="checkbox" name="sex" value="0" checked />男</label>
<label class="g-check-danger"><input type="checkbox" name="sex" value="1" />女</label>
```
## 4. 按钮 g-btn-{color}-{size} 链接 g-link-{color}
> 按钮支持大中小 按钮内可以嵌套font awesome图标
``` html
<button class="g-btn-default-s">小按钮</button>
<button class="g-btn-black">正常按钮</button>
<button class="g-btn-danger">大按钮</button>
<span class="g-btn-success-s">小按钮</span>
<span class="g-btn-warn"><i class="fa fa-home"></i>正常图标按钮</span>
<a class="g-btn-warn"><i class="fa fa-bars"></i>正常图标按钮</a>

<a class="g-link-danger">danger link</a>
<a class="g-warn-danger">warn link</a>
```
## 5. 表格 g-table-{color}
> 配合 thead tbody tfoot
- 行背景，单元格背景滑过变色
- g-noborder 无边框
``` html
<table class="g-table-black">
    <thead>...</thead>
    <tbody>...</tbody>
    <tfoot>...</tfoot>
</table>
```
## N. todo