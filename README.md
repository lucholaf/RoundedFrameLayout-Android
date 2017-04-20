Download
--------
You can download a jar from GitHub's [releases page][1].

Use Gradle:

```gradle
dependencies {
    // RoundedFrameLayout
    compile 'com.github.QuarkWorks:RoundedFrameLayout-Android:0.2'
}
```
How do I use Glide?
-------------------
Configure radius in layout xml file:
```xml
    <com.quarkworks.roundedframelayout.RoundedFrameLayout
        android:id="@+id/refresh_button_container"
        android:layout_width="0dp"
        android:layout_height="match_parent"
        android:layout_weight="1"
        android:layout_margin="4dp"

        app:cornerRadiusTopLeft="10dp"
        app:cornerRadiusTopRight="20dp"
        app:cornerRadiusBottomLeft="20dp"
        app:cornerRadiusBottomRight="10dp"
        app:borderWidth="2dp">

        <!--sub views-->
        <ImageView
            android:id="@+id/refresh_button"
            android:layout_width="match_parent"
            android:layout_height="match_parent"

            android:src="@drawable/image_1"/>

    </com.quarkworks.roundedframelayout.RoundedFrameLayout>
```

Or configure radius in code:
```java
    //setCornerRadius() will set to four corners
    //refreshButtonContainer.setCornerRadius(20);

    refreshButtonContainer.setCornerRadiusTopLeft(10);
    refreshButtonContainer.setCornerRadiusTopRight(20);
    refreshButtonContainer.setCornerRadiusBottomLeft(20);
    refreshButtonContainer.setCornerRadiusBottomRight(10);
    refreshButtonContainer.requestLayout();
```