Sistem Pemantauan dan Edukasi Biodiversitas Mangrove oleh BioMac 🌱
Halo teman-teman! Selamat datang di proyek Sistem Pemantauan dan Edukasi Biodiversitas Mangrove oleh BioMac, dibuat oleh Arry Hutomo dari Eco Techno Leader! Proyek ini dirancang untuk mendukung pelestarian ekosistem mangrove dengan pendekatan disruptive sustainability yang keren banget. Kita akan bikin sistem yang gampang dipake, elegan, dan pastinya punya manfaat besar buat komunitas BioMac dalam menjaga keanekaragaman hayati mangrove serta mengedukasi masyarakat. Yuk, kita mulai petualangan hijau ini! 🚀

Narasi Kasus: BioMac dan Misi Penyelamatan Mangrove
BioMac Biodiversity Mangrove adalah komunitas yang bergerak untuk menyelamatkan ekosistem mangrove di seluruh dunia, dengan fokus pada keanekaragaman hayati (biodiversity) dan keberlanjutan lingkungan. Mangrove bukan sekadar hutan biasa—ini adalah benteng alami yang melindungi pesisir, menyerap karbon, dan menjadi rumah bagi ribuan spesies flora dan fauna. Namun, ekosistem ini terancam oleh deforestasi, polusi, dan perubahan iklim, yang bisa mengganggu keseimbangan alam dan kehidupan masyarakat pesisir.
BioMac punya misi besar:  

Pemantauan Kesehatan Ekosistem: Mendata spesies flora dan fauna di ekosistem mangrove untuk memantau keanekaragaman hayati.  
Kuantifikasi Manfaat Lingkungan: Menghitung potensi karbon yang diserap oleh mangrove untuk mendukung proyek carbon credit dan mitigasi perubahan iklim.  
Edukasi Masyarakat: Memberikan informasi dan rekomendasi aksi kepada masyarakat berdasarkan data yang dikumpulkan, agar mereka ikut terlibat dalam pelestarian mangrove.

Dengan sistem ini, BioMac ingin user (misalnya, relawan atau masyarakat lokal) bisa menginput data seperti nama lokasi, luas area, spesies yang ditemukan, dan status ancaman lingkungan. Sistem akan menghasilkan laporan yang mencakup potensi karbon, tingkat keanekaragaman hayati, dan pesan edukasi untuk masyarakat. Sistem ini juga akan memberikan rekomendasi aksi pelestarian yang bisa langsung diterapkan.

Pengetahuan Detail tentang Mangrove
Apa Itu Mangrove?
Mangrove adalah ekosistem pesisir yang unik, terdiri dari tanaman yang mampu hidup di air asin dan tanah berlumpur dengan kadar oksigen rendah. Di Indonesia, mangrove sering disebut "hutan bakau" dan banyak ditemukan di wilayah seperti pesisir Aceh, Kalimantan, dan Papua. Mangrove punya akar khusus, seperti akar napas (pneumatophores) yang menonjol ke atas untuk bernapas, serta akar jangkar yang kuat untuk menahan gelombang dan lumpur.
Manfaat Mangrove
Mangrove punya peran vital dalam menjaga keseimbangan lingkungan dan kehidupan manusia:

Penjaga Pesisir: Akar mangrove mencegah erosi pantai, melindungi daratan dari tsunami, badai, dan kenaikan permukaan laut.
Penyerap Karbon: Mangrove menyerap karbon hingga 4 kali lebih banyak dibanding hutan hujan tropis, menjadikannya "superhero" dalam mitigasi perubahan iklim.
Keanekaragaman Hayati: Mangrove adalah rumah bagi berbagai spesies, seperti burung migran (misalnya bangau), kepiting bakau, ikan, hingga buaya mangrove di beberapa wilayah.
Sumber Ekonomi: Mangrove mendukung perikanan lokal (ikan dan udang sering berkembang biak di sini), serta menyediakan kayu untuk bahan bangunan atau arang (dengan pengelolaan yang berkelanjutan).
Penyaring Alami: Mangrove menyaring polutan dan sedimen dari air, menjaga kualitas air di sekitar pesisir dan mencegah kerusakan terumbu karang.

Tantangan dan Upaya Pelestarian
Mangrove menghadapi ancaman serius, seperti:

Deforestasi: Banyak mangrove ditebang untuk tambak udang, perkebunan, atau pembangunan.
Polusi: Sampah plastik dan limbah industri sering mencemari ekosistem mangrove.
Perubahan Iklim: Kenaikan permukaan laut dan suhu global mengganggu pertumbuhan mangrove.BioMac berupaya melawan ancaman ini dengan menanam mangrove baru, membersihkan sampah, dan mengedukasi masyarakat. Proyek ini akan membantu BioMac dengan sistem pemantauan yang bisa mendata biodiversitas, menghitung potensi karbon, dan memberikan pesan edukasi yang langsung bisa dipahami oleh masyarakat.


Query Coding Python: Sistem Pemantauan dan Edukasi Biodiversitas Mangrove
Kode ini menggunakan konsep variables (Chapter 1) dan OOP (Chapter 15) dengan pendekatan agak advanced. Kita akan jelaskan setiap langkah query secara detail dengan narasi yang mudah dipahami.
Kode Python
class MangroveEcosystem:
    def __init__(self, nama_lokasi, status_ancaman):
        self.nama_lokasi = nama_lokasi
        self.status_ancaman = status_ancaman.lower()
        self.spesies_flora = []
        self.spesies_fauna = []
        self.luas_area = 0  # dalam hektar
        self.karbon_per_hektar = 150  # ton karbon per hektar (rata-rata mangrove)

    def tambah_spesies_flora(self, spesies):
        self.spesies_flora.append(spesies)
        print(f"Spesies flora '{spesies}' berhasil ditambahkan di {self.nama_lokasi}.")

    def tambah_spesies_fauna(self, spesies):
        self.spesies_fauna.append(spesies)
        print(f"Spesies fauna '{spesies}' berhasil ditambahkan di {self.nama_lokasi}.")

    def set_luas_area(self, luas):
        if luas <= 0:
            print("Luas area harus lebih dari 0 hektar!")
        else:
            self.luas_area = luas
            print(f"Luas area {self.nama_lokasi} berhasil diatur menjadi {self.luas_area} hektar.")

    def hitung_potential_karbon(self):
        total_karbon = self.luas_area * self.karbon_per_hektar
        return total_karbon

    def hitung_indeks_biodiversitas(self):
        total_spesies = len(self.spesies_flora) + len(self.spesies_fauna)
        return total_spesies

    def pesan_edukasi(self):
        if self.status_ancaman == "kritis":
            return ("Mangrove di lokasi ini dalam kondisi kritis! Mangrove sangat penting untuk melindungi pesisir dari erosi, menyerap karbon, dan menyediakan habitat bagi spesies seperti kepiting bakau dan burung migran. Ayo, kita selamatkan bersama dengan menanam mangrove baru dan mengurangi polusi!")
        elif self.status_ancaman == "rawan":
            return ("Mangrove di lokasi ini rawan terancam. Tahukah kamu, mangrove bisa menyerap karbon 4 kali lebih banyak dibanding hutan tropis? Mari kita jaga dengan membersihkan sampah dan melibatkan masyarakat dalam pelestarian!")
        else:
            return ("Mangrove di lokasi ini masih sehat! Mari kita terus pelihara dengan monitoring rutin dan edukasi masyarakat. Mangrove adalah rumah bagi banyak spesies dan membantu menjaga kualitas air pesisir!")

    def rekomendasi_aksi(self):
        indeks_biodiversitas = self.hitung_indeks_biodiversitas()
        if indeks_biodiversitas < 5:
            return "Segera lakukan penanaman mangrove tambahan dan survey biodiversitas untuk meningkatkan keanekaragaman hayati!"
        elif self.luas_area < 10:
            return "Perluas area mangrove untuk meningkatkan penyerapan karbon dan mendukung lebih banyak spesies."
        elif self.status_ancaman in ["kritis", "rawan"]:
            return "Lakukan aksi darurat: bersihkan sampah, tanam mangrove baru, dan edukasi masyarakat sekitar!"
        else:
            return "Ekosistem mangrove sehat, lanjutkan monitoring dan libatkan masyarakat dalam pelestarian jangka panjang!"

# Input dari user
print("=== Sistem Pemantauan dan Edukasi Biodiversitas Mangrove oleh BioMac ===")
nama_lokasi = input("Masukkan nama lokasi mangrove (contoh: Hutan Bakau Desa Makmur): ")
status_ancaman = input("Masukkan status ancaman mangrove (kritis/rawan/aman, contoh: rawan): ")
mangrove = MangroveEcosystem(nama_lokasi, status_ancaman)

# Input luas area
luas = float(input("Masukkan luas area mangrove (dalam hektar, contoh: 20): "))
mangrove.set_luas_area(luas)

# Input spesies flora
print("Masukkan 3 spesies flora yang ada di lokasi (contoh: Rhizophora, Avicennia, Sonneratia):")
for i in range(3):
    spesies = input(f"Spesies flora ke-{i+1}: ")
    mangrove.tambah_spesies_flora(spesies)

# Input spesies fauna
print("Masukkan 3 spesies fauna yang ada di lokasi (contoh: Kepiting Bakau, Burung Migran, Ikan):")
for i in range(3):
    spesies = input(f"Spesies fauna ke-{i+1}: ")
    mangrove.tambah_spesies_fauna(spesies)

# Menampilkan hasil
print("\n=== Laporan Biodiversitas Mangrove ===")
print(f"Lokasi: {mangrove.nama_lokasi}")
print(f"Status Ancaman: {mangrove.status_ancaman}")
print(f"Luas Area: {mangrove.luas_area} hektar")
print(f"Spesies Flora: {mangrove.spesies_flora}")
print(f"Spesies Fauna: {mangrove.spesies_fauna}")
print(f"Indeks Biodiversitas: {mangrove.hitung_indeks_biodiversitas()} spesies")
print(f"Potensi Karbon Diserap: {mangrove.hitung_potential_karbon()} ton")
print(f"Pesan Edukasi: {mangrove.pesan_edukasi()}")
print(f"Rekomendasi Aksi: {mangrove.rekomendasi_aksi()}")

Penjelasan Langkah demi Langkah dengan Narasi Detail
Tahap 1: Membuat Class MangroveEcosystem
Kita mulai dengan membuat class MangroveEcosystem menggunakan konsep OOP (Chapter 15). Class ini akan merepresentasikan ekosistem mangrove di suatu lokasi.  

Langkah 1.1: Inisialisasi AtributDi sini, kita mendefinisikan atribut seperti nama lokasi, status ancaman, daftar spesies, luas area, dan karbon per hektar. Atribut ini disimpan sebagai variables (Chapter 1).  def __init__(self, nama_lokasi, status_ancaman):
    self.nama_lokasi = nama_lokasi
    self.status_ancaman = status_ancaman.lower()
    self.spesies_flora = []
    self.spesies_fauna = []
    self.luas_area = 0  # dalam hektar
    self.karbon_per_hektar = 150  # ton karbon per hektar (rata-rata mangrove)

Narasi: Kita menggunakan method __init__ untuk membuat "blueprint" ekosistem mangrove. nama_lokasi dan status_ancaman diambil dari input user, sementara spesies_flora dan spesies_fauna kita buat sebagai list kosong untuk nanti diisi. karbon_per_hektar kita set sebagai nilai tetap 150 ton per hektar berdasarkan rata-rata mangrove.Do: Gunakan self untuk menyimpan data yang akan dipakai di seluruh class.Don't: Jangan lupa ubah input status_ancaman ke lowercase agar konsisten saat pengecekan nanti.

Tahap 2: Method untuk Menambah Spesies
Kita buat method untuk menambah spesies flora dan fauna ke dalam list.  

Langkah 2.1: Method tambah_spesies_floraMethod ini akan menambahkan spesies flora yang diinput user ke dalam list spesies_flora.  
def tambah_spesies_flora(self, spesies):
    self.spesies_flora.append(spesies)
    print(f"Spesies flora '{spesies}' berhasil ditambahkan di {self.nama_lokasi}.")

Narasi: Method ini sederhana tapi penting. Kita pakai append() untuk menambahkan spesies ke list, lalu kasih konfirmasi ke user bahwa spesies sudah ditambahkan. Misalnya, kalau user input "Rhizophora", sistem akan bilang bahwa spesies itu sudah masuk ke daftar.Do: Gunakan append() untuk menambah elemen ke list.Don't: Jangan pake list kalau data ini gak boleh diubah (pake tuple kalau perlu).  

Langkah 2.2: Method tambah_spesies_faunaSama seperti flora, method ini menambah spesies fauna ke dalam list spesies_fauna.  
def tambah_spesies_fauna(self, spesies):
    self.spesies_fauna.append(spesies)
    print(f"Spesies fauna '{spesies}' berhasil ditambahkan di {self.nama_lokasi}.")

Narasi: Method ini mirip dengan tambah_spesies_flora, tapi khusus untuk fauna. Kita juga kasih konfirmasi ke user supaya mereka tahu data sudah masuk. Misalnya, kalau user input "Kepiting Bakau", sistem akan konfirmasi bahwa spesies itu sudah ditambahkan.Do: Beri feedback ke user dengan print() supaya mereka tahu data sudah diproses.Don't: Jangan lupa cek validitas input kalau sistem lebih kompleks (misalnya, cek apakah spesies sudah ada di list).


Tahap 3: Method untuk Mengatur Luas Area
Kita buat method untuk mengatur luas area mangrove dengan validasi.  

Langkah 3.1: Method set_luas_areaMethod ini memastikan luas area yang diinput user valid (lebih dari 0).  def set_luas_area(self, luas):
    if luas <= 0:
        print("Luas area harus lebih dari 0 hektar!")
    else:
        self.luas_area = luas
        print(f"Luas area {self.nama_lokasi} berhasil diatur menjadi {self.luas_area} hektar.")

Narasi: Method ini menerima input luas area dari user dan menyimpannya ke atribut luas_area. Kita tambahkan validasi sederhana: kalau luas kurang dari atau sama dengan 0, sistem akan kasih peringatan. Kalau valid, luas akan disimpan dan user dapat konfirmasi. Misalnya, kalau user input 20 hektar, sistem akan bilang bahwa luas sudah diatur.Do: Selalu tambahkan validasi untuk input user agar data yang disimpan valid.Don't: Jangan biarkan input invalid (seperti luas negatif) masuk ke sistem tanpa peringatan.

Tahap 4: Method untuk Menghitung Potensi Karbon
Kita buat method untuk menghitung potensi karbon yang diserap mangrove.  

Langkah 4.1: Method hitung_potential_karbonMethod ini menghitung total karbon berdasarkan luas area dan karbon per hektar.  def hitung_potential_karbon(self):
    total_karbon = self.luas_area * self.karbon_per_hektar
    return total_karbon

Narasi: Method ini sederhana tapi sangat penting. Kita kalikan luas area dengan nilai karbon_per_hektar (150 ton per hektar) untuk tahu berapa ton karbon yang bisa diserap. Misalnya, kalau luas area 20 hektar, maka potensi karbonnya adalah 20 * 150 = 3000 ton. Ini akan membantu BioMac dalam proyek carbon credit.Do: Simpan konstanta seperti karbon_per_hektar sebagai atribut class agar mudah diubah kalau perlu.Don't: Jangan hardcode nilai konstanta di dalam method, biar fleksibel.

Tahap 5: Method untuk Menghitung Indeks Biodiversitas
Kita buat method untuk menghitung indeks biodiversitas berdasarkan jumlah spesies.  

Langkah 5.1: Method hitung_indeks_biodiversitasMethod ini menghitung total spesies flora dan fauna sebagai indeks sederhana.  def hitung_indeks_biodiversitas(self):
    total_spesies = len(self.spesies_flora) + len(self.spesies_fauna)
    return total_spesies

Narasi: Indeks biodiversitas kita buat sederhana dengan menjumlahkan jumlah spesies flora dan fauna. Misalnya, kalau ada 3 spesies flora dan 3 spesies fauna, indeksnya adalah 6. Ini akan jadi acuan untuk rekomendasi aksi nanti.Do: Gunakan len() untuk menghitung jumlah elemen dalam list dengan cepat.Don't: Jangan pake logika yang terlalu rumit untuk indeks sederhana, biar gampang dimengerti.

Tahap 6: Method untuk Pesan Edukasi
Kita buat method untuk memberikan pesan edukasi kepada masyarakat berdasarkan status ancaman.  

Langkah 6.1: Method pesan_edukasiMethod ini memberikan pesan yang berbeda sesuai status ancaman.  def pesan_edukasi(self):
    if self.status_ancaman == "kritis":
        return ("Mangrove di lokasi ini dalam kondisi kritis! Mangrove sangat penting untuk melindungi pesisir dari erosi, menyerap karbon, dan menyediakan habitat bagi spesies seperti kepiting bakau dan burung migran. Ayo, kita selamatkan bersama dengan menanam mangrove baru dan mengurangi polusi!")
    elif self.status_ancaman == "rawan":
        return ("Mangrove di lokasi ini rawan terancam. Tahukah kamu, mangrove bisa menyerap karbon 4 kali lebih banyak dibanding hutan tropis? Mari kita jaga dengan membersihkan sampah dan melibatkan masyarakat dalam pelestarian!")
    else:
        return ("Mangrove di lokasi ini masih sehat! Mari kita terus pelihara dengan monitoring rutin dan edukasi masyarakat. Mangrove adalah rumah bagi banyak spesies dan membantu menjaga kualitas air pesisir!")

Narasi: Method ini memberikan pesan edukasi yang relevan untuk masyarakat. Kalau status ancaman "kritis", pesan akan lebih mendesak dan mengajak aksi langsung. Kalau "rawan", pesan akan berisi fakta menarik tentang mangrove untuk meningkatkan kesadaran. Kalau "aman", pesan akan mengajak untuk terus menjaga ekosistem. Pesan ini dirancang supaya masyarakat paham pentingnya mangrove dan termotivasi untuk ikut melestarikan.Do: Buat pesan yang informatif dan mengajak aksi dengan bahasa yang sederhana.Don't: Jangan pake pesan yang terlalu panjang atau teknis, biar mudah dipahami masyarakat umum.

Tahap 7: Method untuk Rekomendasi Aksi
Kita buat method untuk memberikan rekomendasi aksi pelestarian.  

Langkah 7.1: Method rekomendasi_aksiMethod ini memberikan saran berdasarkan indeks biodiversitas, luas area, dan status ancaman.  def rekomendasi_aksi(self):
    indeks_biodiversitas = self.hitung_indeks_biodiversitas()
    if indeks_biodiversitas < 5:
        return "Segera lakukan penanaman mangrove tambahan dan survey biodiversitas untuk meningkatkan keanekaragaman hayati!"
    elif self.luas_area < 10:
        return "Perluas area mangrove untuk meningkatkan penyerapan karbon dan mendukung lebih banyak spesies."
    elif self.status_ancaman in ["kritis", "rawan"]:
        return "Lakukan aksi darurat: bersihkan sampah, tanam mangrove baru, dan edukasi masyarakat sekitar!"
    else:
        return "Ekosistem mangrove sehat, lanjutkan monitoring dan libatkan masyarakat dalam pelestarian jangka panjang!"

Narasi: Method ini menganalisis tiga faktor: indeks biodiversitas, luas area, dan status ancaman. Kalau indeks biodiversitas kurang dari 5, kita sarankan untuk menambah spesies. Kalau luas area kurang dari 10 hektar, kita sarankan untuk memperluas. Kalau status ancaman kritis atau rawan, kita sarankan aksi darurat. Kalau semua baik, kita dorong untuk terus monitoring. Rekomendasi ini akan membantu BioMac merencanakan langkah pelestarian yang tepat.Do: Gunakan logika bertingkat untuk rekomendasi yang spesifik dan actionable.Don't: Jangan buat rekomendasi yang terlalu umum, biar user tahu langkah konkret yang harus dilakukan.

Tahap 8: Input dari User
Kita minta user untuk menginput data yang dibutuhkan sistem.  

Langkah 8.1: Input Nama Lokasi dan Status Ancaman  
nama_lokasi = input("Masukkan nama lokasi mangrove (contoh: Hutan Bakau Desa Makmur): ")
status_ancaman = input("Masukkan status ancaman mangrove (kritis/rawan/aman, contoh: rawan): ")
mangrove = MangroveEcosystem(nama_lokasi, status_ancaman)

Narasi: Pertama, kita minta user untuk menginput nama lokasi mangrove, misalnya "Hutan Bakau Desa Makmur". Lalu, kita minta status ancaman dengan tiga pilihan: kritis, rawan, atau aman. Input ini akan digunakan untuk membuat objek MangroveEcosystem yang akan menyimpan semua data.Do: Beri contoh input yang jelas supaya user tahu apa yang harus dimasukkan.Don't: Jangan lupa ubah input status_ancaman ke lowercase di __init__ agar konsisten.

Langkah 8.2: Input Luas Area  
luas = float(input("Masukkan luas area mangrove (dalam hektar, contoh: 20): "))
mangrove.set_luas_area(luas)

Narasi: Selanjutnya, kita minta user untuk menginput luas area dalam hektar, misalnya 20. Input ini harus dalam bentuk angka desimal, jadi kita ubah ke float. Method set_luas_area akan memproses input ini dan memberikan konfirmasi kalau luas sudah disimpan.Do: Ubah input ke tipe data yang sesuai (misalnya float untuk angka desimal).Don't: Jangan lupa validasi input di method set_luas_area.

Langkah 8.3: Input Spesies Flora  
print("Masukkan 3 spesies flora yang ada di lokasi (contoh: Rhizophora, Avicennia, Sonneratia):")
for i in range(3):
    spesies = input(f"Spesies flora ke-{i+1}: ")
    mangrove.tambah_spesies_flora(spesies)

Narasi: Kita minta user untuk menginput 3 spesies flora yang ditemukan di lokasi, misalnya "Rhizophora", "Avicennia", dan "Sonneratia". Kita gunakan loop for untuk minta input 3 kali, dan setiap spesies akan diproses oleh method tambah_spesies_flora, yang juga akan kasih konfirmasi ke user.Do: Gunakan loop untuk minta input berulang dengan jumlah tertentu.Don't: Jangan minta input tanpa batas, biar sistem gak membingungkan.

Langkah 8.4: Input Spesies Fauna  
print("Masukkan 3 spesies fauna yang ada di lokasi (contoh: Kepiting Bakau, Burung Migran, Ikan):")
for i in range(3):
    spesies = input(f"Spesies fauna ke-{i+1}: ")
    mangrove.tambah_spesies_fauna(spesies)

Narasi: Sama seperti flora, kita minta user untuk menginput 3 spesies fauna, misalnya "Kepiting Bakau", "Burung Migran", dan "Ikan". Loop for digunakan lagi untuk minta input 3 kali, dan method tambah_spesies_fauna akan memprosesnya sambil kasih konfirmasi.Do: Beri petunjuk input yang spesifik supaya user tahu format yang diharapkan.Don't: Jangan lupa kasih konfirmasi setiap kali data ditambahkan, biar user tahu prosesnya berhasil.


Tahap 9: Menampilkan Laporan
Kita tampilkan laporan lengkap berdasarkan data yang diinput user.  

Langkah 9.1: Menampilkan Hasil  print("\n=== Laporan Biodiversitas Mangrove ===")
print(f"Lokasi: {mangrove.nama_lokasi}")
print(f"Status Ancaman: {mangrove.status_ancaman}")
print(f"Luas Area: {mangrove.luas_area} hektar")
print(f"Spesies Flora: {mangrove.spesies_flora}")
print(f"Spesies Fauna: {mangrove.spesies_fauna}")
print(f"Indeks Biodiversitas: {mangrove.hitung_indeks_biodiversitas()} spesies")
print(f"Potensi Karbon Diserap: {mangrove.hitung_potential_karbon()} ton")
print(f"Pesan Edukasi: {mangrove.pesan_edukasi()}")
print(f"Rekomendasi Aksi: {mangrove.rekomendasi_aksi()}")

Narasi: Terakhir, kita tampilkan laporan lengkap yang mencakup semua data: nama lokasi, status ancaman, luas area, daftar spesies, indeks biodiversitas, potensi karbon, pesan edukasi, dan rekomendasi aksi. Laporan ini dirancang supaya user (relawan atau masyarakat) bisa langsung paham kondisi ekosistem dan apa yang harus dilakukan selanjutnya.Do: Tampilkan data dengan format yang rapi dan mudah dibaca.Don't: Jangan tampilkan data tanpa konteks, biar user tahu maksud dari setiap informasi.

Tahap 10: Menjalankan dan Melihat Hasil
Jalankan kode di VS Code:  

Copy kode di atas.  
Buka VS Code, buat file baru bernama mangrove_system.py.  
Paste kode, lalu simpan (Ctrl+S).  
Buka terminal di VS Code (Ctrl+`).  
Ketik python mangrove_system.py lalu Enter.

Contoh Input dan Output:Input:  
Masukkan nama lokasi mangrove (contoh: Hutan Bakau Desa Makmur): Hutan Bakau Desa Makmur
Masukkan status ancaman mangrove (kritis/rawan/aman, contoh: rawan): rawan
Masukkan luas area mangrove (dalam hektar, contoh: 20): 20
Masukkan 3 spesies flora yang ada di lokasi (contoh: Rhizophora, Avicennia, Sonneratia):
Spesies flora ke-1: Rhizophora
Spesies flora ke-2: Avicennia
Spesies flora ke-3: Sonneratia
Masukkan 3 spesies fauna yang ada di lokasi (contoh: Kepiting Bakau, Burung Migran, Ikan):
Spesies fauna ke-1: Kepiting Bakau
Spesies fauna ke-2: Burung Migran
Spesies fauna ke-3: Ikan

Output:  
=== Sistem Pemantauan dan Edukasi Biodiversitas Mangrove oleh BioMac ===
Luas area Hutan Bakau Desa Makmur berhasil diatur menjadi 20 hektar.
Spesies flora 'Rhizophora' berhasil ditambahkan di Hutan Bakau Desa Makmur.
Spesies flora 'Avicennia' berhasil ditambahkan di Hutan Bakau Desa Makmur.
Spesies flora 'Sonneratia' berhasil ditambahkan di Hutan Bakau Desa Makmur.
Spesies fauna 'Kepiting Bakau' berhasil ditambahkan di Hutan Bakau Desa Makmur.
Spesies fauna 'Burung Migran' berhasil ditambahkan di Hutan Bakau Desa Makmur.
Spesies fauna 'Ikan' berhasil ditambahkan di Hutan Bakau Desa Makmur.

=== Laporan Biodiversitas Mangrove ===
Lokasi: Hutan Bakau Desa Makmur
Status Ancaman: rawan
Luas Area: 20 hektar
Spesies Flora: ['Rhizophora', 'Avicennia', 'Sonneratia']
Spesies Fauna: ['Kepiting Bakau', 'Burung Migran', 'Ikan']
Indeks Biodiversitas: 6 spesies
Potensi Karbon Diserap: 3000 ton
Pesan Edukasi: Mangrove di lokasi ini rawan terancam. Tahukah kamu, mangrove bisa menyerap karbon 4 kali lebih banyak dibanding hutan tropis? Mari kita jaga dengan membersihkan sampah dan melibatkan masyarakat dalam pelestarian!
Rekomendasi Aksi: Lakukan aksi darurat: bersihkan sampah, tanam mangrove baru, dan edukasi masyarakat sekitar!

"Setiap langkah kecil dalam melestarikan mangrove adalah cara kita bersyukur kepada Tuhan atas ciptaan-Nya yang indah. Jangan pernah menyerah, karena usahamu adalah bagian dari perubahan besar untuk dunia yang lebih hijau! 🌿"
"Ya Tuhan, kuatkan hati kami dalam belajar dan menyelesaikan proyek ini. Berikan kami keikhlasan dan ketekunan untuk terus berkarya demi menjaga bumi yang Kau ciptakan. Aamiin."
Untuk Komunitas BioMac
Proyek ini dirancang untuk langsung bisa digunakan oleh komunitas BioMac Biodiversity Mangrove di mana saja. Kalian bisa:  

Gunakan sistem ini untuk memantau biodiversitas mangrove dan menghitung potensi karbon.  
Sebarkan pesan edukasi kepada masyarakat untuk meningkatkan kesadaran.  
Terapkan rekomendasi aksi untuk langkah pelestarian yang konkret.Bersama, kita wujudkan sustainability yang berdampak! 🌍

Dibuat dengan 💖 oleh Arry Hutomo - Eco Techno Leader.


