# Penjelasan Layout dan Styling dengan Tailwind CSS

## 1.Jelaskan keputusan grid-cols/gap di setiap breakpoint?

Saya pilih grid-cols dan gap berbeda untuk tiap ukuran layar supaya tampilan gambar optimal.  
Di HP, pakai 1 kolom agar gambar besar dan mudah dilihat.  
Di tablet, 2 kolom agar muat lebih banyak tanpa terasa sempit.  
Di laptop, 3-4 kolom supaya galeri rapi dan padat seperti Instagram asli.  
Untuk jarak (gap), di HP jaraknya kecil supaya space tidak terbuang, sedangkan di layar besar jaraknya lebih luas agar tampilan nyaman dan tidak mepet.

## 2. bagaimana kamu memanfaatkan utility responsive Tailwind untuk memecahkan masalah layout yang muncul di mobile?

Tailwind punya fitur responsive untuk atur tampilan berdasarkan ukuran layar.  
Di HP, layout di tumpuk vertikal pakai `flex-col` supaya mudah di scroll.  
Di tablet atau komputer, pakai `md:flex-row` agar layout sejajar dan rapi.  
Untuk sorotan gambar, menggunakan `overflow-x-auto` supaya bisa scroll horizontal di HP tanpa merusak tampilan.  
Jadi, dengan Tailwind cukup pakai class responsive yang tersedia tanpa perlu banyak kode khusus.

## 3. jelaskan trade-off antara memakai banyak utility classes vs membuat component CSS tersendiri

**Pakai banyak class Tailwind:**  
Cepat dan praktis, langsung di HTML, mudah atur responsive tanpa kode panjang, tapi HTML bisa jadi penuh dan susah dibaca.

**Bikin CSS sendiri:**  
HTML lebih bersih, styling terpusat dan bisa reuse, tapi butuh waktu nulis dan atur media query manual.

**Kesimpulan:**  
Untuk proyek kecil dan cepat, Tailwind efisien.  
Untuk proyek besar dan tim, CSS terstruktur lebih mudah dipelihara.
