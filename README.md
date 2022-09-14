# Writing-and-Presentation-2

### Javascript Dasar

Javascript merupakan bahasa pemograman yang paling populer karena mudah digunakan dan paling banyak digunakan ketika membuat aplikasi website. javascript mampu membuat aplikasi menjadi dinamis atau nampak hidup dikarenakan terjadi interaksi dua arah. 

### menjalankan javascript
1.  melalui browser

### syntax
syntax bisa diartikan sebagai kosakata dan tata cara penulisan pada bahasa pemograman.

contoh syntax : Alert() , Prompt(), Confirm (), dll.

### Console log
merupakan perintah untuk memperlihatkan kepada browser bahwa suatu program benar atau salah

### Tipe Data
merupakan klasifikasi dari berbagai macam tipe data. terdapat 6 tipe data dasar.
1.  number

adalah tipe data bertipe angka yang bernilai angka bilangan bulat. nummber dibagi 2 ada integer dan ada float/decimal. tipe data integer seperti angka 1, 2, 3 atau -1, -2, -3 dll. sedangkan tipe data float seperti 0,1 0,2 dll

2.  string 

adalah kumpulan dari beberapa karakter huruf, angka dll. penulisan data string diawali denga single quote ('....') atau double quote ("..."). 

3. Boolean

adalah tipe data yang hanya mempunyai dua nilai yaitu true dan false.

4. null

adalah nilai dari suatu variable yang kosong.

5.  undefined

tipe data yang tidak terdefinisi

6.  object

adalah tipe data yang sedang dipakai saat ini. tipe data objek adalah tipe data yang saling berhubungan dengan yang lainnya.

penggunaan tipe data digunakan sesuai dengan kebutuhan programer dalam mengerjakan projek.

### Variable
adalah wadah yang digunakan untuk menyimpan sebuah nilai. contoh jika wadah kosong di isi dengan nilai angka maka variable tersebut bertipe data number.

3 cara mendefinisikan variable yaitu let, var dan const. penggunaan let pada pendefnisian javascript yang baru. sedangkan var pada javascript versi lama. penggunaan const yaitu pada tipe data yang bernilai sudah mutlak dan tidak dapat diubah. 

### Operator
1.  assignment operator digunakan untuk menyimpan sebuah nilai pada variable berupa tanda samadengan (=)
2.  Increment dan Decrements digunakan untuk menambah atau mengurangi sebesar 1 nilai.
3.  Aritmathic Operator digunakan untuk menjalankan operasi matematika seperti: perkalian (*), pembagian (/), penjumlahan (+), pengurangan (-), dan modulus atau hasil bagi (%)
4.  comparison operator digunakan untuk membandingkan dari satu nilai dengan nilai yang lain. outputnya true or false. simbol perbandingan seperti: 
- Lebih kecil dari : <
- Lebih besar dari: >
- Lebih kecil atau sama dengan: <=
- Lebih besar atau sama dengan: >=
- Sama dengan: ===
- Tidak sama dengan: !==

5. logical operator digunakan ketika terdapat sebuah kondisi pada pemograman. Simbol dari Logical Operator sebagai berikut:
- AND operator : &&
- OR operator: ||
- NOT operator: !

### Javascript Conditional
adalah sebuah kondisi jika maka seperti jika lapar maka makan. cara penulisan kondisi di javascript sebagai berikut:
1. If statement yaitu pengeksekusian 1 kondisi.
2. IF .. ELSE statement yaitu pengeksekusian 1 kondisi dan kondisi lainnya apabila nilai bernilai salah.
3. IF ..ELSE IF statement yaitu pengeksekusian nilai apabila memiliki berbagai kondisi.
4. Truthy and falsy digunakan untuk mengecek apakah variabel telah terisi namun tidak mementingkan nilainya.
5. Switch Case Conditional digunakan jika kondisi dan percabangan terlalu banyak.
6. thernary operator digunakan untuk menyingkat syntax menjadi satu baris.

### Javascript Looping
adalah perulangan terhadap sebuah perintah hingga kondisi terpenuhi atau kondisi berhenti tercapai.
1.  for 
2.  while
3.  do while
4.  Nested Loop

### Javascript Scope
Scope adalah suatu konsep untuk memberikan batasan-batasan tertentu dalam menentukan suatu variable dapat diakses atau tidak. batasan tersebut ada yang dinamakan scope global dan local.

Blocks merupakan code yang didalamnya terdapat curly brace/ kurung kurawal {}, yang mana variable yang terdapat di dalam curly brace disebut scope local dan variable diluar curly brace disebut scope global. scope local hanya dapat diakses didalam blocks.

### Javascript Function
Function adalah block code dalam sebuah pemograman yang bertujuan untuk menyelesaikan suatu kasus.

contoh anatomi function

function greeting(){
return "Hello world"
}

ket:
Function => kata kunci dari fungsi
greeting => nama dari fungsi
() => Parameter
return "Hello World" => algoritma
return => perintah untuk mengeluarkan nilai dari local scope ke global scope

#### Parameter dan Argument
Parameter merupakan inputan data terhadap suatu fungsi ketika fungsi dijalankan. 

Argument adalah nilai yang digunakan saat memanggil fungsi

#### Function Helper
menggunakan suatu fungsi untuk fungsi lainnya.

#### Arrow Function
yaitu cara lain menuliskan fungsi, seperti const.

### Data Type Built In
merupakan tipe data bawaan dari javascript. tipe data dapat digolongkan sebagai tipe data primitiv values dan data objects.
- primitiv velues artinya nilai yang bersifat tunggal. pendefinisian data primitiv seperti let nilai = 1
- tipe data object memiliki atribut di local scopenya. contohnya seperti:
let orang (){
 nama : "nisa",
 alamat: "Sumbawa"
 }

contoh cara cek tipe data sebagai berikut:
let nilai = 10;
console.log (typeof nilai); maka akan muncul tipe data number di web browser

- array artinya variable yang nilainya bersifat jamak dan diawali cruly brecat seperti []. data array didefinisikan seperti let KumpulanNilai = [1, 2, 3, 4]. di dalam data array bisa memuat nilai yang tipe datanya berbeda-beda.

### JavaScript dan HTML DOM
digunakan untuk memanipulasi tampilan web agar lebih dinamis. DOM (Document Object Model) bukanlah Javascript melainkan sebuah pintu menuju web browser menggunakan javascript.
- proses rendering dibalik layar sebelum dokumen HTML, CSS maupun javascript ditampilkan ke halaman web browser. berikut proses rendering file HTML
1. Document HTML diproses (Parsing HTML)
2. dipecah menjadi beberapa element yang memuat nama tag dan isi konten (tokens). misalnya tag h1 berisi text: "Hello World"
3. terbentuk render tree yang memuat setiap pecahan dari dokumen HTML sehingga diproses menjadi DOM (Tree). 
4. Misalnya main ---> 1. h1
5.                    2. span
6.                    3. articles -----> 1. p
7.                                       2. h1
8. layout tampilan HTML muncul di web browser (DOM). 
9. *apabila terdapat file CSS maka pembacaan file CSS sama dengan proses rendering file HTML. Perbedaan nya terletak pada hasil akhirnya. pada file CSS akan menjadi CSSOM
10. Selanjutnya, untuk menampilkan file Javascript. Layouting HTML dan CSS digabung membentuk render tree. hasil akhir akan menampilkan tampilan website yang dinamis.

*penempatan script JS dapat mempengaruhi proses rendering file HTML.

Jika saat proses parsing HTML, ditemukan tag <script>, secara default proses parsing akan dihentikan sampai script tersebut selesai diunduh dan dijalankan. oleh karena itu, script pada umumnya diletakkan sebelum tag penutup body agar proses parsing HTML selesai dijalankan.
  
- manipulasi element HTML
1. mencari element HTML. ada 3 mencari element HTML melalui file js. cara pertama menggunakan 1 element dengan id tertentu contoh document.getElementById("header"). cara kedua menggunakan beberapa element sekaligus dengan class tertentu, contoh: document.getElementByClassName ("container"). cara ketiga menggunakan kombinasi selector, contohnya: document.querySelector("#header p span"). 
  
2. mengubah konten element. terdapat dua cara mengubah konten element. pertama Element.textContent yaitu mengubah isi berupa text dari sebuah element secara spesifik. sedangkan yang kedua Element.innerHTML yaitu mendapatkan value berdasarkan content tetapi juga bisa memuat tag html itu sendiri.
3. membuat element HTML. 
  - interaksi users (Events). macam-macam events antara lain click, focus, hover, change, blur, scroll, dan submit. Salah satu cara menangkap interaksi users Element.AddEventListener("Event").

  
















