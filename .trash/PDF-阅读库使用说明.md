# 如果你想直接使用这个库去阅读你的PDF文件
你可以参考[这个视频](https://www.bilibili.com/video/BV1gi421v7QN/?spm_id_from=333.999.0.0)里演示的操作去进行使用。

# 如果你想把这个库里的PDF标注功能迁移到你自己的OB库里
你可以参考[这个视频](https://www.bilibili.com/video/BV1ox4y147tZ/?spm_id_from=333.999.0.0)去进行操作。

# 如果你想对不同的PDF文件设置不同的标记标签

你可以参考[这个视频](https://meeting.tencent.com/crm/NgWnJO6N37)从1小时03分开始的演示操作去进行相关的设置。

其中你需要使用的模板是：

```javascript
### {{moment().format("YYYYMMDDHHmmss")}}

{{color !== "" ? "#" : ""}}{{color == "yellow" ? properties.yellow : ""}}{{color == "red" ? properties.red : ""}}{{color == "note" ? properties.note : ""}}{{color == "important" ? properties.important : ""}}{{color == "alert" ? properties.alert : ""}}
{{text}}

{{linkWithDisplay}}
```
