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
#### 20.Indeksi 3-e bölünýän harplardan täze söz döret.
```

let s = 'atajan alijanow asxxx';
let s1 = '';
for ( let i = 0; i < s.length; i++){
    if( i % 3 == 0 ){
    s1 = s1 + s[i];
    }
}  
console.log(s1);

```
#### 21."apple" setirinde "a" bar diýip barla.
```

let s = 'apple';
for (let i = 0; i < s.length; i++){
    if(s[i] == 'a'){
        console.log('bar');
        return
    }
}
console.log('yok');

```
#### 22."hello" setirinde "lo"-nyň indeksini tap.
```

let s = 'hello';
console.log(s.indexOf('lo'));

```
#### 23."Hello" "He" bilen başlaýarmy?
```

let s = 'Hello';
if(s.indexOf('He') == 0){
    console.log('baslanyar');
} else {
    console.log('baslanmayar');
}

```
#### 24.Setir ".js" bilen gutarýarmy?
```

let s = 'zadaci24.js';
if(s.indexOf('.js') == s.length-3){
    console.log('gutaryar');
} else {
    console.log('gutarmayar');
}

```
#### 25."hello" setirinde "l"-iň iň soňky indeksini tap.
```

let s = 'hello';
for (let i = 0; i < s.length; i++){
    if(s[i] == 'l'){
        k = i;
    }
}
console.log(k);

```
#### 26.Ulanyjynyň sözi jümlede barmy diýip barla.
```

let s = 'my name is atajan alijanow';
let s1 = 'name';
if(s.indexOf(s1) != -1){
    console.log('bar');
} else {
    console.log('yok');
}

```
#### 27."goose" setirinde ikinji "o"-nyň indeksini tap.
```

let s = 'goose';
let k = 0;
let i1 = 0;
for ( let i = 0; i < s.length ; i++ ){
    if(s[i] == 'o'){
        k++
        i1 = i;
    }
    if(k == 2){
        console.log(i1);
        return
    }
}

```
#### 28.Setirde "a" näçe gezek bar diýip hasapla.
```

let s = 'atajan aliajanow';
let k = 0;
for (let i = 0; i < s.length; i++){
    if(s[i] == 'a'){
        k++
    }
}
console.log(k);

```
#### 29.Tekstde "cat" sözüniň ähli ýerleşýän ýerlerini tap.
```

let s = 'atajan alijanow cat white height cat';
while(s.indexOf('cat') != -1){
    console.log(s.indexOf('cat'));
    s = s.replace('cat','aaa');
}

```
#### 30.Yzygiderli gaýtalanýan nyşan bar diýip barla.
```

let s = 'atajan alijanoww';
for (let i = 0; i < s.length-1; i++ ){
    if(s[i] == s[i+1]){
        console.log('bar');
        return
    }
}
console.log('yok');


```
#### 31."Hello" kiçi harplara geçir.
```

let s = 'Hello';
s[0] = s[0].toLocaleLowerCase();
console.log(s);

```
#### 32."hello" uly harplara geçir.
```

let s = 'hello';
console.log(s.toUpperCase());

```
#### 33.Setirleri harp ýagdaýyna garamazdan deňeşdir.
```

let s = 'aTaJan';
let s1 = 'AtaJan';
s = s.toUpperCase;
s1 = s1.toUpperCase;
if(s == s1){
    console.log('den');
} else {
    console.log('den dal');
}

```
#### 34.Setirde ähli harplar kiçimi diýip barla.
```

let s = 'atajan';
let k = 0;
for (let i = 0; i < s.length; i++){
    if(s[i] == s[i].toLocaleLowerCase()){
        k++
    }
}
if(k == s.length){
    console.log('ahli harplar kici');
} else {
    console.log('ahli harplar kici dal');
}

```
#### 35.Setiriň ilkinji harpyny uly harpa geçir.
```

let s = 'atajan alijanow';
s = s[0].toUpperCase() + s;
s = s.replace(s[1],'');
console.log(s);


```
#### 36.Her sözüň ilkinji harpyny uly harpa geçir.
```

let s = 'atajan alijanow';
let s1 = '';
s = ' ' + s;
let i = -1;
while (  i < s.length-1 ){
    i++
    if(s[i] == ' '){
        s1 += ' ' + s[i+1].toUpperCase();
        i++
    }else{
        s1 += s[i];
    }
}
s1 = s1.replace(' ','');
console.log(s1);


```
#### 37.Harplaryň ýagdaýyny tersine öwür (uly → kiçi, kiçi → uly).
```

let s = 'Atajan Alijanow';
let s1 = '';
for (let i = 0; i < s.length; i++){
    if (!(((s[i].codePointAt() >= 65)&&(s[i].codePointAt() <= 90)) ||
    ((s[i].codePointAt() >= 97)&&(s[i].codePointAt() <= 122)))){ s1 += s[i]; }else{
    if(s[i] === s[i].toLowerCase()){
        s1 += s[i].toUpperCase();
    }
    if(s[i] === s[i].toUpperCase()){
        s1 += s[i].toLowerCase();
    }}
}
console.log(s1);


```
#### 38.Diňe sesli harplary uly harpa geçir.
```

let s = 'atajan';
let i = -1;
let s1 = '';
while ( i < s.length-1){
    i++
    if((s[i] == 'a')||
    (s[i] == 'e')||
    (s[i] == 'i')||
    (s[i] == 'y')||
    (s[i] == 'o')||
    (s[i] == 'u')){
        s1 += s[i].toUpperCase();
        i++
    }
    s1 += s[i];
}
console.log(s1);


```
#### 39.Setiri "camelCase" formatyna geçir.
```

let s = 'hello world';
let i = 0;
let s1 = '';
while(i<s.length){
    if(s[i] != ' '){
        s1 += s[i];
    } else {
        s1 += s[i+1].toUpperCase();
        i++;
    }
    i++;
}
console.log(s1);

```
#### 40.Setiri "snake_case" formatyna geçir.
```

let s = 'Hello World';
let i = -1;
let s1 = '';
while(i < s.length-1){
    i++;
    if(s[i] == ' '){
        s1 += '_';
    } else {
        s1 += s[i].toLowerCase();
    }

}
console.log(s1);

```
#### 41."hello" setirinden "ell" bölegini al.
```

let s = 'hello';
console.log(s.slice(1,4));

```
#### 42.Setiriň ilkinji 4 nyşanyny al.
```

let s = 'hello';
console.log(s.slice(0,4));


```
#### 43.Ilkinji 2 nyşany aýyr.
```

let s = 'hello';
s = s.replace(s.slice(0,2),'');
console.log(s);

```
#### 44.Soňky 3 nyşany al.
```

let s = 'hello';
console.log(s.slice(s.length-3, s.length));


```
#### 45.Jümläniň ortasyndaky sözi al.
```

let s = '1323 32 #!%$^ $%SA ASFf sdgd sglsk';
let s1 = [];
let s2 = '';
let k = 0;
s += ' '; 
for (let i = 0; i < s.length; i++){
    if(s[i] != ' '){
        s2 += s[i]; 
    } else {
        k++
        s1[k] = s2;
        s2 = '';
    }
}
if(k % 2 != 0){
    console.log(s1[k-Math.floor(k / 2)]);
}

```
#### 46.Iki boşluk arasyndaky sözi al.
```

let s = 'atajan sowket erkin';
let k = s.indexOf(' ');
s = s.replace(' ','!');
let k1 = s.indexOf(' ');
console.log(s.slice(k+1,k1));

```
#### 47.Faýl adyndan giňeltmäni aýyr.
```

let s = 'zadaci47.js';
s = s.replace(s.slice(s.indexOf('.'),s.length),'');
console.log(s);


```
#### 48.E-mailden @-dan öňki ady al.
```

let s = 'atajanalijanow5@gmail.com';
console.log(s.slice(0,s.indexOf('@')));


```
