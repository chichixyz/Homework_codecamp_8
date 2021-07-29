# Homework_codecamp_8
### JavaScript Exercise การเขียนเงื่อนไข
ธนกฤต ชัยวานิชกุล

1.เลขที่ถูก alert เป็นลำดับสุดท้ายคือเลขอะไร
> 1

2.code ทั้งสองอันนี้จะแสดง alert ออกมาเหมือนกันทั้งหมดหรือไม่
> ไม่เหมือน

3.code ทั้งสองอันนี้จะแสดง alert ออกมาเหมือนกันทั้งหมดหรือไม่
> เหมือนกัน

4.ให้เขียน loop ทั้งแสดงเลข 2 ถึง 10 ออกมา
``` 
for (let i = 2; i <= 10; i++) {
  console.log(i)
}
```

5.เปลี่ยน code for loop ด้านล่างนี้ให้เป็น while loop โดยที่ผลลัพธ์ยังเหมือนเดิม
```
for (let i = 0; i < 3; i++) {
  alert( `number ${i}!` );
}
```
แปลงเป็น
```
let i = 0;
while (i < 3) {
  alert( `number ${i}!` );
  i++
};
```

6.ให้เขียนเกมส์ทายตัวเลขสำหรับเล่นสองคน โดย
- ให้ผู้เล่นคนแรกพิมพ์เลขใส่ใน prompt ที่อยู่ระหว่าง 1 ถึง 100 โดยไม่ให้ผู้เล่นคนที่สองรู้ว่าตัวเลขเป็นอะไร
- และให้ผู้เล่นคนที่สองทายเลขโดยการพิมพ์เลขใส่ใน prompt จนกว่าจะถูก ถ้าไม่ถูก จะต้องบอกด้วยว่าเลขที่ผู้เล่นคนที่สองพิมพ์เข้ามา มากกว่า หรือ น้อยกว่าคำตอบนั้น"
```
function  checkInputNumber() {
  while (true) {
    let x = prompt('player 1 : please enter the number between 1-100');
    if(Number(x) >= 1 && Number(x) <= 100) return x;
  };
};

let theNumber = checkInputNumber();

while (true) {
  let answer =  Number(prompt('player 2 : please guess the number'));
  if (answer == theNumber) {
    alert('you win!');
    break;
  } else if (answer < theNumber) {
    alert('the number is greater than your answer');
  } else {
    alert('the number is lesser than your answer');
  } 
};

```





