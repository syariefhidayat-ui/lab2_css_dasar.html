#Lab2
# Membuat dokumen HTML
Menggunakan < !DOCTYPE html > untuk memberitahu browser bahwa dokumen ini adalah HTML5, < head > untuk tempat menaruh informasi tentang halaman seperti judul, dan < title > untuk judul halaman yang muncul di tab browser.
<img width="1366" height="768" alt="Screenshot (49)" src="https://github.com/user-attachments/assets/ca92e312-ba0c-44d2-8eff-1d85d64b0b4c" />
<br>
<br>
# Mendeklarasikan CSS Internal
Menggunakan < style > ... < / style > untuk tempat menulis kode CSS langsung di dalam file HTML, menggunakan selector seperti body, h1, p, atau kelas/id untuk mengatur elemen
<img width="1366" height="768" alt="Screenshot (50)" src="https://github.com/user-attachments/assets/ac17e928-e73f-428f-962e-47f1e83ceb5a" />
<br>
<br>
# Menambahkan Inline CSS
Menggunakan style = "..." untuk atribut yang digunakan untuk menulis Inline CSS
<img width="1366" height="768" alt="Screenshot (51)" src="https://github.com/user-attachments/assets/e54399a6-81e6-4165-b65d-71c9509de30f" />
<br>
<br>
# Membuat CSS Eksternal
Menggunakan < link rel = " stylesheet " href = " style.css " > untuk menghubungkan file CSS eksternal bernama style.css agar semua gaya di file CSS diterapkan ke halaman, dan < head > untuk bagian yang berisi informasi halaman
<img width="1366" height="768" alt="Screenshot (52)" src="https://github.com/user-attachments/assets/42695413-e918-40bd-ba25-aee5304bf960" />
<br>
<br>
# Menambahkan CSS Selector
Menggunakan # digunakan untuk ID Selector, dan . digunakan untuk Class Selector
<img width="1366" height="768" alt="Screenshot (53)" src="https://github.com/user-attachments/assets/b9d35cc2-0a55-4ac1-a8be-b97de08075d5" />
<br>
<br>
# Jawaban Tugas
1. Saya melakukan beberapa percobaan dengan menambahkan properti baru pada kode CSS di atas dengan mengacu pada CSS Cheat Sheet. Berikut contohnya:<br>
   /* ID Selector */
#intro {
  background: linear-gradient(to right, #418fb1, #09c6f9); /* ubah background jadi gradasi */
  border: 2px dashed #099249;        /* garis tepi jadi garis putus-putus */
  min-height: 120px;                 /* tinggi minimum ditambah jadi 120px */
  padding: 15px;                     /* jarak isi kotak ditambah */
  text-align: center;                /* teks di tengah */
  border-radius: 10px;                /* sudut kotak dibuat melengkung */
  box-shadow: 2px 4px 8px rgba(0,0,0,0.3); /* bayangan untuk efek 3D */
}
#intro h1 {
  color: #fff;
  font-family: 'Arial', sans-serif;  /* ganti jenis font */
  font-size: 28px;                    /* ubah ukuran teks */
  text-transform: uppercase;          /* ubah teks jadi huruf kapital */
}
/* Class Selector */
.button {
  padding: 12px 24px;
  background: #bebcbd;
  color: #fff;
  border-radius: 5px;                  /* sudut tombol melengkung */
  transition: background 0.3s ease;    /* efek transisi saat hover */
}
.button:hover {
  background: #444;                    /* warna berubah saat kursor diarahkan */
} <br>
2. h1 { ... } adalah selector elemen yang berlaku untuk semua elemen < h1 > di dalam dokumen HTML.
   intro h1 { ... } adalah selector gabungan ID + elemen yang hanya akan diterapkan pada elemen < h1 > yang berada di dalam elemen dengan id = "intro" <br>
3. Jika ketiga jenis CSS digunakan pada elemen yang sama, inline CSS memiliki prioritas tertinggi, diikuti internal CSS, kemudian eksternal CSS (selama tidak ada penggunaan !important).
Urutan prioritas:
Inline CSS (paling kuat)
Internal CSS
Eksternal CSS
contohnya:
< head >
  < link rel="stylesheet" href="style.css" >
  < style >
    p {
      color: blue;
    }
  < / style >
< / head >
< body >
  < p style="color: red;" > Ini paragraf < / p >
< / body > Jika di style.css warna p hijau, di internal warna p biru, dan di inline warna p merah, Maka warna teks yang ditampilkan adalah merah karena inline CSS memiliki prioritas tertinggi <br>
4. 
