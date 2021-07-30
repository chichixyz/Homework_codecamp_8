# Homework_codecamp_8
### Advance JavaScript Exercise Array
ธนกฤต ชัยวานิชกุล

1.ผลลัพธ์ของความยาว array คืออะไร
> 4

2.ให้ทำตามขั้นตอนต่อไปนี้
- สร้าง array ชื่อ styles ที่มี items ชื่อ “Jazz” และ “Blues”
- เพิ่ม “Rock-n-Roll” ต่อท้าย
- นำค่า Classics ไปทับค่าตรงกลางของ Array
- นำ items ตัวแรกออกมาและลบ items ตัวนั้นออกจาก array
- เพิ่ม “Rap” และ “Reggae” ไปข้างหน้าของ Array
```
styles = ['Jazz', 'Blues']
styles.push('Rock-n-Roll')
styles[1] = 'Classics'
styles.shift()
styles.unshift('Rap', 'Reggae')
```

3.เขียนฟังก์ชัน sumInput() ที่
- ใช้ propmt รับ value มาเก็บใน array
- หยุดถามเมื่อเจอค่าที่ไม่ใช่ ตัวเลข
- คำนวณผลรวมของตัวเลขทั้งหมดใน Array
```
function sumInput() {
  let arr = []
  while(true) {
    let input = prompt('please input a number')
    if (isNaN(input)) break;
    arr.push(Number(input))
  }
  let sum = 0
  for (n of arr) {
    sum += n
  }
  return sum
}
```
