# Homework_codecamp_8
### JavaScript Exercise Switch Cases
ธนกฤต ชัยวานิชกุล

จงเขียน method draw(int n) ให้ print ออกมาในกรณีที่ n มีค่าต่างๆ ได้ผลลัพธ์ดังนี้

1.
```
        function draw(n) {
            let result = ""
            let i = 0
            while (i < n) {
                i++;
                result = result + "*";
            }
            console.log(result)
        }
```
2.
```
        function draw(n) {
            let result = ""
            let newLine = ""
            for (let i = 0; i < n; i++) {
                result = result + "*";
            }
            for (let x = 0; x != n; x++) {
                newLine += result + "\n"
            }
            console.log(newLine)
        }
```
3.
```
        function draw(n) {
            let result = ""
            let newLine = ""
            for (let i = 0; i < n; i++) {
                result += (i + 1)
            }
            for (let x = 0; x != n; x++) {
                newLine += result + "\n"
            }
            console.log(newLine)
        }
```
4.
```
        function draw(n) {
            let result = ""
            for (let i = 1; i <= n; i++) {
                for (let x = 0; x != n; x++) {
                    result += i
                }
                result += "\n"
            }
            console.log(result)
        }
```
5.
```
    function draw(n) {
        let result = ""
        for ( let i = n; 1 <= i; i--) {
                for ( let x = 0; x != n; x++) {
                result += i
            } 
            result += "\n"
            } console.log (result)
        }
```
6.
```
    function draw(n) {
        let result = "";
        for (let i = 1; i <= (n**2); i++) {
            result += i;
            if (i % n == 0) {
                result += "\n";
            }
        } console.log (result)
    }
```
7.
```
    function draw(n) {
        let result = ""
        for ( let i = (n**2); i >= 1; i--) {
            result += i;
            if (i % n == 1) {
                result += "\n";
            }
        } console.log (result)
    }
```
8.
```
    function draw(n) {
        let result = ""
        for ( let i = 0; i < n*2; i++) {
            if ( i % 2 == 0 ) {
            result += i;
            } else ( result += "\n")
        } console.log (result)
    }
```
9.
```
    function draw(n) {
        let result = ""
        for ( let i = 1; i <= n*2; i++) {
            if ( i % 2 == 0 ) {
            result += i;
            } else ( result += "\n")
        } console.log (result);
    }
```
10.
```
    function draw(n) {
        let result = ""
        for ( let i = 0; i < n; i++) {
            for (let row = 1; row <= n; row++) {
                result += (row + (i * row));
            } result += "\n";
        } console.log (result)
    } 
```
11.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = 1; i <= n; i++) {
                for (let x = 1; x <= n; x++) {
                    if (i == x) {
                        result = "_";
                    } else {
                        result = "*";
                    } compare += result;
                } compare += "\n"
            } console.log (compare)
        }
```
12.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = 1; i <= n; i++) {
                for (let x = n; x >= 1; x--) {
                    if (i == x) {
                        result = "_";
                    } else {
                        result = "*";
                    } compare += result;
                } compare += "\n"
            } console.log (compare)
        }
```
13.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = 1; i <= n; i++) {
                for (let x = 1; x <= n; x++) {
                    if (i < x) {
                        result = "_";
                    } else {
                        result = "*";
                    } compare += result;
                } compare += "\n"
            } console.log (compare)
        }
```
14.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = 1; i <= n; i++) {
                for (let x = n; x >= 1; x--) {
                    if (i > x) {
                        result = "_";
                    } else {
                        result = "*";
                    } compare += result;
                } compare += "\n"
            } console.log (compare)
        }
```
15.
```
    function draw(n) {
        let combine = "";
        let result;
        for(let row = 1; row <= n; row++) {
            for(let column = 1; column <= n; column++) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result
            }
            combine += "\n";
        };
        for(let row = n-1; row >= 1; row--) {
            for(let column = 1; column <= n; column++) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result
            }
            combine += "\n";
        };
        console.log(combine)
    }

```
16.
```

```
17.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = 1; i <= n; i++) {
            for (let x = n; x >= 1; x--) {
                if (i < x) {
                    result = "_";
                } else {
                    result = "*";
                } compare += result
            } compare += "\n";
        } console.log (compare)
    }
```
18.
```
    function draw(n) {
        let compare = "";
        let result;
        for (let i = n; i >= 1; i--) {
            for (let x = n; x >= 1; x--) {
                if (i < x) {
                    result = "_";
                } else {
                    result = "*";
                } compare += result
            } compare += "\n";
        } console.log (compare)
    }
```
19.
```
    function draw(n) {
        let combine = "";
        let result;
        for(let row = 1; row <= n; row++) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result
            }
            combine += "\n";
        }
        for(let row = n - 1; row >= 1; row--) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result
            }
            combine += "\n";
        }
        alert(combine)
    }
```
20.
```
     function draw(n) {
        let combine = "";
        let result;
        let num = 1;
        for(let row = 1; row <= n; row++) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof result != "number") continue;
                num++
            }
            combine += "\n";
        }
        for(let row = n - 1; row >= 1; row--) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof result != "number") continue;
                num++
            }
            combine += "\n";
        }
        console.log(combine)
    }
```
21.
```
    function draw(n) {
        let combine = "";
        let result;
        for(let row = 1; row <= n; row++) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            for(let column = 2; column <= n; column++) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            combine += "\n"
        }
        console.log(combine)
    }
```
22.
```
    function draw(n) {
        let combine = "";
        let result;
        for(let row = 1; row <= n; row++) {
            for(let column = 1; column <= n; column++) {
                if(row <= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            for(let column = n-1; column >= 1; column--) {
                if(row <= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            combine += "\n"
        }
        console.log(combine)
    }
```
23.
```
    function draw(n) {
        let combine = "";
        let result;
        for(let row = 1; row <= n; row++) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            for(let column = 2; column <= n; column++) {
                if(row >= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            combine += "\n"
        }
        for(let row = 2; row <= n; row++) {
            for(let column = 1; column <= n; column++) {
                if(row <= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            for(let column = n-1; column >= 1; column--) {
                if(row <= column) {
                    result = "*";
                }else {
                    result = "-";
                }
                combine += result 
            }
            combine += "\n"
        }
        console.log(combine)
    }

```
24.
```
    function draw(n) {
        let combine = "";
        let result;
        let num = 1;
        for(let row = 1; row <= n; row++) {
            for(let column = n; column >= 1; column--) {
                if(row >= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof result != "number") continue;
                num++ 
            }
            for(let column = 2; column <= n; column++) {
                if(row >= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof result != "number") continue;
                num++ 
            }
            combine += "\n"
        }
        for(let row = 2; row <= n; row++) {
            for(let column = 1; column <= n; column++) {
                if(row <= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof result != "number") continue;
                num++ 
            }
            for(let column = n-1; column >= 1; column--) {
                if(row <= column) {
                    result = num;
                }else {
                    result = "-";
                }
                combine += result
                if(typeof star != "number") continue;
                num++
            }
            combine += "\n"
        }
        console.log(combine)
    }
```
