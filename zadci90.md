####  "hello" setiriniň uzynlygyny görkez.
```

let s = 'hello';
console.log(s.length);

```
####  "  space  " setirinde näçe nyşan bar?
```

let s = ' space ';
let k = 0;
for ( let i = 0; i < s.length; i++){
    if (!(((s[i].codePointAt(0) >= 48)&&(s[i].codePointAt(0) <= 57)) ||
        ((s[i].codePointAt(0) >= 65) && (s[i].codePointAt(0) <= 90)) ||
        ((s[i].codePointAt(0) >= 97) && (s[i].codePointAt(0) <= 122))
    ))
    {
        k++
    }
}
console.log(k);

```
#### Ulanyjynyň girizen setiriniň uzynlygyny al.
```

let s = 'Atajan';
let a = s.length;
console.log(a);

```
#### Setir boşmy diýip barla (length === 0).
```

let s = '';
if( s.length === 0) {
    console.log('true');
} else {
    console.log('false');
}

```
