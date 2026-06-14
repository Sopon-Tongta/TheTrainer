# React Native UI Theme Prompt

ใช้ Template นี้สำหรับให้ AI ปรับแต่งหน้าจอ React Native ที่มีอยู่แล้ว ให้เป็นธีมสีตามที่ต้องการ โดยส่งเฉพาะโค้ดภายใน `return View` ของ Component

---

## รูปแบบมาตรฐาน

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  view-code: <<โค้ด return View ของ App เรา>>
]: ปรับเป็นธีม สีฟ้า
```

---

## Parameters

| Parameter        | Description                                                  |
| ---------------- | ------------------------------------------------------------ |
| React Native     | ใช้ React Native                                             |
| รูปแบบ           | SinglePage                                                   |
| แบบ              | FullCode                                                     |
| default-function | App                                                          |
| without          | KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView |
| view-code        | โค้ดภายใน return ของ Component                               |
| Theme            | ธีมที่ต้องการ เช่น สีฟ้า, สีเขียว, สีม่วง, Dark Mode         |

---

## ตัวอย่างการใช้งาน

### Input

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  view-code: <View>
      <Text>
        Create Task
      </Text>

      <TextInput
        placeholder="ชื่องาน"
      />

      <TextInput
        placeholder="รายละเอียด"
      />

      <TouchableOpacity style={styles.createBtn}>
        <Text>
          Create
        </Text>
      </TouchableOpacity>

      <TouchableOpacity>
        <Text>
          Back to list
        </Text>
      </TouchableOpacity>
  </View>
]: ปรับเป็นธีม สีฟ้า
```

---

## Expected Result

AI จะ:

* ปรับ Layout ให้ดูทันสมัย
* ใช้โทนสีฟ้าเป็นหลัก
* เพิ่ม Shadow และ Border Radius
* ปรับ Typography ให้อ่านง่าย
* ปรับ Button ให้โดดเด่น
* ปรับ TextInput ให้ดูสวยงาม
* ส่งกลับเป็น Full Code พร้อม Styles ครบถ้วน
* สามารถนำไปใช้ใน Expo Snack ได้ทันที

---

## Theme Examples

### สีฟ้า

```text
]: ปรับเป็นธีม สีฟ้า
```

### สีเขียว

```text
]: ปรับเป็นธีม สีเขียว
```

### สีม่วง

```text
]: ปรับเป็นธีม สีม่วง
```

### Dark Mode

```text
]: ปรับเป็น Dark Theme
```

### Modern Corporate

```text
]: ปรับเป็นธีม Modern Corporate
```

### Glassmorphism

```text
]: ปรับเป็นธีม Glassmorphism
```

---

## Rules

* ส่งกลับเป็น React Native Full Code
* ใช้ Function Component ชื่อ App
* ห้ามใช้ KeyboardAvoidingView
* ห้ามใช้ TouchableWithoutFeedback
* ห้ามใช้ SafeAreaView
* ปรับเฉพาะ UI และ UX
* สามารถเพิ่ม Style ได้ตามความเหมาะสม
* รองรับ Expo Snack
* เน้นความสวยงามและใช้งานได้จริง

```
```
