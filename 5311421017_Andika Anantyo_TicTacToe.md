Nama : Andika Anantyo

NIM : 5311421017

**PERMAINAN TIC TAC TOE**

**Ringkasan**

Permainan tic tac toe dapat menggunakan algoritma heuristic untuk mencapai solusi optimal. Initial state permainan ini adalah puzzle kosong ukuran 8. Ketika pemain pertama menekan ubin, maka akan membuat tanda silang. Pemain kedua harus menghalangi pemain pertama untuk membuat tanda silang berjajar secara vertikal, horizontal, maupun diagonal. Goal state atau akhir dari permainan ini adalah ketika salah satu pemain berhasilkan menderetkan tanda mereka baik secara vertikal, horizontal, maupun diagonal. Solusi permasalahan pada game ini dapat dilakukan dengan membuat topologi Tree, kemudian setiap langkah pemain akan dijadikan initial state selanjutnya, dan akan dijadikan sebagai initial state yang baru hingga menentukan goal statenya.

![tp_tree](https://github.com/akvrba/praktek_bfs_tictactoe/assets/147400178/63d2004a-6b25-4534-976b-eee38eefae1a)

**Gambar 1.** Topologi Tree pada tic tac toe

**Penjelasan program**

Permainan dibuat menggunakan Java Swing yang terdiri dari 3 buah Java Class dan 3 buah pendeklarasian enumaration. File tersebut ditulis terpisah namun disimpan dalam folder yang sama.

1.  State.Java
2.  Seed.Java
3.  GameState.Java
4.  Cell.Java
5.  Board.Java
6.  GameMain.Java

Enumeration digunakan untuk menyimpan semua variabel secara berurutan. Pada program ini terdapat tiga enumerasi yang didefinisikan yaitu GameState, Seed, dan State.

1.  GameState.Java

    Enumeration ini digunakan untuk mengidentifikasi berbagai status permainan dalam permainan Tic Tac Toe. Terdapat empat konstanta yang didefinisikan di dalam enumerasi ini yaitu:

    **PLAYING**, menunjukkan permainan sedang berlangsung

    **DRAW**, menunjukkan permainan selesai/berakhir dalam kondisi seri/draw

    **CROSS_WON**, menunjukkan pemain dengan tanda “X” menang dalam permainan

    **NOUGHT_WON**, menunjukkan pemain dengan tanda “O” menang dalam permainan
  
3.  Seed.Java

    Enumeration ini digunakan untuk mengidentifikasi isi sel pada permainan. Terdapat tiga variabel yaitu:

    **EMPTY**, menunjukkan sel kosong

    **CROSS**, menunjukkan sel berisi tanda ”X”

    **NOUGHT**, menunjukkan sel berisi tanda ”O”
  
3. State.Java

    Enumeration ini memiliki isi yang sama dengan GameState yaitu PLAYING, DRAW, CROSS_WON, NOUGHT_WON

Ketiga kelas yang dibuat yaitu:

1.  Cell.Java

    Kelas ini digunakan untuk merepresentasikan setiap sel pada papan permainan tic tac toe yang terdiri dari baris dan kolom. Pada kelas ini, terdapat beberapa fungsi yaitu menyimpan isi dari setiap sel (kosong/X/O) dan menggambarkan simbol X dan O pada sel.

2.  Board.Java

    Kelas ini digunakan untuk memodelkan board/papan permainan tic tac toe dengan tiap selnya dan beberapa fungsi pengelolaan seperti pemantauan dan pemeriksaan status permainan pada board (seri/menang).

3.  GameMain.Java

    Kelas ini mengimplementasikan logika permainan tic tac toe, mengatur tampilan board, dan memberikan interaksi dengan pemain melalui klik dengan mouse dengan Mouse Click Handler. Metode main pada kelas ini digunakan untuk memulai aplikasi permainan, mengatur jendela aplikasi, dan memulai permainan dalam lingkungan GUI.

**Hasil**

Hasil program adalah tampilan papan tic tac toe. Pemain dapat mengisi dengan klik sel yang ada yang akan terisi dengan simbol X dan O. Ketika berhasil menghasilkan deret vertikal, horizontal, maupun diagonal, pemain yang berhasil dinyatakan menang yang ditunjukkan pada bar status bagian bawah board.

![hasil_program_tictac](https://github.com/akvrba/praktek_bfs_tictactoe/assets/147400178/f6c39098-9b21-4b4f-b55e-73e93c900bea)

**Gambar 2.** Hasil program

**Penggunaan Java Applet (JApplet)**

Penggunaan Java Applet dan HTML pada jobsheet ketika dijalankan pada browser hanya menampilkan judul dan keterangan ” Your browser does not seem to support \<APPLET\> tag!”.

![hasil_program_website](https://github.com/akvrba/praktek_bfs_tictactoe/assets/147400178/2a065cb4-4335-4a90-88ef-e4ab36eb4671)

**Gambar 3.** Hasil program pada website

**Perubahan Kode**

Perubahan kode yang saya lakukan yaitu pada bagian GameMain.Java. Pada class tersebut terdapat fungsi yang dapat mengatur jumlah kolom dan baris board permainan yang diinginkan, judul permainan, ukuran dan padding cell, ukuran simbol, warna board, dan fungsi lainnya. Perubahan yang saya lakukan adalah penambahan baris dan kolom menjadi 4x4, penggantian keterangan judul dan status bar, dan ukuran cell. Hasil yang didapatkan sebagai berikut.

![hasil_perubahan_program](https://github.com/akvrba/praktek_bfs_tictactoe/assets/147400178/8155865d-b83d-4ea5-815e-bb9074c2774b)

**Gambar 4.** Perubahan program
