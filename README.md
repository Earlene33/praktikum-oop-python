# praktikum-oop-python

Tugas Analisis 1 = Maka nilai HP milik hero1 akan berubah dari 100 menjadi 500

Tugas Analisis 2 = Parameter lawan harus berupa objek agar program bisa mengakses nama, HP, dan method milik lawan. Jika hanya string, HP lawan tidak bisa dikurangi dan serangan tidak bisa diproses.

Tugas Analisis 3 = 
- Jika dihapus maka muncul error
- Error, terjadi karena constructor (__init__) milik class Hero tidak dijalankan, sehingga atribut name, hp, dan attack_power tidak pernah dibuat di dalam objek Mage. Meskipun nilai "Eudora" dikirim saat pembuatan objek, data tersebut tidak otomatis tersimpan tanpa pemanggilan constructor induk.
- Fungsi super() berperan untuk memanggil constructor class induk, agar semua atribut milik Hero dapat diwariskan dan digunakan oleh class Mage. Tanpa super(), class anak tidak memiliki data dasar dari class induk.
  
Tugas Analisis 4 =
1. Nilai HP tetap bisa muncul saat diakses dengan _Hero__hp karena Python memakai name mangling. Walaupun bisa, cara ini tidak boleh dipakai karena melanggar aturan enkapsulasi dan membuat data jadi tidak aman.
2. Jika setter tidak diberi validasi, HP bisa menjadi negatif. Setter penting untuk menjaga data tetap masuk akal dan aturan game tidak rusak.

Tugas Analisis 5 = 
1. Error muncul karena Hero tidak membuat method serang yang wajib dari GameUnit. Artinya class belum memenuhi aturan, sehingga objek tidak bisa dibuat.
2. GameUnit tidak bisa dijadikan objek karena hanya berfungsi sebagai kerangka. Tujuannya untuk memastikan semua turunan punya method yang sama dan program tetap konsisten.

Tugas Analisis 6 = 
1. Program tetap jalan walaupun ditambah Healer. Polimorfisme memudahkan penambahan karakter baru tanpa mengubah kode lama.
2. Program error karena serang diganti namanya. Dalam polimorfisme, nama method harus sama agar bisa dipanggil bersama dalam satu loop.


