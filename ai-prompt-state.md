# React Native Prompt Template

## Requirement

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView

  view-code-page-1:
  <<โค้ด View ของหน้า 1>>

  view-code-page-2:
  <<โค้ด View ของหน้า 2>>

  requirement-page1: [
    req1: <<Requirement 1>>
    req2: <<Requirement 2>>
  ]

  requirement-page2: [
    req1: <<Requirement 1>>
    req2: <<Requirement 2>>
  ]
]: ขอรวม code ทั้งหมดแบบ FullCode เพื่อ Copy ไปใช้งาน
```

## Expected Output

- รวมโค้ดทั้งหมดเป็นไฟล์เดียว
- ใช้ `export default function App()`
- สร้าง State ให้ครบตาม Requirement
- สร้าง Function ที่เกี่ยวข้องให้ครบ
- สร้าง StyleSheet ให้ครบ
- สามารถ Copy ไปวางใน Expo Snack ได้ทันที
- ห้ามตอบเป็นบางส่วน
- ห้ามใช้ Placeholder Code
- ส่งผลลัพธ์เป็น Full Code เท่านั้น

---

# Example

## Input

```text
[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView

  view-code-page-1:
  <View style={{ flex: 1 }}>

    <View style={styles.header}>
      <Text style={styles.headerText}>
        Task List
      </Text>

      <TouchableOpacity style={styles.addBtn}>
        <Text style={styles.addBtnText}>
          Create
        </Text>
      </TouchableOpacity>
    </View>

    <FlatList
      data={tasks}
      keyExtractor={(item) => item.id}
      contentContainerStyle={{ padding: 10 }}
      renderItem={({ item }) => (
        <View style={styles.card}>
          <Text style={styles.title}>
            {item.name}
          </Text>

          <Text style={styles.detail}>
            {item.detail}
          </Text>

          <TouchableOpacity
            style={[
              styles.statusBtn,
              item.done ? styles.done : styles.todo,
            ]}>
            <Text style={styles.btnText}>
              {item.done ? 'Done ✓' : 'Mark Done'}
            </Text>
          </TouchableOpacity>
        </View>
      )}
    />
  </View>

  view-code-page-2:
  <View style={styles.createContainer}>

    <Text style={styles.headerText}>
      Create Task
    </Text>

    <TextInput
      style={styles.input}
      placeholder="ชื่องาน"
    />

    <TextInput
      style={styles.input}
      placeholder="รายละเอียด"
    />

    <TouchableOpacity style={styles.createBtn}>
      <Text style={styles.btnText}>
        Create
      </Text>
    </TouchableOpacity>

    <TouchableOpacity>
      <Text style={styles.backText}>
        Back to list
      </Text>
    </TouchableOpacity>

  </View>

  requirement-page1: [
    req1: ผูก state CurrentPage คลิ๊กปุ่ม Create ให้ไปหน้า 2
    req2: ผูก state FlatList เมื่อคลิ๊กปุ่ม Mark Done ในรายการ ให้ update ปุ่มเป็น Done
  ]

  requirement-page2: [
    req1: ผูก state TaskName กรณีพิมพ์ ชื่องาน
    req2: ผูก state TaskDescription กรณีพิมพ์ รายละเอียด
    req3: ผูก state FlatList คลิ๊กปุ่ม Create ให้เพิ่ม ชื่องาน และ รายละเอียด และกลับไปที่หน้า 1
    req4: ผูก state CurrentPage คลิ๊กปุ่ม Back to list ให้กลับไปที่หน้า 1
  ]
]: ขอรวม code ทั้งหมดแบบ FullCode เพื่อ Copy ไปใช้งาน
```