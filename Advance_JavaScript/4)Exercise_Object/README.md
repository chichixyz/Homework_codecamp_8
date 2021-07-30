Exercise Object

1.ให้ทำตามคำสั่งต่อไปนี้
- สร้าง Object เปล่าขึ้นมา
- เพิ่ม properties name เข้าไปและให้ value เป็น “Sonter”
- เพิ่ม properties surname เข้าไปและให้ value เป็น “Pakorn”
- เปลี่ยน properties name เป็น “Boy”
- ลบ properties name ออกจาก Object
```
let obj = {};
obj.name = 'Sonter'
obj.surname = 'Pakorn'
obj.name = 'Boy'

delete obj.name
```

2.ให้เขียนฟังก์ชันชื่อ isEmpty(obj) โดยจะมี parameters เป็น obj และ ฟังก์ชันนี้จะเช็คว่า obj นี้มี properties ไหม 
ถ้ามีให้คืนค่า false ถ้าไม่มีให้คืนค่า true
```
function isEmpty(obj) {
    for(let key in obj) {
        if(obj.hasOwnProperty(key))
            return false;
    }
    return true;
}
```

3.การเขียนข้างล่างต่อไปนี้ Error ไหม
> ไม่ Error

4.จงเขียนฟังก์ชัน sum(obj) ที่รับ obj ที่เก็บ properties โดยมี key เป็นชื่อพนักงานและมี value เป็นเงินเดือน 
ให้ฟังก์ชันคืนค่าเป็นผลรวมของเงินเดือนพนักงานทั้งหมด
```
function sum(obj) {
  let sum = 0;
  for (let x in obj) {
    sum += obj[x]
  }
  return sum;
};
```

5.จงเขียนฟังก์ชัน multiplyNumeric(obj, times) โดยถ้า properties นั้นมี value เป็น number 
ให้คูณ value นั้นด้วย times ถ้าข้อมูลเเป็นอย่างอื่นไม่ต้องทำอะไร"
```
function multiplyNumeric(obj, times) {
  for (let x in obj) {
    if (typeof obj[x] !== Number) continue; 
    obj[x] *= times
  }
}
```

