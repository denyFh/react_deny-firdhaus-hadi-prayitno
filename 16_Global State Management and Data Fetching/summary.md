# Global State Management

## Resume Materi
Dalam materi ini, mempelajari:
- [Global State Management](#global-state-management)
  - [Resume Materi](#resume-materi)
    - [1. Global State Introduction](#1-global-state-introduction)
    - [2. Redux Thunk and Persisted State](#2-redux-thunk-and-persisted-state)
    - [3. Fetching Data](#3-fetching-data)
  - [Task](#task)
    - [Membuat proyek todoapp yang telah dibuat sebelumnya dengan redux](#membuat-proyek-todoapp-yang-telah-dibuat-sebelumnya-dengan-redux)

### 1. Global State Introduction
Global State merupakan artian bahwa state yang diberada dalam setiap komponen react nantinya akan bisa digunakan secara global. Cara untuk mewujudkan hal tersebut adalah dengan menggunakan Redux. Kapan kita harus menggunakan redux:
1. Banyak state yang perlu ditaruh di banyak template
2. State pada app sering berubah
3. Logic untuk mengubah state kompleks
4. Ukuran codebase yang sedang-besar, dan dikerjakan oleh banyak orang
5. Perlu untuk mengetahui bagaimana state diupdate seiring dengan waktu

Beberapa tools dan libraries yang dibutuhkan:
1. React-redux
2. Redux Toolkit
3. Redux DevTools Extension

Komponen penting dalam redux:
1. actions : perantara / pemberi informasi antara reducer dengan store 
2. reducer : tempat untuk mendefinisikan state global dengan mengambil state dan mengembalikan nilai state
3. store : tempat untuk menyimpan state dan perubahan state yang terjadi

Cara untuk memakai dan mengubah state dapat dilakukan dengan dua cara yakni dengan menggunakan hooks atau connect.
### 2. Redux Thunk and Persisted State
Thunk Middleware yang ada pada redux dapat memungkinkan kita untuk membuat action creator yang mengembalikan function bukan action. Redux Thunk diperlukan untuk menghandle side effect logic seperti logic synchronous komples yang perlu mengakses store dan juga logic async seperti request data. Kemudian terdapat Persisted State merupakan suatu implementasi dari library redux-persist yang memungkinkan kita untuk menyimpan suatu state yang telah kita inisialisasi sehingga ketika kita mencoba melakukan reload app kita maka akan memuat state yang sudah diterima atau disimpan pada browser localstorage.
### 3. Fetching Data
Fetching data merupakan salah satu hal yang sering dijumpai dalam suatu app sekarang. dimana kita meminta sebuah data, mengeditnya kemudian menyimpan data tersebut. Terdapat beberapa cara untuk melakukan fetching data dalam react diantaranya:
1. Fetch API
2. Axios
3. React Query Library
## Task
### Membuat proyek todoapp yang telah dibuat sebelumnya dengan redux
Pada task ini, saya ditantang untuk membuat proyek todoapp dengan library react, redux-toolkit, dan react-redux serta react-persist.

Berikut merupakan link repo untuk tugas tersebut:
[Repo Tugas Praktikum Global State Management Deny](https://github.com/denyFh/redux-todo)

Berikut merupakan screenshot dari hasil tampilan website:
![reactReduxAndPersistUsage](./screenshots/global-state.png)

