1. Lampirkan kedua script SQL kelompok Anda: (1) Query JOIN yang kompleks, dan (2) Script DDL pembentukan kolom/tabel denormalisasi beserta query panggilannya!

jawab:

2. Berdasarkan percobaan kelompok Anda, jelaskan dengan bahasa sendiri kelebihan denormalisasi dalam memangkas penggunaan klausa JOIN pada sistem informasi!

Jawab: Kelebihan utama denormalisasi dalam sistem ini adalah kemampuannya dalam memotong waktu dan fungsi agregasi nya yang berat saat menampilkan data perhitungan (rekapitulasi) dengan menyimpan atribut hasil perhitungan langsung dalam tabel master, jadi sistem hanya perlu memanggilnya dan membuat prosesnya menjadi cepat, dan optimal

3.Jelaskan secara singkat, apa risiko utama terhadap data (contoh: inkonsistensi) yang muncul akibat kelompok Anda menambahkan atribut turunan atau tabel rekapitulasi tersebut?

Jawab: Risiko utama terhadap data akibat penerapan denormalisasi adalah potensi terjadinya inkonsistensi data. Risiko ini muncul karena nilai pada kolom turunan disimpan secara permanen, sehingga jika ada perubahan data asli pada tabel terkait (misalnya mitra menambah atau menghapus lokasi baru), nilai rekapitulasi pada tabel master tidak akan memperbarui dirinya sendiri secara otomatis kecuali dilakukan pembaruan manual atau menggunakan fungsi trigger. Akibatnya, data yang tampil di aplikasi bisa menjadi tidak sinkron atau berbeda dengan kondisi data aslinya.
