TAILWIND CSS

TAILWIND CSS merupakan sebuah framework css yang mana dia dapat memungkinkan kita untuk membangun sebauh website dengan ulitias yang ada

perbedaan antara TAILWIND CSS dengan BOOTSTRAP yaitu terdapat pada jenisnya
BOOTSTRAP merupakan jenis UI framework yang mana kita bisa mengambil sebuah tatanan yang ada, seperti kita mengambil card,form,sidebar,navbar
TAILWIND CSS merupakan sebuah utility class yang mana kita bisa membuat seperti navbar tetapi dengan melakukan customisasi sendiri

sebelum kita menggunakan TAILWIND CSS diharapkan kita sudah menginstall nodejs versi 19 atau terbaru dan npm versi terbaru

TAHAPAN MENGGUNAKAN TAILWIND CSS
 1. instalasi tailwind css disarankan menggunakan CLI
 2. konfigurasi tailwind css

 1. TAHAP INSTALASI
    untuk melakukan instalasi tailwind css dengan CLI maka jalankan kode berikut (sebelumnya harus sudah menginstall nodejs dan npm versi terbaru)
        npm init -y 
        npm install -D tailwindcss
        npx tailwindcss init 

     npm init -y akan melakukan eksekusi yang mana memudahkan kita untuk melakukan installasi dependency atau modul modul yg di butuhkan dan dia akan membuatkan file package.json secara otomatis
     npx tailwindcss init untuk membuat file tailwind.config.js yang berfungsi sebagai configurasi
     jika seluruh command berhasil di jalankan maka akan terdapat folder node_modules dan file tailwind.config.js package.json package-lock.json

 2. KONFIGURASI 
    a. konfigurasi path merupakan tahap untuk menggunakan code tailwind yang akan di masukan kedalam file html atau javascript lihat file tailwind.config.js
    b. tambhakan file dengan nama bebas dan berextensi .css dan isi dengan @tailwind base;@tailwind components;@tailwind utilities; yangmana code tersebut akan di jalankan pertama kali oleh tailwind
    c. menjalankan tailwind buildprocess dengan mengeksekusi command berikut
        npx tailwindcss -i ./input.css -o ./ouput.css --watch --minify
          npx tailwindcss sebagai eksekusi command
          -i sebagai file eksekusi pertamakali yang akan di jalankan oleh tailwind ikutserkatan pathnya (nama bebas)
          -o sebagai output hasil css kita yangkana kita gunakan di dalam web kita (nama bebas)
          --watch prosess akan terus berjalan sampai kita matikan kembali
          -- minify sebagai versi kecil dari hasil compile cssnya
