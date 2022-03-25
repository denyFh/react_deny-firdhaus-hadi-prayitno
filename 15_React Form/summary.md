# React Forms

## Resume Materi
Dalam materi ini, mempelajari:
- [React Forms](#react-forms)
  - [Resume Materi](#resume-materi)
    - [1. Penggunaan dan Macam Form](#1-penggunaan-dan-macam-form)
    - [2. Controlled Component & Uncontrolled Component](#2-controlled-component--uncontrolled-component)
    - [3. Basic Validation](#3-basic-validation)
      - [3.1 Mengapa harus validasi?](#31-mengapa-harus-validasi)
      - [3.2 Tipe Validasi](#32-tipe-validasi)
      - [3.3 Built-in validation HTML5](#33-built-in-validation-html5)
      - [3.4 JS Validation](#34-js-validation)
  - [Task](#task)
    - [Mengubah proyek todoapp yang telah dibuat](#mengubah-proyek-todoapp-yang-telah-dibuat)

### 1. Penggunaan dan Macam Form
Form merupakan salah satu hal yang sering digunakan dalam suatu pengembangan aplikasi website. Banyak sekali macam tipe dalam form yakni 
- elemen input
- elemen text area
- elemen select
- radio button
- checkbox

dalam sebuah elemen input terdapat banyak tipe diantara:
- text
- number
- button
- date
- datetime
- time
- file
- reset
- email
- password
- range
dan banya lainnya.
### 2. Controlled Component & Uncontrolled Component
- Controlled Component merupakan sebuah komponen yang elemen formnya di kontrol dengan menggunakan state pada react seperti untuk menyimpan dan memperbarui state pada elemen form tersebut.

- Uncontrolled component adalah alternatif lain dari controlled component, dimana data form akan ditangani oleh DOM-nya sendiri. Untuk menulis uncontrolled component, alih-alih menulis event handler untuk setiap pembaruan state, kita bisa menggunakan ref untuk mendapatkan nilai form dari DOM.

- Kesimpulan yang bisa diambil dari form controlled dan uncontrolled memiliki kelebihannya sendiri. Kita perlu mengevaluasi situasi kita secara spesifik dan memilih pendekatan apa yang cocok untuk kondisi kita.

Jika formulir sangat sederhana dalam hal umpan balik UI, uncontrolled dengan refs sepenuhnya baik-baik saja. Kita tidak perlu mendengarkan apa yang dikatakan berbagai artikel bahwa uncontrolled itu "buruk". Lagipula kita selalu dapat bermigrasi ke controlled input.

### 3. Basic Validation
#### 3.1 Mengapa harus validasi?
Pada dasarnya, ada 3 alasan mengapa validasi form diperlukan :
Mencari input data yang benar dan sesuai format. Sebuah web/aplikasi tidak dapat berjalan dengan benar, jika data yang diolah tidak sesuai dengan kebutuhan aplikasi
Melindungi akun pengguna. Misalnya, membuat pengguna untuk memasukkan data password yang aman
Melindungi sistem/aplikasi. Validasi form yang kuat dapat meminimalisir perilaku pengguna yang ingin meretas sistem/aplikasi

#### 3.2 Tipe Validasi 
1. Client-side Validation 
2. Server-side Validation

#### 3.3 Built-in validation HTML5
1. required
2. minlength n maxlength
3. min n max
4. type
5. pattern

#### 3.4 JS Validation
Bisa kapan saja melakukan validasi dengan menggunakan javascript?
- Ketika ada perubahan di form. Ketika ada perubahan, akan mentrigger event onChange. Kelebihannya validasi akan cukup real-time berdasarkan perubahan data, namun fungsi akan terus dipanggil selama ada perubahan. Bisa dikombinasikan dengan disable button.
- Ketika menekan tombol submit. Ketika menekan tombol submit, akan mentrigger event onSubmit. Kelebihannya validasi cukup sekali, namun tidak akan real-time memvalidasi form.

## Task
### Mengubah proyek todoapp yang telah dibuat
Pada task ini, saya ditantang untuk membuat proyek dengan library react menerapkan react forms dan validation.

Berikut merupakan link repo untuk tugas tersebut:
[Repo Tugas Praktikum React Hooks Deny](https://github.com/denyFh/tugas-react-form-alta)

Berikut merupakan screenshot dari hasil tampilan website:
![reactFormsUsage](./screenshots/react-forms.png)

