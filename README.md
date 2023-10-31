# Lab5web

Nama : Reza Kurniawan

NIM  : 312210436

Kelas : TI.22.A1

## DAFTAR ISI <br>
| No | Description | Link |
|-----|------|-----|
|1|Instruksi Praktikum|[Click Here](#instruksi-praktikum)|
|2|Langkah-langkah Praktikum|[Click Here](#langkah-langkah-praktikum)|
|3|Pertanyaan dan Tugas|[Click Here](#pertanyaan-dan-tugas)|

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab5Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org


## Langkah-langkah Praktikum
> - Persiapan membuat dokumen HTML dengan nama file `lab5_javascript.html` seperti berikut :
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>Mengenal JavaScript</title>
</head>
<body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
<script>
    document.write("Hello World");
    console.log("Hello World");
</script>
</body>
</html>
```

<img width="960" alt="Jav1" src="https://github.com/MohAzmii04/lab5web/assets/115864496/26c10d77-9478-422a-9918-4b648e28edfb">

**1. Javascript Dasar**
> - Pemakaian `Alert` sebagai property window
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>alert box</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    window.alert("ini merupakan pesan untuk anda");
    //-->
    </script>
</body>
</html>
```

<img width="960" alt="situs alert" src="https://github.com/MohAzmii04/lab5web/assets/115864496/38379b6f-2743-496c-b968-5853b4e070d8">


> - Pemakaian `Method` dalam objek
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>skrip javascript</title>
</head>
<body>
percobaan memakai javascript:<br>
    <script language = "javascript" >
    <!-- 
    document.write("selamat mencoba javascript<br>");
    document.write("semoga sukses!");
    //-->
    </script>
</body>
</html>
```


<img width="960" alt="perceboaan jav pic3" src="https://github.com/MohAzmii04/lab5web/assets/115864496/91c64acd-6b38-4e10-9bb2-9dbbe39bb2ae">

> - Pemakaian `Prompt`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>pemasukan data</title>
</head>
<body>
    <script language = "javascript" >
    <!-- 
    var nama = prompt("siapa nama anda?","masukkan nama anda");
    document.write("hai, " + nama);
    //-->
    </script>
</body>
</html>
```


https://github.com/MohAzmii04/lab5web/assets/115864496/4c8e94be-ce97-46b1-9977-eb5b4ee53bd4



> - Pembuatan `Fungsi` dan cara pemanggilannya
```
<!DOCTYPE html>
<html lang="en">
<head>
    <title>contoh program javascript</title>
    <script language="javascript">
    function pesan(){
        alert ("memanggil javascript lewat body onload")
    }
    </script>
</head>
<body onload=pesan()>
</body>
</html>
```

<img width="960" alt="fungsi ppic4" src="https://github.com/MohAzmii04/lab5web/assets/115864496/1407a886-24c0-40af-b8bb-4c053cd0725e">


**2. Dasar Pemrograman di Javascript**
> - Operasi dasar `aritmatika`
```
<html>
<head>
    <title>contoh program javascript</title>

    <script language="javascript">
    function test (val1,val2)
    {
        document.write("<br>"+"perkalian : val1*val2 "+"<br>")
        document.write(val1*val2)
        document.write("<br>"+"pembagian : val1/val2 "+"<br>")
        document.write(val1/val2)
        document.write("<br>"+"penjumlahan : val1+val2 "+"<br>")
        document.write(val1+val2)
        document.write("<br>"+"pengurangan : val1-val2 "+"<br>")
        document.write(val1-val2)
        document.write("<br>"+"modulus : val1%val2 "+"<br>")
        document.write(val1%val2)
    }
    </script>
</head>
<body>
    <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
    </body>
    </html>
```

### vidio belum di up overloud

> - Seleksi kondisi `(if..else)`
```
<html>
<head>
    <title>contoh if-else</title>
</head>
<body>
    <script language = "javascript">
    <!--
      var nilai = prompt("nilai (0-100): ", 0);
      var hasil = "";
      if (nilai >= 60)
      hasil = "lulus";
      else 
      hasil = "tidak lulus";
      document.write("hasil:" + hasil);   
    //-->
    </script>
</body>
</html>
```

### vidio belum di up overloud


> - Penggunaan operator `switch` untuk seleksi kondisi
```
<html>
<head>
    <title>contoh program javascript</title>

<script language="javascript">
function test ()
{
    val1=window.prompt("input nilai (1-5):")
    switch (val1)
    {
        case "1" :
            document.write("bilangan satu")
            break
        case "2" :
            document.write("bilangan dua")
            break
        case "3" :
            document.write("bilangan tiga")
            break
        case "4" :
            document.write("bilangan empat")
            break
        case "5" :
            document.write("bilangan lima")
            break
        default :
            document.write("bilangan lainnya")
    }
}
</script>
</head>
<body>
    <input type="button" name="button1" value="switch" onclick=test()>
</body>
</html>
```

### vidio belum di up overloud

**3. Pembuatan Form**
> - Form `Input`
```
<html>
<head>
    <script language="javascript">
    function test () {
        var val1=document.kirim.T1.value
        if (val1%2==0)
            document.kirim.T2.value="bilangan genap"
        else
            document.kirim.T2.value="bilangan ganjil"
    }
    </script>
</head>
<body>
    <form method="POST" name="kirim">
        <p>BIL <input type="text" name="T1" size="20">
        MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
        <p><input type="button" value="TEBAK" name="B1" onclick=test()></p>
    </form>
</body>
</html>
```

### vidio belum di up overloud

> - Form `Button`
```
<html>
<head>
    <title>objek document</title>
</head>
<body>
    <script language = "javascript">
    <!--
    function ubahWarnaLB(warna) {
        document.bgColor = warna;
    }    
    function ubahWarnaLD(warna) {
        document.fgColor = warna;
    }
    //-->
    </script>

    <h1>tes</h1>
    <form>
        <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
        <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
        <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLLOW')">
        <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
    </form>
    <script language = "javascript">
    <!--
    document.write("Dimodifikasi terakhir pada " +
    document.lastModified);
    //-->
    </script>
</body>
</html>
```



https://github.com/MohAzmii04/lab5web/assets/115864496/f7557725-acea-4c9a-91ed-17bc4e6981d7


**4. HTML DOM**
> - Pilihan menggunakan `checkbox` dengan perhitungan otomatis
```
<!--
File: daftar_menu.html
-->
<html>
<head>
    <title>Daftar Menu</title>
    <script>
        function hitung(ele) {
            var total = document.getElementById('total').value;
                total = (total ? parseInt(total) : 0);
            var harga = 0;

            if (ele.checked) {
                harga = ele.value
                total += parseInt(harga);
            } else {
                harga = ele.value;
                if (total > 0)
                    total -= parseInt(harga);
            }
            document.getElementById('total').value = total;
        }
    </script>
</head>
<body>
    <h1>Daftar Menu Makanan</h1>
    <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" /> Ayam Goreng Rp. 5.000</label><br />
    <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" /> Tempe Goreng Rp. 5.00</label><br />
    <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" /> Telur Dadar Rp. 2.500</label><br />
    <strong>Total Bayar: Rp. <input id="total" type="text" /></strong>
</body>
</html>
```



https://github.com/MohAzmii04/lab5web/assets/115864496/ca2c536e-5758-4e24-bb7c-4925addc05c6


## Pertanyaan dan Tugas
**1. Buat script untuk melakukan `validasi` pada isian form**
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Formulir Validasi</title>

    <!-- my styles css -->
    <link rel="stylesheet" href="style.css">
    <script>
        function validateForm() {
            // Dapatkan referensi ke elemen-elemen formulir
            var nama = document.forms["myForm"]["nama"].value;
            var email = document.forms["myForm"]["email"].value;

            // Lakukan validasi
            if (nama == "") {
                alert("Nama wajib diisi");
                return false;
            }

            if (email == "") {
                alert("Email wajib diisi");
                return false;
            }

            // Validasi apakah email sesuai dengan format yang benar
            var emailPattern = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;

            if (!emailPattern.test(email)) {
                alert("Email tidak valid. Harap masukkan alamat email yang benar.");
                return false;
            }
        }
    </script>
</head>
<body>
    <h1>Formulir Validasi</h1>
    <div class="container">
        <form name="myForm" onsubmit="return validateForm()" method="post">
            <div class="input-group">
                <label for="nama"><img src="user (3).svg" class="label-img"></label>
                <input type="text" id="nama" name="nama" placeholder="Nama" class="input">
            </div>
            
            <div class="input-group">
                <label for="email"><img src="mail.svg" class="label-img"></label>
                <input type="text" id="email" name="email" placeholder="Email" class="input">
            </div>
            
    
            <input type="submit" value="Submit" class="btn">
        </form>
    </div>
    
</body>
</html>
```



https://github.com/MohAzmii04/lab5web/assets/115864496/2d828860-41f1-4c04-97f0-3b59030e69c4



## Finish, Terima Kasih
