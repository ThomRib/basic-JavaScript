
# Include Script JavaScript
```html
<script src="scripts/his-name.js"></script>;
```

---

# Komentar
Komentar adalah kode program yang tidak akan dieksekusi ketika dibaca</br>
komentar biasannya digunakan sebagai informasi tambahan atau petunjuk

```js
//komentar 1 baris

/*
komentar lebih dari satu baris
*/
```

---

# Tipe Data
JavaScript hanya mendukung satu tipe data number, dimana tipe data number di JavaScript bisa berupa bilangan bulat atau bilangan desimal
## Number Notation
JavaScript mendukung number notation, defaultnya ada basis 10, JavaScript juga mendukung binary, hexadecimal dan octal</br>
```js
	document.writeln(100)
	document.writeln("</br>")
	document.writeln(100.100)
```
Hexadecimal : 0xFF</br>
Binary : 0b10101</br>
Octal : 0o10</br>
## Boolean
Tipe data boolean adalah tipe data yang berisi data kebenaran, artinya hanya ada dua data, benar dan salah(yes atau no)</br>
Benar di representasikan dengan kata kunci true, dan salah direpresentasikan dengan kata kunci false
```js
	document.writeln(true)
	document.writeln("</br>")
	document.writeln(false)
```
## String
Tipe data string atau text adalh tipe data yang berisikan kumpulan kosong atau lebih karakter</br>
untuk membuat data dengan tipe string, kita perlu menggunakan "(petik dua) atau '(petik satu)sebelum dan setelah isi text nya
```js
	document.writeln("his name");
```
## String
Tipe data string atau text adalh tipe data yang berisikan kumpulan kosong atau lebih karakter</br>
untuk membuat data dengan tipe string, kita perlu menggunakan "(petik dua) atau '(petik satu)sebelum dan setelah isi text nya
```js
	document.writeln("his name");
```
## Escape Sequence
JavaScript mendukung escape sequence di string. Escape sequence merupakan karakter khusus, seperti ENTER, TAB, "(kutip dua), dan lain-lain. </br>
Berikut contoh escape sequence yang didukung oleh JavaScript di data string
<img width="1219" height="344" alt="image" src="https://github.com/user-attachments/assets/e40b9291-605f-4672-b02d-91072c3fa84e" />
```js
  document.writeln("<textarea cols='100' rows='10'>")
  document.writeln("his \n name");
  document.wtiteln("\\helo\\name");
  document.wtiteln('\'learn\'');
  document.wtiteln("</textarea>");
```
## Variable
Variable adalah tempat untuk menyimpan data</br>
Dengan menyimpan data di variable, kita bisa menggunakannya lagi dengan menyebutkan nama variable nya</br>
Untuk membuat variable di JavaScript, kita bisa menggunakan kata kunci var diikuti dengan nama variable nya</br>
JavaScript adalah dynamic language, artinya variable di JavaScript tidak terpaku harus menggunakan satu tipe data, kita bisa mengubah-ubah tipe data di variable yang sama</br>
```js
  var fullname;
```
## Mengubah Value di Variable
Setelah variable di deklarasikan, kita bisa mengubah value atau nilai di dalam variable tersebut</br>
Untuk mengubahnya, kita bisa menggunakan perintah nama variable diikuti dengan tanda = (sama dengan) lalu diikuti dengan value atau nilai nya
```js
  var fullName;

  fullName = "his name";
```
## Membuat Variable Langsung Dengan Value 
Di JavaScript juga kita bisa mendeklarasikan sebuah variable, langsung dengan isi value nya
Caranya kita bisa menggunakan kata kunci var, diikuti nama variable, lalu diikuti dengan tanda = (sama dengan), dan di ikuti dengan value atau nilai nya
```js
  var firstName = "his";
  var Lastname = "name";
  var fullName = "his" + "" + "name";
```
## Mengakses Variable
Salah satu keuntungan menggunakan variable adalah variable bisa digunakan kembali</br>
Hali ini akan mempermudah kita membutuhkan data yang sama berkali-kali</br>
Untuk mengakses variable. kita cukup menyebutkan nama variable nya
```js
  var firstName = "his name";
  document.writeln(firstName);
  document.writeln("</br>");
  document.wrtieln(firstName);
```
## Kata Kunci let dan Const
JavaScript sekarang tidak direkomendasikan lagi menggunakan kata kunci var untuk membuat variable, namun diganti dengan let, hal ini dikarenakan ada masalah dari desain awal var
```js
  //variable let
  let firstName = "his";
  document.writeln("firstName");

  //variable const
  const application = "his name";
```
Kata kunci let itu seperti kata kunci var, dimana data di variable tersebut bisa diubah-ubah sesuka kita</br>
Sedangkan kata kunci const berbeda, ketika sebuah variable sudah diisi di variable const, maka variable tersebut tidak bisa diubah lagi value nya</br>
Variable sejenis ini disebut juga constant

---

# Operator Matematika
JavaScript mendukung banyak sekali operator Matematika untuk tipe data Number, Seperti :
## Operator Aritmatika
```js
  let result = 1 + 2;
  document.writeln("<p>1 + 2 = " + result + "</p>");
  let originalResult = result;
  
  result = result - 1;
  document.writeln("<p>" + originalResult + " - 1 = " + result + "</p>");
  originalResult = result;
  
  result = result * 2;
  document.writeln("<p>" + originalResult + " * 2 = " + result + "</p>")
  originalResult = result;
```
<img width="1220" height="475" alt="image" src="https://github.com/user-attachments/assets/0ee7b127-ba6e-4234-b45b-7a91878aa1df"/>

## Operator Augmented Assignments
```js
  let result = 10;
  result += 10;
  document.writeln("<p>" + result + "</p>");
  
  result -= 10;
  document.writeln("<p>" + result + "</p>");
  
  result *= 10;
  document.writeln("<p>" + result + "</p>");
```
<img width="1219" height="474" alt="image" src="https://github.com/user-attachments/assets/a800823c-365f-4da8-bb34-0803c25288b0"/>

## Operator Unary
```js
  let result = +1;
  document.writeln("<p>" + result + "</p>");
  
  result --;
  document.writeln("<p>" + result + "</p>");
  
  result ++;
  document.writeln("<p>" + result + "</p>");
  
  result = -result;
  document.writeln("<p>" + result + "</p>");
```
<img width="1220" height="344" alt="image" src="https://github.com/user-attachments/assets/eb9e5ac3-f569-484b-8e36-0bbaa18a2f21"/>

Dan lain-lain</br>

---

# Operator Perbandingan
Operasi perbandingan adalah operasi untuk membandingkan dua buah data</br>
Operasi perbandingan adalah operasi yang menghasilkan nilai boolean</br>
Jika hasil operasinya adalah benar, maka nilanya adalah true</br>
Jika hasil operasinya adalah salah, maka nilanya adalah false
<img width="962" height="474" alt="image" src="https://github.com/user-attachments/assets/6732671f-c831-48ee-b6df-e1f09cc441da" />
```js
  let result = 5 == "5";
  document.writeln("<p>" + result + "</p>")
  
  let result = 5 === "5";
  document.writeln("<p>" + result + "</p>")
  
  let result = 5 > 10;
  document.writeln("<p>" + result + "</p>")
  
  let result = 5 < 10;
  document.writeln("<p>" + result + "</p>")
```

---

# Operator Logika
Operator logika adalah operator untuk dua buah data boolean</br>
Hasil dari operator logika adalah boolean lagi
<img width="964" height="218" alt="image" src="https://github.com/user-attachments/assets/bebd1053-8363-4c3f-afd4-cfe2ead00d1b" />
```js
  const nilaiUjian = 70;
  const nilaiAbsensi = 70;
  
  const lulusUjian = nilaiUjian > 75;
  const lulusAbsensi = nilaiAbsensi > 75;
  
  const lulus = lulusUjian && lulusAbsensi;
  document.writeln("<p>" + lulus + "</p>")
```
## Operator &&
<img width="964" height="272" alt="image" src="https://github.com/user-attachments/assets/a1f3ad08-f42f-49aa-9b42-ef768f2121cf" />

## Operator ||
<img width="961" height="269" alt="image" src="https://github.com/user-attachments/assets/49839367-0871-4509-902c-1184a3d884cc" />

## Operator Unary !
<img width="951" height="167" alt="image" src="https://github.com/user-attachments/assets/258c9348-937b-44fe-8207-fb6c72757055" />

---

# Console
JavaScript memiliki fitur untuk melakukan logging bernama Console</br>
Logging adalah mekanisme yang biasa dilakukan oleh programmer untuk menampilkan informasi dari aplikasi yang sedang berjalan, tanpa harus mengganggu alur kerja aplikasi dan juga interaksi user</br>
Untuk melakukan ini, kita bisa menggunakan fitur Console di JavaScript</br>
Untuk menggunakan Console, kita cukup gunakan perintah console di kode JavaScript
<img width="963" height="272" alt="image" src="https://github.com/user-attachments/assets/e57b4f69-d44f-40a5-9f4e-eab84f98cbda" />
```js
	console.log("halo");
```

---

# String Template
Kita sudah tahu bahwa untuk menambahkan string dengan data lain, kita bisa mengguankan operator + (plus)</br>
Namun pada kasus tertentu, penggunaan operator + (plus) sangat menyulitkan, apalagi jika dalam jumlah banyak</br>
JavaScript memiliki fitur yang bernama String Template, dimana kita bisa mensubtitusi data dari luar String ke dalam String, seperti mengambil data variable, atau bahkan melakukan operasi matematika</br>
Untuk menggunakan String Template, cara pembuatan String nya harus menggunakan `(backtick), bukan '(petik satu) atau "(petik dua)
```js
	const template = `Name : `;
```

---

# Mengambil Variable
```js
	const name = "his name";
	const template = `Name : ${name}`;
	
	console.info(template);
```

---

# Expression di String Template
```js
	const name = "his name";
	const value = 80;
	const template = `Name : ${name}, Lulus : ${value > 75}`;
	
	console.info(template);
```

---

# Multiline String 
Stirng template juga bisa digunakan untuk membuat string multi line</br>
Kita cukup tambahkan enter di text nya
```js
	let multiLineString = `
	his
	name
	`;
	
	document.writeln("<pre>");
	document.writeln(multiLineString);
	document.writeln("</pre>");
```

---

# Konversi String dan Number
Saat membuat aplikasi, kadang kita input dari pengguna selalu dalam bentuk String</br>
Sedangkan kita ingin mengelola datanya dalam bentuk Number</br>
Maka sangat disarankan untuk melakukan konversi tipe data
<img width="965" height="359" alt="image" src="https://github.com/user-attachments/assets/b55857ed-155d-4eb4-8706-9a1410f2a8f1" />

## Masalah Tanpa Konversi
```js
	const value1 = "1";
	const value2 = 1;
	const sum = value1 + value2;
	
	document.writeln(`<p>${sum}</p>`)
```
## Konversi String ke Number
```js
	document.writeln(`<p>${parseInt("1.1")}</p>`); // 1
	document.writeln(`<p>${parseFloat("1.1")}</p>`); // 1.1
	document.writeln(`<p>${Number("1.1")}</p>`); // 1.1
```
## NaN
Bagaimana jika ternyata jika ternyata data string yang kita coba konversi ke number bukanlah data yang valid?</br>
Jika data string yang kita coba lakukan konversi bukan lah data valid, maka hasil dari konversi tersebut adalah NaN (Not a Number)</br>
NaN adalah number spesial yang menyebutkan bahwa ini bukanlah number</br>
Jika NaN dioperawsikan dengan data number lainnya, maka hasilnya akan menjadi NaN lagi</br>
```js
	document.writeln(`<p>${parseInt("salah")}</p>`); // NaN
	document.writeln(`<p>${parseFloat("1.1text")}</p>`); // 1.1
	
	// Bumber() tidak akan mentolelir kesalah pada data
	document.writeln(`<p>${Number("1.1ups")}</p>`); // NaN
	document.writeln(`<p>${Number("1x")}</p>`); // NaN
	document.writeln(`<p>${Number("bukan number")}</p>`); // NaN
```
## Operasi pada NaN
```js
	const value1 = Number("salah"); // NaN
	const value2 = 100;
	const sum = value1 + value2; // NaN
	
	document.writeln(`<p>${sum}</p>`);
```
## isNaN() Function
Kadang kita ingin mengecek apakah sebuah number itu NaN atau bukan</br>
Untuk melakukan pengecekan tersebut, kita bisa mengguankan function isNaN(number)</br>
Hasil nya adalah berupa data boolean, true jika NaN, false jika bukan

---

# Tipe Data Array
Array adalah tipe data yang berisikan kumpulan data</br>
Array di JavaScript memiliki sifat dinamis, artinya datanya bisa bertambah dengan sendirinya saat kita memasukan data ke dalam Array
## Membuat Array
```js
	let arrayKosong = [];
	let arrayNama = ["his", "name"];
```
## Cara Kerja Array
Setiap data di Array akan disimpan dalam posisi berurutan, dimana ururtan pertama dimulai dari nomer 0 </br>
Setiap kita menambah data ke Array, otomatis data akan disimpan di urutan terakhir</br>
Urutan di Array, kita sebut dengan index
## Menambah Array
```js
	const name = [];
	names.push("his");
	names.push("name","thomas");
	
	console.table(names);
```
## Operasi di Array
```js
	const name = [];
	names.push("his");
	names.push("name","thomas");
	
	console.table(names);
	
	names[0] = "alex";
	
	console.table(names);
	console.info(names.length)
```
<img width="962" height="347" alt="image" src="https://github.com/user-attachments/assets/75ecef29-710e-4012-9e9b-96f7ac8e55ab" />

## Perlu Diingat!!!
Data di dalam Array tidak ada batasnya harus data apa</br>
Jadi kita bisa memasukkan data apapun ke dalam Array</br>
Bahkan kita juga bisa memasukkan Array ke dalam Array jika kita mau

---

## 📬 Kontak
If you have any questions or would like to contribute, you can call me out:
- 📞 **WhatsApp**: [contact me](https://wa.me/6281258189596)

---
