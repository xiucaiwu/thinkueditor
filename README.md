停止维护，请慎用。

# Ueditor
this is a ueditor

## 安装

> composer require "xiucaiwu/thinkueditor"

## 删除

> composer remove xiucaiwu/thinkueditor

## 更新

> composer update xiucaiwu/thinkueditor

## 使用

```
//引入类库
use think\ueditor\Ueditor;
```

```
//添加ueditor方法
public function ueditor()
{
    $data = new Ueditor();
    echo $data->output();
}
```
## 视图

```
<script>
    $(function(){
        var ue = UE.getEditor('container',{
            serverUrl :"{:url('模块/控制器/ueditor')}",   // 调用的上面控制器里的方法
			initialFrameHeight:450		// 初始化高度
        });
    })
</script>
```

## 上传目录

默认上传至 public/uploads/ueditor 请确认目录存在。

目前仅支持TP5以上版本,不支持SAE平台。

## ueditor.zip

ueditor 1.4.3.3 版本 ,解压拷贝至public目录

```

<script src="{:url('/')}ueditor/ueditor.config.js"></script>
<script src="{:url('/')}ueditor/ueditor.all.min.js"></script>
<script src="{:url('/')}ueditor/lang/zh-cn/zh-cn.js"></script>

```