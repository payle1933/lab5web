# Praktikum 5 - Pemrograman Web
```
Maulana hasanudin
312010106
TI.20.D.1
Universitas Pelita Bangsa
```
# buat dokumen HTML dengan nama file lab5_javascript.html dan masukan coding

Java Script Dasar
Pemakaian Alert sebagai property window
<img width="1070" alt="1" src="https://user-images.githubusercontent.com/101716660/163516530-5c01fa19-c168-428c-92db-938967ca8cc0.png">

<img width="1070" alt="aaaa" src="https://user-images.githubusercontent.com/101716660/163516677-950c0f6b-bedd-4592-961b-6c6157729186.png">

## Pemakaian method dalam objek
<img width="1070" alt="2" src="https://user-images.githubusercontent.com/101716660/163516735-98462ad5-eb6c-4b55-8c96-19996564e072.png">

<img width="1070" alt="2a" src="https://user-images.githubusercontent.com/101716660/163516748-7dc47bed-f799-46a5-9736-3abcb5a39d3a.png">


## Pemakaian Prompt
<img width="1070" alt="3" src="https://user-images.githubusercontent.com/101716660/163515775-7309a1ef-7216-44cc-a4b6-f2a42ce8d7d9.png">
<img width="1070" alt="3a" src="https://user-images.githubusercontent.com/101716660/163515829-6abf5981-4ba8-4509-92a7-68097324b044.png">



## Pembuatan fungsi dan cara pemanggilannya
<img width="1070" alt="4" src="https://user-images.githubusercontent.com/101716660/163515851-55519a1d-e17c-4e9c-8087-18bd09e9004c.png">
<img width="1070" alt="4a" src="https://user-images.githubusercontent.com/101716660/163515857-2cc88aa6-8a72-4151-9851-66c3a68324b3.png">


# Dasar Pemrograman Di Javascript
## Operasi dasar Aritmatika
<img width="1070" alt="5" src="https://user-images.githubusercontent.com/101716660/163516247-46ec47bf-2858-4514-8d20-2eb067daa338.png">


<img width="1070" alt="5a" src="https://user-images.githubusercontent.com/101716660/163515903-fae485d9-002c-4082-8d4e-0d1e593a2a01.png">



## Seleksi kondisi (if..else)
<img width="1070" alt="6" src="https://user-images.githubusercontent.com/101716660/163515943-efecc2cb-46b3-40fa-9686-8818359dde9e.png">

## Output
<img width="1070" alt="6a" src="https://user-images.githubusercontent.com/101716660/163516786-301c8e99-efda-4bb4-8a09-9f03decfa2f1.png">


## Penggunaan operator switch untuk seleksi kondisi
## Coding LANGKAH 8 Penggunaan operator switch untuk seleksi kondisi (coding)

<img width="1070" alt="7" src="https://user-images.githubusercontent.com/101716660/163516331-125b1a34-e5e0-4397-a34a-3f3b07b3ce52.png">

<img width="1070" alt="7a" src="https://user-images.githubusercontent.com/101716660/163516363-26735e5d-7caa-442f-8e70-916e2cba5502.png">


# Pembuatan Form
## Form Input
### Coding
<img width="1070" alt="8" src="https://user-images.githubusercontent.com/101716660/163516899-07fdf039-a07e-4c59-a5e4-1eea4a238474.png">

### Output 
<img width="1070" alt="8a" src="https://user-images.githubusercontent.com/101716660/163516923-d07f4f27-0a32-4874-8cf6-19bb69b85761.png">


## Form Button
### Coding 

<img width="1070" alt="9" src="https://user-images.githubusercontent.com/101716660/163517049-fe9afda4-9467-491e-842b-14969183dff2.png">



### Output
<img width="1070" alt="9a" src="https://user-images.githubusercontent.com/101716660/163517089-ea5b3fdb-b5d2-4d94-8cb0-5bfea23431d8.png">

# HTML DOM
### Coding 
<img width="1070" alt="10" src="https://user-images.githubusercontent.com/101716660/163517107-40f7c820-6b48-41e9-b081-214a89f5ec12.png">

### Output
<img width="1070" alt="10A" src="https://user-images.githubusercontent.com/101716660/163517127-95955908-9d96-453f-8a83-fbbd0d47a2f3.png">




# TUGAS
## 1. Buat script untuk melakukan validasi pada isian form.
## Buat form pada lab5_javascript.html
```
<!DOCTYPE html>
<html lang="en">
<head>
	<title>Form Validasi</title>
	<link rel="stylesheet" type="text/css" href="style.css">
    <script type="text/javascript">
        function validasiForm() {
            var nama = document.getElementById("nama").value;
            var email = document.getElementById("email").value;
            var alamat = document.getElementById("alamat").value;
            if (nama != "" && email!="" && alamat !="") {
                return true;
            }else{
                alert('Isi Alamat Anda dengan lengkap !');
                return false;
            }
        }
    </script>
</head>
<body>
	<div class="login">
		<form action="beranda.html" method="POST" onSubmit="return validasiForm()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
</html>
```
<img width="1070" alt="11" src="https://user-images.githubusercontent.com/101716660/163517263-08792d7f-c132-4145-82e4-bf95ea3362d8.png">

## Buat halaman beranda beranda.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Beranda</title>
    <link rel="stylesheet" href="style.css">
    <script lang="javascript">
        function pesan() {
            alert ("Selamat Datang!")
        }
    </script>
</head>
<body onload=pesan()>
    <center><h1>Terimakasih telah mendaftar!!!</h1></center>
</body>
</html>
```
<img width="1070" alt="12" src="https://user-images.githubusercontent.com/101716660/163517306-f0a6b001-2030-40c3-b3d9-294f408fd5ce.png">



## Tambahkan CSS untuk mempercantikan tampilan
```
body {
    background: darkgray;
    font-family: sans-serif;
    padding: 100px;
  }
  
  h2 {
    color: #fff;
  }
  
  .login {
    padding: 1em;
    margin: 2em auto;
    width: 17em;
    background: #fff;
    border-radius: 3px;
  }
  
  label {
    font-size: 10pt;
    color: #555;
  }
  
  input[type="text"],
  input[type="email"],
  textarea {
    padding: 8px;
    width: 95%;
    background: #efefef;
    border: 0;
    font-size: 10pt;
    margin: 6px 0px;
  }
  
  .tombol {
    background: #3498db;
    color: #fff;
    border: 0;
    padding: 5px 8px;
  }
 ```
 <img width="1070" alt="13" src="https://user-images.githubusercontent.com/101716660/163517673-b41277d2-abf9-4a6e-81ec-f970f358e155.png">

## hasil akhir

<img width="1070" alt="14" src="https://user-images.githubusercontent.com/101716660/163517804-2105ebb3-fe5a-4f92-a004-d393a62d0bdd.png">

<img width="1070" alt="15" src="https://user-images.githubusercontent.com/101716660/163517815-cc598467-693c-4186-a851-9c2fb0e474c9.png">
