# Homework_codecamp_8
### Advance JavaScript Exercise Code
ธนกฤต ชัยวานิชกุล

1. แก้ไขการเขียนโค้ดต่อไปนี้
```
function pow(x,n)
{
  let result=1;
  for(let i=0;i<n;i++) {result*=x;}
  return result;
}
let x=prompt("x?",''), n=prompt("n?",'')
if (n<=0)
{
  alert(`Power ${n} is not supported, please enter an integer number greater than zero`);
}
else
{
  alert(pow(x,n))
}
```
แก้เป็น
```
function pow(x,n) {
  let result=1;
  for(let i=0;i<n;i++) result*=x;
  return result;
};

let x=prompt("x?",'');
let n=prompt("n?",'');

if (n<=0) {
  alert(`Power ${n} is not supported, please enter an integer number greater than zero`);
} else {
  alert(pow(x,n))
};
```
