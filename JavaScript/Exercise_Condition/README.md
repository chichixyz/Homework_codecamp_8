Exercise การเขียนเงื่อนไข

1.Browser จะโชว์ข้อความ “Hello Codecamp #5” ไหม
> โชว์ เพราะ "0" เป็นค่าใน string = True

2.ใช้ if else ในการเขียนถามชื่อของคุณ
- ถ้าตอบถูกให้แสดงคำว่า “เก่งมาก”
- ถ้าตอบผิดให้แสดงคำว่า “คุณไม่รู้จักชื่อฉัน”

```
let myName = prompt("ฉันชื่ออะไร")
let message
message = (myName === "ธนกฤต")? "เก่งมาก" : "คุณไม่รู้จักชื่อฉัน"
alert(message)
```

3.ใช้ prompt ในการรับคะแนนมาคำนวณเกรด
- ถ้าคะแนน มากกว่าเท่ากับ 80    ได้ A
- ถ้าคะแนน อยู่ระหว่าง 70 - 79     ได้ B
- ถ้าคะแนน อยู่ระหว่าง 60 - 69     ได้ C
- ถ้าคะแนน อยู่ระหว่าง 50 - 59     ได้ D
- ถ้าคะแนน น้อยกว่า 50            ได้ F

```
let studentScore = Number(prompt("What is the student score?"))

if (studentScore >= 80) {
    alert("grade : A")
  } else if (studentScore >= 70) {
    alert("grade : B")
  } else if (studentScore >= 60) {
    alert("grade : C")
  } else if (studentScore >= 50) {
    alert("grade : D")
  } else {
    alert("grade : F")
  }
```

4.เปลี่ยน if-else ข้างล่างในอยู่ในรูปของ Ternary Operators
```
let age = Number(prompt("how old are you?"))
let price
price = (age < 18)? 2000:3500;
```

