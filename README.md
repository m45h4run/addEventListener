# addEventListener

`addEventListener()` adalah metode dalam JavaScript yang digunakan untuk menambahkan event listener ke elemen tertentu. Event listener adalah fungsi yang akan dieksekusi ketika event tertentu terjadi pada elemen tersebut.

Berikut adalah beberapa aksi yang dapat Anda gunakan dengan `addEventListener()`:

1. **click**: Terjadi ketika elemen diklik.
2. **mouseenter**: Terjadi ketika kursor mouse memasuki area elemen.
3. **mouseleave**: Terjadi ketika kursor mouse meninggalkan area elemen.
4. **input**: Terjadi ketika nilai dalam elemen input berubah.
5. **change**: Terjadi ketika nilai dalam elemen input berubah dan elemen kehilangan fokus.
6. **submit**: Terjadi ketika sebuah formulir diserahkan.
7. **keydown**: Terjadi ketika tombol keyboard ditekan.
8. **keyup**: Terjadi ketika tombol keyboard dilepaskan setelah ditekan.
9. **focus**: Terjadi ketika elemen menerima fokus.
10. **blur**: Terjadi ketika elemen kehilangan fokus.

Dan masih banyak lagi. Anda dapat menemukan daftar lengkap aksi dan deskripsi mereka di [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/Events). Dengan menggunakan `addEventListener()` dengan salah satu dari aksi ini, Anda dapat menangani interaksi pengguna dengan elemen HTML dan meresponsnya dengan cara yang sesuai.

Contoh: 

    var passwordField = document.getElementById("password");
    passwordField.addEventListener("focus", function() {
    
      if (passwordField.type === "password") {
        passwordField.type = "text";
        showPasswordIcon.className = "show-password glyphicon glyphicon-eye-close";
      } else {
        passwordField.type = "password";
        showPasswordIcon.className = "show-password glyphicon glyphicon-eye-open";
      }

    });
