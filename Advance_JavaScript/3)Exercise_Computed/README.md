# Homework_codecamp_8
### Advance JavaScript Exercise Computed Properties
ธนกฤต ชัยวานิชกุล

1.ให้เขียนโปรแกรมที่รับค่า key และ value ของ Properties ของ Object หนึ่ง จนกว่าจะเจอคำว่า stop และนำค่าเหล่านั้นมาสร้าง Object หลังจากนั้น console.log() object นั้นออกมา

```
let obj = {};

while (true) {
  theKey = prompt('please insert the key');
  if (theKey === 'stop') break;
  theValue = prompt('please insert the value for '+ theKey);
  if (theValue === 'stop') break;
  obj[theKey] = theValue
}


console.log(obj)
```


2.ให้เขียนโปรแกรมที่รับค่า key และ value ของ Properties ของ Object หนึ่ง โดยให้ key เป็นชื่อของผลไม้ และ value เป็นจำนวนของผลไม้ (number) โดยถ้า ผลไม้ชนิดไหนที่มีมากกว่า 1 ผล ให้เติม s ไปหลัง key นั้นด้วย

```
let fruit = {};

while (true) {
  fruitName = prompt('please insert the fruit name');
  if (fruitName === '') break;
  theAmount = Number(prompt('please insert the amount of '+ fruitName));
  if (theAmount > 1) {
    fruitName += 's'
  };
  fruit[fruitName] = theAmount
}

console.log(fruit)
```
