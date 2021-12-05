# AspectRatioImageView
**AspectRatioImageView** has abilities like give images **aspect ratio** and **corner radius**.

To get a Git project into your build:

## Implementation 
**Step 1.** Add the JitPack repository to your build file

```
allprojects {
   repositories {
      ...
      maven { url 'https://jitpack.io' }
   }
}
```
**Step 2.** Add the dependency

```
dependencies {
   implementation 'com.github.svlilyas:AspectRatioImageView:1.0'
}
```
## Using

```
<com.svlilyas.aspectratioimageview.AspectRatioImageView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_margin="20dp"
        android:src="@drawable/img_2560x1440_16_9"
        app:ari_ratio="0.5625"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
```

![This is an image](/app/src/main/res/drawable/img_2560x1440_16_9.png)
