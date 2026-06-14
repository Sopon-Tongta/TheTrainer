[
  React Native
  รูปแบบ: SinglePage
  แบบ: FullCode
  default-function: App
  without: KeyboardAvoidingView, TouchableWithoutFeedback, SafeAreaView
  view-code: <<โค้ด return View ของ App เรา>>
]: ปรับเป็นธีม สีฟ้า

ตัวอย่าง 

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