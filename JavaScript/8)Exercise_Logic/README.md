# Homework_codecamp_8
### JavaScript Exercise ตัวดำเนินการแบบตรรกะ
ธนกฤต ชัยวานิชกุล

1. คำสั่งต่อไปนี้จะแสดงค่าเป็นอะไร

alert( null || 2 || undefined );
> 2

alert( alert(1) || 2 || alert(3) );
> 2

alert( 1 && null && 2 );
> null

alert( alert(1) && alert(2) );
> 1

alert( null || 2 && 3 || 4 );
> 3

2. เขียนคำสั่ง if ที่เช็คอายุว่าอยู่ระหว่าง 18 - 60
```
let age = Number(prompt("what is your age?"))

if (age >= 18 && age <= 60){
  console.log("Your age is between 18 - 60")
}
```

3. เขียนคำสั่ง if ที่เช็คอายุว่าไม่อยู่ระหว่าง 18 - 60
```
let age = Number(prompt("what is your age?"))

if (age < 18 || age > 60){
  console.log("Your age is not between 18 - 60")
}
```

4. คำสั่ง alert ไหนที่จะถูกรันบ้าง

if (-1 || 0) alert( 'first' );
> run

if (-1 && 0) alert( 'second' );
> doesn't run

if (null || -1 && 0) alert( 'third' );
> doesn't run


5. ให้เขียนระบบ login
- ให้ใช้ prompt ในการถามใครเป็นคน login
- ถ้าผู้ใช้กรอกว่า “Admin” ให้ใช้ prompt ถาม password
- วิธีเช็ค Password
- ถ้า string นั้นเป็น “codecamp#5” ให้ alert “ยินดีต้อนรับ”
- ถ้า string เป็นอย่างอื่นให้ alert เป็น “Wrong password”
- ถ้าเป็น string ว่าง หรือ กด cancel ให้ alert ว่า “ยกเลิก”
- ถ้าผู้ใช้กรอกอย่างอื่นที่ไม่ใช่ “Admin” ให้ alert ว่า “ผมไม่รู้จักคุณ”
- ถ้าผู้ใช้กรอก input เป็น string ว่าง หรือกด Esc ให้ alert ว่า “ยกเลิก”

```
let username
let password

username = prompt("Username")

if (username === "Admin") {
  password = prompt("Password")
    if (password === "codecamp#5") {
      alert("ยินดีต้อนรับ")
    } else if (password !== "codecamp#5" && password != null && password != "") {
      alert("Wrong password")
    } else {
      alert("ยกเลิก")
    }
  } else if (username !== "Admin" && username != null && username != "") {
   alert("ผมไม่รู้จักคุณ")
  } else {
  alert("ยกเลิก")
  }

```

