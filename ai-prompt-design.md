# React Native Prompt Template

ใช้ Template ด้านล่างสำหรับสร้างหน้าจอ React Native แบบ Single Page และ Full Code

## รูปแบบมาตรฐาน

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ ???
```

---

## Parameters

| Parameter        | Value                                                        |
| ---------------- | ------------------------------------------------------------ |
| Framework        | React Native                                                 |
| รูปแบบ           | SinglePage                                                   |
| แบบ              | FullCode                                                     |
| Default Function | App                                                          |
| Without          | KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView |
| Start Layout     | View                                                         |
| Theme            | general                                                      |

---

## ตัวอย่างการใช้งาน

### 1. หน้าจอ Login

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ Login
```

### 2. หน้าจอรายการพนักงาน

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ รายการพนักงาน
```

### 3. หน้าจอรายการสินค้า

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ รายการสินค้า
```

### 4. หน้าจอ Dashboard

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ Dashboard
```

### 5. หน้าจอ Profile

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  start-layout: View
  theme: general
]: Desige หน้าจอ Profile
```

---

## หมายเหตุ

* สร้างโค้ด React Native แบบ Full Code พร้อมใช้งาน
* ใช้ Function Component ชื่อ `App`
* เริ่มต้น Layout ด้วย `View`
* ไม่ใช้:

  * `KeyboardAvoidingView`
  * `TouchableWithoutFeedback`
  * `SafeAreaView`
* ออกแบบ UI ตาม Theme ที่กำหนด (`general`)
* โค้ดต้องสามารถนำไปใช้ใน Expo Snack หรือ React Native Project ได้ทันที
