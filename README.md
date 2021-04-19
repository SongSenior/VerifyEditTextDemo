# VerifyEditTextDemo

# 使用方法
```xml
<com.songsenior.verifyedittext.VerifyEditText
        android:id="@+id/vet1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:verify_count = "4"
        android:layout_marginTop="30dp"
        app:verify_inputType = "number"
        app:verify_password = "true"
        app:verify_width = "20dp"
        app:verify_height = "20dp"
        app:verify_password_visible_time = "500"
        app:verify_textSize = "14sp"
        app:verify_margin = "25dp"
        app:verify_background_normal = "@drawable/shape_verify_edittext_default_bg"/>
```
# 自定义属性

```xml
app:verify_count = "5"//验证码item个数
app:verify_width = "50dp"//单个 item 的高度
app:verify_height = "50dp"//单个 item 的宽度
app:verify_margin = "15dp"//item 间的间隔
app:verify_textSize = "15sp"//item 的字体大小
app:verify_textColor = "#ff00dd"//item 的文字颜色
app:verify_background_normal = "@drawable/shape_bottom_line_normal"//空背景
app:verify_background_selected = "@drawable/shape_bottom_line_selected"//输入值后的背景
app:verify_password = "true"//显示密文 true，显示明文 false
app:verify_password_visible_time = "200"//输入值200ms后变为密文显示
app:verify_inputType = "none"//使用方式和 EditText 的 inputType 一样
```
# 项目依赖

## 1在根 build.gradle上添加maven

```groovy
allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}
```

## 2添加依赖
```groovy
dependencies {
	        implementation 'com.github.SongSenior:VerifyEditText:1.0'
	}
```
