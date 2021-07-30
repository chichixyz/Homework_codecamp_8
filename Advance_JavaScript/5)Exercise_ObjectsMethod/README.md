# Homework_codecamp_8
### Advance JavaScript Exercise Methods ของ Object
ธนกฤต ชัยวานิชกุล

Exercise Methods ของ Object
1.การทำงานของ code ดังกล่าวจะได้อะไรออกมา
> 'John'

2.การทำงานของ code ดังกล่าวจะได้อะไรออกมา
> ''

3.สร้าง object calculator จาก 3 methods นี้:
- read() ใช้ prompts สำหรับรับค่ามา 2 ค่าและเก็บเป็น object properties.
- sum() คืนค่าผลบวกของ 2 ค่านั้น.
- mul() คืนค่าผลคูณของ 2 ค่านั้น.
```
calculator = {
  read() {
    this.x = Number(prompt('please input the 1st value'))
    this.y = Number(prompt('please input the 2nd value'))
  },
  sum() {
    return this.x + this.y
  },
  mul() {
    return this.x * this.y
  }
}
```

4.ให้ Object ชื่อ ladder มี method ขึ้น และ ลง
- Object ชื่อ ladder สามารถเรียก function แบบนี้ได้
- ดัดแปลง Object ชื่อ ladder สามารถเรียก function แบบนี้ได้
```
let ladder = {
  step: 0,
  up() {
    this.step++;
    return this
  },
  down() {
    this.step--;
    return this
  },
  showStep() { 
    alert( this.step );
    return this
  }
};
```
