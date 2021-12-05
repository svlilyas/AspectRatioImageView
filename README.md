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

## Attributes

<table>
    <tr>
        <th>Attribute</th>
        <th>Description</th>
        <th>Default</th>
    </tr>
    <tr>
        <td><b>ari_ratio</b></td>
        <td>Should define float value of <b>height/width</b> which for<br/> 16:9 aspect ratio is <b>9/16</b> = <b>5.5625</b><br/>
        Should define one of <b>width</b> or <b>height</b> <b>0dp</b> and other<br/> <b>match_parent</b>, <b>wrap_content</b> or <b>exact value</b> like <b>120dp</b>.
       </td>
        <td>-</td>
    </tr>
   <tr>
        <td><b>radius</b></td>
        <td><b>DP</b> value for corner radius</td>
        <td><b>0dp</b></td>
    </tr>
    <tr>
        <td><b>corners</b></td>
        <td>There are <b>8 types</b> of different corners<br><br>
            <b>topLeft</b><br>
             makes top left corner defining radius value.<br>
            <b>topRight</b><br>
             makes top right corner defining radius value.<br>
           <b>bottomLeft</b><br>
             makes bottom left corner defining radius value.<br>
           <b>bottomRight</b><br>
             makes bottom right corner defining radius value.<br>
           <b>left</b><br>
             makes left corners defining radius value.<br>
           <b>right</b><br>
             makes right corners defining radius value.<br>
           <b>top</b><br>
             makes top corners defining radius value.<br>
           <b>bottom</b><br>
             makes bottom corners defining radius value.<br>
        </td>
        <td>all corners</td>
    </tr>
</table>
![This is an image](/app/src/main/res/drawable/img_2560x1440_16_9.png)
