# Homework_codecamp_8
### JavaScript Exercise Arrow Function
ธนกฤต ชัยวานิชกุล

แปลง function ข้างล่างให้อยู่ในรูป arrow function
```
function ask(question, yes, no) {
  if (confirm(question)) yes()
  else no();
}

ask(
  "Do you agree?",
  function() { alert("You agreed."); },
  function() { alert("You canceled the execution."); }
);
```
แปลงเป็น
```
let ask = (question, yes, no) => {
  if (confirm(question)) yes()
  else no();
}

let agree = () => alert("You agreed.")

let cancel = () => alert("You canceled the execution.")

ask("Do you agree?", agree, cancel);
```
