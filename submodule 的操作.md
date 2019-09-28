
1、一个项目中包含子tag时的操作：
```
1、给主项目打tag：
     git tag -a Publish_v3.2.1 -m "Publish_v3.2.1"
2、给submodule 打tag：
     git submodule foreach git tag -a Publish_v3.2.1 -m "Publish_v3.2.1"
3、检查submodule 打tag情况：
     git submodule foreach git tag
4、提交submodule 打的tag：
      git submodule foreach git push origin Publish_v3.2.1
5、提交主项目tag：
      git push origin Publish_v3.2.1
```