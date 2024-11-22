# Cipta-Nama
![CiptaNama](https://og.tailgraph.com/og?fontFamily=Roboto&title=Cipta%20Nama&titleTailwind=text-gray-800%20font-bold%20text-6xl&titleFontFamily=Poppins&text=PHP%20Library%20Generator%20Nama%20Orang%20Orang%20Indonesia&textTailwind=text-gray-700%20text-2xl%20mt-4%20font-semibold&textFontFamily=Poppins&logoTailwind=h-8&bgUrl=https%3A%2F%2Fik.imagekit.io%2Fboostmyo2%2Fogimages_rUeGPDrlM.png%3FupdatedAt%3D1728680113005&bgTailwind=bg-blueGray-900&footer=github.com/wafarifki/Cipta-Nama&footerTailwind=font-bold%20text-3xl%20text-green-600&t=1728680196099&refresh=1%22 "Cipta Nama")

Cipta Nama adalah sebuah library PHP yang berfungsi untuk menghasilkan nama-nama orang Indonesia, baik laki-laki maupun perempuan. Library ini dapat digunakan dalam berbagai proyek untuk menciptakan nama-nama Indonesia yang unik dan autentik.

Cipta Nama dibuat oleh Wafa Rifqi Anafin untuk memudahkan penggunaan generator pembuat nama acak, baik dalam pengembangan aplikasi, situs web, maupun simulasi data lainnya.

Library Cipta-Nama memberikan solusi sederhana dan praktis untuk menghasilkan nama-nama orang Indonesia secara acak, baik untuk jenis kelamin pria maupun wanita. Dengan fungsi yang mudah digunakan, library ini sangat berguna bagi pengembang yang ingin mengintegrasikan nama-nama Indonesia yang otentik ke dalam proyek mereka, misalnya untuk aplikasi, situs web, atau simulasi data.

Fitur Utama:
- Generate Nama Lengkap secara acak untuk pria, wanita, atau campuran.
- Generate Daftar Nama dengan jumlah dan jenis kelamin yang dapat ditentukan.

Dengan instalasi cepat menggunakan Composer, Cipta-Nama siap digunakan dalam berbagai aplikasi PHP dengan cara yang sederhana dan efisien.

## Instalasi
Install library Cipta Nama dari komposer 
```bash
composer require wafarifki/cipta-nama
```

## Penggunaan
Setelah menginstal library ini melalui Composer, Anda dapat menggunakan Cipta Nama di proyek Anda dengan langkah-langkah berikut:
1. **Autoload Composer**: Pastikan untuk memuat autoloader Composer di file PHP Anda.
2. **Inisialisasi Kelas**: Buat instance dari kelas `CiptaNama`.
3. **Generate Nama**: Panggil metode `generateNamaLengkap()` atau `generateDaftarNama()` untuk mulai menghasilkan nama.

## Contoh Kode
Berikut adalah contoh penggunaan Cipta Nama:

```php
<?php
    require 'vendor/autoload.php';
    use Wafarifki\CiptaNama\CiptaNama;
    $generator = new CiptaNama();
    
    // Generate nama lengkap secara acak
    echo "Nama Lengkap Acak: " . $generator->generateNamaLengkap();
    echo '<br><br>';
    
    // Generate nama lengkap pria secara acak
    echo "Nama Lengkap Acak Pria: " . $generator->generateNamaLengkap('pria');
    echo '<br><br>';
    
    // Generate nama lengkap wanita secara acak
    echo "Nama Lengkap Acak Wanita: " . $generator->generateNamaLengkap('wanita');
    echo "<br><br>";
    
    $daftarNamaPria = $generator->generateDaftarNama(5, 'pria');
    echo "5 Daftar Nama Pria: <br>";
    foreach ($daftarNamaPria as $nama) {
        echo $nama;
        echo "<br>";
    }
    
    echo "<br>";
    $daftarNamaWanita = $generator->generateDaftarNama(5, 'wanita');
    echo "5 Daftar Nama Wanita: <br>";
    foreach ($daftarNamaWanita as $nama) {
        echo $nama;
        echo "<br>";
    }
    
    echo "<br>";
    $daftarNamaRandom = $generator->generateDaftarNama(10, 'random');
    echo "5 Daftar Nama Random: <br>";
    foreach ($daftarNamaRandom as $nama) {
        echo $nama;
        echo "<br>";
    }
?>
```

### Let's connect with me!
<p>
    <a href="https://wafarifki.github.io" target="_blank"><img src="https://img.shields.io/badge/Website-https://wafarifki.github.io-blue?" /></a>
    <a href="https://wafarifki.com" target="_blank"><img src="https://img.shields.io/badge/Website-https://wafarifki.com-blue?" /></a>
    <a href="https://www.linkedin.com/in/wafarifqi" target="_blank"><img src="https://img.shields.io/badge/Linkedin-WafaRifkiAnafin_-blue" /></a>
    <a href="https://facebook.com/wafarifkianafin" target="_blank"><img src="https://img.shields.io/badge/Facebook-wafarifkianafin-blue" /></a>
    <a href="https://instagram.com/wafarifki_" target="_blank"><img src="https://img.shields.io/badge/Instagram-@wafarifki_-blue" /></a>
    <a href="https://github.com/wafarifki/wafarifki/raw/main/CV_WafaRifqiAnafin.pdf" target="_blank"><img src="https://img.shields.io/badge/Download-CV_-blue" /></a>
    <a href="https://github.com/sponsors/wafarifki/card" target="_blank"><img src="https://img.shields.io/badge/Give_Me_Your_-Sponsor_To_This_Repository-pink" /></a>
</p>
