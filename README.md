# TeachMe
Nama : Gevyndo Gunawan 
NIM : 18221076 
URL API : https://teachme-gevyndo-18221070.azurewebsites.net/

Penjelasan Pembuatan dan Deploy API
Pembuatan API ini menggunakan bahasa Python dengan framework Django dengan REST API. Pada pendeployan, awalnya dilakukan containerization menggunakan Docker terhadap API yang dibuat, lalu container yang telah dibuat dilakukan deploy pada layanan Container Instance milik Microsoft Azure. 
Untuk selengkapnya, dapat dilihat pada link GitHub berikut:
https://github.com/gevyndo/TeachMe

Deskripsi API : 
TeachMe Booking Teacher: Merupakan salah satu microservice dari core business TeachMe untuk memesan tutor. Awalnya pengguna harus memasukkan data terkait dirinya sendiri, seperti nama, email, dan password yang digunakan untuk mendaftarkan akunnya.
Disini saya menggunakan framework Django untuk membuat API tersebut dan mengisolasi dengan docker dan dideploy dengan bantuan Azure. DJango sendiri telah memiliki framework yang jika dijalankan URL-nya lalu ditambahi “/admin/” di belakang URL tersebut akan memiliki tampilan admin yang bisa menambah dan mengurangi data.

Penjelasan Method API 
- /students (GET) → mendapatkan seluruh list data students yang ada
- /students/<id: int> (GET) → mendapatkan data students pada index yang dituju
- /students (POST) → menambahkan destinasi baru dengan field “id”, “name”, “password”
- /students/<id: int> (PUT) → meng-update data students sesuai index
- /students/<id: int> (DELETE) → menghapus data studentsi sesuai dengan index
