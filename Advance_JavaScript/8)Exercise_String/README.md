# Homework_codecamp_8
### Advance JavaScript Exercise String
ธนกฤต ชัยวานิชกุล

1.เขียนฟังก์ชัน ucFirst(string) โดยทำคืนค่าเป็น string เดิม แต่ตัวแรกของ string กลายเป็นพิมพ์ใหญ่
```
function ucFirst(string) {
  return string[0].toUpperCase() + string.slice(1)
}
```

2.เขียนฟังก์ชันที่ checkSpam โดยถ้าข้อความดังกล่าวมีคำว่า “xxx” หรือ “viagra” ให้คืนค่าเป็น true ถ้าไม่มีให้คืนค่าเป็น false
```
function checkSpam(string) {
  if (string.includes('xxx') || string.includes('viagra')) {
    return true
  } else return false
}
```

3.เขียนฟังก์ชันที่ truncate(str, maxlength) โดยฟังก์ชันดังกล่าวจะเช็คว่า string 
ที่ถูกส่งเข้ามามีความยาวเกิน maxlength ไหม ถ้าเกินให้แทน ข้อความต่อจากนั้นด้วย “...”
```
function truncate(str, maxlength) {
  if(str.length > maxlength) {
    str = str.slice(0, maxlength) + '...';
  }
  return str
}
```

4.เขียนฟังก์ชันที่ extractCurrencyValue(string, rate) โดยที่ฟังก์ชันดังกล่าวจะแปลง string ที่เป็นค่าเงิน dollar 
ให้เป็น number ที่มีค่าเป็นเงินบาทไทย โดยอ้างอิง  rate จาก parameters ตัวที่สอง ที่ส่งมาให้
```
function extractCurrencyValue(string, rate) {
  return Number(string.replace(/[^0-9]/g, '')) * rate
}
```
