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
#### 9.Sanawdaky her bir sözüň uzynlygyny görkez.
```

let s = 'Atajan Alijanow';
let s1 = '';
let k = 0;
s = s + ' ';
for ( let i = 0; i < s.length; i++){
    if(s[i] != ' '){
        s1 = s1 + s[i];
    } else {
        k++
        console.log(k,' nji sozink uzunlygy',s1.length);
        s1 = '';
    }
}

```
#### 10.Eger setiriň uzynlygy > 5 bolsa, soňky 3 nyşany aýyr.
```

let s = 'atajan';
let s1 = '';
if(s.length > 5){
    for ( let i = 0; i < s.length - 3 ; i ++){
        s1 = s1 + s[i];
    }
} else {
    console.log(s);
}
console.log(s1);

```
#### 11.Setiriň ilkinji harpyny görkez.
```

let s = '12-081!@#Ztajan alijanow';
for ( let i = 0; i < s.length; i++){
    if (((s[i].codePointAt(0) >= 65) && (s[i].codePointAt(0) <= 90)) ||
        ((s[i].codePointAt(0) >= 97) && (s[i].codePointAt(0) <= 122)))
    {
        console.log(s[i]);
        return
    }
}

```
#### 12.Soňky harpyny al.
```

let s = '12-081!@#Ztajan alijanow';
let c = '';
for ( let i = 0; i < s.length; i++){
    if (((s[i].codePointAt(0) >= 65) && (s[i].codePointAt(0) <= 90)) ||
        ((s[i].codePointAt(0) >= 97) && (s[i].codePointAt(0) <= 122)))
    {
        c = s[i];
    }
}
console.log(c);

```
#### 13.3-nji indeksdäki nyşany al.
```

let s = '213=-3123!@$$ atajan alijanow';
console.log(s[2]);

```
#### 14.Sözleriň sanawyndan her biriniň ilkinji harplaryndan täze setir döret.
```

let s = '294 0-= 3120 #$@% atajan alijanow'; 
let s1 = '';
let s2 = '';
s = s + ' '; 
for ( let i = 0; i < s.length; i++ ){
    if(s[i] != ' '){
        s1 = s1 + s[i];
    } else {
        s2 = s2 + s1[0];
        s1 = '';
    }
}
console.log(s2);

```
#### 15.Nyşanlaryň Unicode kodlarynyň jemi.
```

let s = 'atajan';
let jem = 0;
for ( let i = 0; i < s.length; i++){
    jem = jem + s[i].codePointAt(0);
}
console.log(jem);

```
#### 16.Setiriň her ikinji harpyny al.
```

let s = 'atajan alijanow';
let s1 = '';
let s2 = '';
s = s + ' ';
for (let i = 0; i < s.length; i++){
    if(s[i] != ' '){
        s1 = s1 + s[i];
    } else {
        s2 = s2 + s1[1];
        s1 = '';
    }
}
console.log(s2);

```
#### 17.Setiri tersine ýaz (harp boýunça).
```

let s = 'atajan';
let s1 = '';
for ( let i = 1; i < s.length+1; i++){
    s1 = s1 + s[(s.length)-i];
}
console.log(s1);

```
#### 18.Diňe täk sanly indeksdäki harplardan setir döret.
```

let s = 'atajan alijanow';
let s1 = '';
for (let i = 0; i< s.length;i++){
    if(i % 2 != 0) {
        s1 = s1 + s[i];
    }
}
console.log(s1);

```
#### 19.Unicode kodlaryny 1 artdyryp şifrle.
```

let s = 'atajan alijanow';
let s1 = '';
for (let i = 0; i < s.length; i++){
    s1 = s1 + String.fromCodePoint(s[i].codePointAt(0)+1);
}
console.log(s1);

```
