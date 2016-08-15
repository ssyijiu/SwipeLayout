#SwipeLayout
侧滑删除，适用于任何View。

> Github上有一个非常著名的侧滑删除[daimajia/AndroidSwipeLayout](https://github.com/daimajia/AndroidSwipeLayout)，但是我在使用的时候发现了一些BUG。
> 其他的侧滑删除大都又是与ListView、RecyclerView耦合在一起，不适用于目前的项目，于是有了这个小巧简洁的SwipeLayout。

##项目原理
使用ViewDragHelper和ViewDragHelper.Callback完成一系列的侧滑动作。

##效果展示

##使用说明

###布局
布局分内容区域和删除区域，内容区域为正常展示数据的区域，删除区域是侧滑出来的区域。
```html
<com.ssyijiu.swipelayout.SwipeLayout
        android:id="@+id/swipelayout"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        >
        <!--内容区域-->
        <include layout="@layout/layout_content"/>

        <!--删除区域-->
        <include layout="@layout/layout_delete"/>

</com.ssyijiu.swipelayout.SwipeLayout>
```

## 联系作者
- Github: [ssyijiu](https://github.com/ssyijiu)
- E-mail: lxmyijiu@163.com
- WeChat: ssyijiu11

##License

```
Copyright 2016 ssyijiu

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```