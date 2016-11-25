# ratingbarview

<img width="1193" alt="2016-11-25 3 13 36" src="https://cloud.githubusercontent.com/assets/5822929/20617104/d13b8eb6-b321-11e6-82dd-330c14b9a4a7.png">

```xml
<com.young.widget.RatingBarView
    android:id="@+id/rating_bar"
    android:layout_width="wrap_content"
    android:layout_height="wrap_content"
    android:layout_alignParentBottom="true"
    android:layout_marginStart="70dp"
    rating:starCount="5"
    rating:starEmpty="@drawable/icon_star_off"
    rating:starFill="@drawable/icon_star_on"
    rating:starImageSize="16dp"
    rating:starClickable="false"
    />
```

```java
//设置 高亮星星数量
ratingBar.setStar(entry.stars, false);
ratingBar.setOnRatingListener(new RatingBarView.OnRatingListener() {
    @Override
    public void onRating(Object bindObject, int RatingScore) {
        //点击回调
    }
});
```




Step 1. Add the JitPack repository to your build file

Add it in your root build.gradle at the end of repositories:
```dsl
    allprojects {
        repositories {
            ...
            maven { url "https://jitpack.io" }
        }
    }
```
Step 2. Add the dependency
```dsl
    dependencies {
            compile 'com.github.wjehovah:ratingbarview:-SNAPSHOT'
    }
```
一个简单的评分view 上传到 jitpack方便使用，[代码来自 eclipse_xu](http://www.jianshu.com/p/06c321b7f19b)，感谢原作者
