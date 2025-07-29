####  1."hello" setiriniň uzynlygyny görkez.
```

let s = 'hello';
console.log(s.length);

```
####  2."  space  " setirinde näçe nyşan bar?
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
#### 3.Ulanyjynyň girizen setiriniň uzynlygyny al.
```

let s = 'Atajan';
let a = s.length;
console.log(a);

```
#### 4.Setir boşmy diýip barla (length === 0).
```

let s = '';
if( s.length === 0) {
    console.log('true');
} else {
    console.log('false');
}

```
#### 5.Eger setir 10 nyşandan uzyn bolsa, diňe ilkinji 10 nyşany al.
```

let s = 'arzsdgxhfcvblkjn;m';
let s1 = '';
if(s.length > 10) {
    for ( let i = 0; i <=10; i++){
        s1 = s1 + s[i];
    }
} else { 
    console.log(s);
}
console.log(s1);


```
#### 6.Diňe 3 nyşandan uzyn setirleri massiwe goş.
```

let s = '1234567890---==$%^&%^%atajan';
let a = [];
let s1 = '';
let k = 0;
for (let i of s){
    s1 = s1 + i;
    if(s1.length == 3){
        k++
        a[k] = s1;
        s1 = '';
    }
}
for ( let i = 0; i <= k; i++){
    console.log(a[i]);
}

```
#### 7.Iki setiriň uzynlygyny deňeşdir.
```

let s = 'Atajan';
let s1 = 'Atajan';
if( s.length == s1.length ){
    console.log('den');
} else {
    console.log('den dal');
}

```
#### 8.Setiriň ýarysyna çenli (length / 2) gyrk.
```

let s = 'atajana';
let s1 = '';
if (s.length % 2 == 0){
    for (let i = 0; i < Math.floor( s.length / 2 ); i++){
        s1 = s1 + s[i];
    }
} else {
    for (let i = 0; i <= Math.floor( s.length / 2 ); i++){
        s1 = s1 + s[i];
    }
}
console.log(s1);


```
