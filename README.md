# Assignment1_DiosiPutriArlita_G1A023012
A. PENDAHULUAN

1.1	Latar Belakang Pemograman Java

Di era digital yang semakin maju, pemrograman  menjadi salah satu faktor kunci dalam perkembangan teknologi informasi. Bahasa pemrograman Java yang pertama kali diperkenalkan oleh Sun Microsystems pada tahun 1995 telah menjadi salah satu bahasa pemrograman yang paling berpengaruh dan relevan di industri perangkat lunak. Java menjadi populer karena reputasinya sebagai bahasa pemrograman yang kuat, portabel, dan aman, yang menginspirasi banyak pengembang perangkat lunak untuk menggunakannya dalam berbagai proyek.
Java telah digunakan dalam berbagai konteks pengembangan perangkat lunak, termasuk pengembangan aplikasi desktop, aplikasi web, aplikasi seluler (seperti aplikasi Android), dan bahkan dalam perangkat lunak perusahaan. Keunggulan Java, termasuk portabilitasnya yang luar biasa, menjadikannya ideal untuk proyek yang memerlukan aplikasi yang dapat berjalan di berbagai platform tanpa memerlukan perubahan besar pada sumber kode.
Selain itu, Java  memiliki ekosistem yang kuat dengan banyak perpustakaan dan kerangka kerja  yang membantu pengembang membuat aplikasi kompleks dengan lebih mudah. Hal ini menjadikan Java  pilihan utama untuk mengembangkan perangkat lunak bisnis, sistem perbankan, aplikasi  jaringan, dan banyak lagi. Tugas ini dimaksudkan untuk mempelajari lebih dalam tentang pemrograman Java, termasuk sintaksisnya, fitur-fitur utama, peran dalam pengembangan aplikasi, dan perkembangan terkini di dunia Java.
 Dengan pemahaman  mendalam tentang Java, pembaca akan dapat mengapresiasi pentingnya bahasa ini dalam dunia teknologi informasi dan bagaimana Java terus berkembang dan mengikuti tren teknologi terkini. 

1.2	Rumusan masalah 

1.	Bagaiman cara membuat perulangan pada java?
2.	Bagaimana membuat program dengan menerapkan if else dalam perulangan while?
3.	Bagaimana membuat program zodiac dengan menggunakan fitur input dengan hasil menampilkan zodiac sesuai dengan tanggal lahir yang diinputkan ?
4.	Bagaimana cara membuat sebuah variabel dengan tipe data array, dan menampilkan semua nilai dalam variabel tersebut menggunakan perulangan for?

1.3	Tujuan 
1.	Untuk mengetahui cara membuat perulangan pada java dan menerapkan if else dalam perulangan
2.	Untuk mengetahui cara membuat program zodiac dengan java dan cara membuat variable dengan tipe data array

1.4 Manfaat
1.	Menambah ilmu dan wawasan mengenai pengaplikasian perulangan pada java dan menerapkan if else dalam perulangan
2.	Meningkatkan pemahaman dalam membuat program zodiac dengan java dan cara membuat variable dengan tipe data array
3.	Melatih dan meningkatkan kemampuan dalam pemograman
B. Soal dan Pembahasan
1. Buatlah perulangan hingga 100 menggunakan Java dengan output sebagai berikut:
    1
    2
    3
    4
    5
    6
    7
    8
    9
    (Your Name)
    (Your Name)
    (Your Name)
Jawab :
public class perulangan {
    public static void main(String[] args) {
        for (int i = 1; i <= 100; i++) {
            if (i <= 9) {
                System.out.println(i);
            } else {
                System.out.println(" Diosi Putri Arlita ");
            }
        }
    }
}

Penjelasan Source Code :
1.	public class perulangan {: Ini adalah deklarasi class dengan nama "perulangan". Setiap program Java memerlukan setidaknya satu class dengan nama yang sama dengan nama file Java. Class ini akan berisi metode main yang merupakan titik awal eksekusi program.
2.	public static void main(String[] args) {: Ini adalah deklarasi metode main. Metode main adalah metode yang akan dijalankan ketika program dimulai. Parameter String[] args adalah argumen baris perintah yang dapat diterima oleh program.
3.	for (int i = 1; i <= 100; i++) {: Ini adalah deklarasi perulangan for. Perulangan ini akan dijalankan dari i sama dengan 1 hingga i kurang dari atau sama dengan 100. Pada setiap iterasi, i akan meningkat sebesar 1 (i++).
4.	if (i <= 9) {: Ini adalah pernyataan if yang memeriksa apakah nilai i kurang dari atau sama dengan 9.
5.	System.out.println(i);: Jika kondisi di atas terpenuhi (yaitu jika i kurang dari atau sama dengan 9), maka angka i akan dicetak ke layar dengan menggunakan System.out.println(). Ini akan mencetak angka dari 1 hingga 9.
6.	else {: Jika kondisi di atas tidak terpenuhi, maka bagian else akan dijalankan.
7.	System.out.println(" Diosi Putri Arlita ");: Jika i lebih besar dari 9, teks "Diosi Putri Arlita" akan dicetak ke layar. Ini akan terjadi untuk semua nilai i dari 10 hingga 100.
8.	Dengan demikian, program ini mencetak angka dari 1 hingga 9 ke layar dan kemudian mencetak teks "Diosi Putri Arlita" untuk nilai i dari 10 hingga 100.
2. Buatlah program bebas, dengan menerapkan if else dalam perulangan while.
Jawab :

import java.util.Scanner;

public class GenapGanjilChecker {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        while (true) {
            System.out.print("Masukkan angka (0 untuk keluar): ");
            int angka = scanner.nextInt();

            if (angka == 0) {
                break; // Keluar dari program jika angka yang dimasukkan adalah 0
            }

            if (angka % 2 == 0) {
                System.out.println(angka + " adalah angka genap.");
            } else {
                System.out.println(angka + " adalah angka ganjil.");
            }
        }

        System.out.println("Terima kasih telah menggunakan program ini!");
    }
}

Penjelasan Source Code :
Kode di atas adalah program Java sederhana yang meminta pengguna memasukkan angka melalui keyboard, dan program tersebut akan menentukan apakah angka tersebut adalah angka genap atau ganjil. Program akan terus berjalan hingga pengguna memasukkan angka 0 untuk keluar. 
1.	import java.util.Scanner;: Ini adalah pernyataan impor yang mengimpor kelas Scanner dari paket java.util. Kelas Scanner digunakan untuk membaca input dari pengguna.
2.	public class GenapGanjilChecker {: Ini adalah deklarasi class dengan nama "GenapGanjilChecker". Setiap program Java memerlukan setidaknya satu class dengan nama yang sama dengan nama file Java. Class ini akan berisi metode main yang merupakan titik awal eksekusi program.
3.	public static void main(String[] args) {: Ini adalah deklarasi metode main. Metode main adalah metode yang akan dijalankan ketika program dimulai. Parameter String[] args adalah argumen baris perintah yang dapat diterima oleh program.
4.	Scanner scanner = new Scanner(System.in);: Ini adalah pembuatan objek Scanner yang akan digunakan untuk membaca input dari keyboard (System.in).
5.	while (true) {: Ini adalah perulangan while yang akan terus berjalan selama kondisi di dalam tanda kurung true, yang berarti selamanya.
6.	System.out.print("Masukkan angka (0 untuk keluar): ");: Ini mencetak pesan ke layar untuk meminta pengguna memasukkan angka. Pengguna diminta untuk memasukkan angka, dan 0 digunakan untuk keluar dari program.
7.	int angka = scanner.nextInt();: Ini mengambil angka yang dimasukkan oleh pengguna melalui keyboard dan menyimpannya dalam variabel angka.
8.	if (angka == 0) {: Ini adalah pernyataan if yang memeriksa apakah angka yang dimasukkan adalah 0.
9.	break;: Jika kondisi di atas terpenuhi (yaitu jika angka yang dimasukkan adalah 0), maka program akan keluar dari perulangan while menggunakan pernyataan break.
10.	if (angka % 2 == 0) {: Ini adalah pernyataan if lain yang memeriksa apakah angka yang dimasukkan adalah genap atau ganjil. Ini dilakukan dengan memeriksa sisa pembagian angka dengan 2. Jika sisa pembagian adalah 0, maka angka tersebut adalah genap.
11.	System.out.println(angka + " adalah angka genap.");: Jika kondisi di atas terpenuhi, program mencetak pesan yang menyatakan bahwa angka tersebut adalah angka genap.
12.	else {: Jika kondisi di atas tidak terpenuhi (yaitu angka adalah ganjil), maka bagian else akan dijalankan.
13.	System.out.println(angka + " adalah angka ganjil.");: Jika angka adalah ganjil, program mencetak pesan yang menyatakan bahwa angka tersebut adalah angka ganjil.
14.	Setelah pernyataan if dan else, program kembali ke awal perulangan while dan meminta pengguna untuk memasukkan angka lagi.
15.	Setelah pengguna memasukkan angka 0 untuk keluar, program akan keluar dari perulangan while dan mencetak pesan "Terima kasih telah menggunakan program ini!".
16.	Program ini akan berjalan terus menerima input angka dari pengguna hingga pengguna memasukkan 0 untuk keluar. Saat program berjalan, program akan memberi tahu apakah angka yang dimasukkan adalah genap atau ganjil.

3. Buatlah program zodiac dengan menggunakan fitur input dengan hasil menampilkan zodiac sesuai dengan tanggal lahir yang diinputkan.
Jawab :

import java.util.Scanner;

public class CekZodiak {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);

        System.out.print("Masukkan tanggal lahir (format DD/MM): ");
        String tanggalLahir = input.nextLine();

        // Mengambil tanggal dan bulan dari input
        String[] parts = tanggalLahir.split("/");
        int tanggal = Integer.parseInt(parts[0]);
        int bulan = Integer.parseInt(parts[1]);

        String zodiak = "";

        // Menentukan zodiak berdasarkan tanggal lahir
        if ((bulan == 3 && tanggal >= 21) || (bulan == 4 && tanggal <= 19)) {
            zodiak = "Aries";
        } else if ((bulan == 4 && tanggal >= 20) || (bulan == 5 && tanggal <= 20)) {
            zodiak = "Taurus";
        } else if ((bulan == 5 && tanggal >= 21) || (bulan == 6 && tanggal <= 20)) {
            zodiak = "Gemini";
        } else if ((bulan == 6 && tanggal >= 21) || (bulan == 7 && tanggal <= 22)) {
            zodiak = "Cancer";
        } else if ((bulan == 7 && tanggal >= 23) || (bulan == 8 && tanggal <= 22)) {
            zodiak = "Leo";
        } else if ((bulan == 8 && tanggal >= 23) || (bulan == 9 && tanggal <= 22)) {
            zodiak = "Virgo";
        } else if ((bulan == 9 && tanggal >= 23) || (bulan == 10 && tanggal <= 22)) {
            zodiak = "Libra";
        } else if ((bulan == 10 && tanggal >= 23) || (bulan == 11 && tanggal <= 21)) {
            zodiak = "Scorpio";
        } else if ((bulan == 11 && tanggal >= 22) || (bulan == 12 && tanggal <= 21)) {
            zodiak = "Sagittarius";
        } else if ((bulan == 12 && tanggal >= 22) || (bulan == 1 && tanggal <= 19)) {
            zodiak = "Capricorn";
        } else if ((bulan == 1 && tanggal >= 20) || (bulan == 2 && tanggal <= 18)) {
            zodiak = "Aquarius";
        } else if ((bulan == 2 && tanggal >= 19) || (bulan == 3 && tanggal <= 20)) {
            zodiak = "Pisces";
        } else {
            zodiak = "Tanggal tidak valid.";
        }

        System.out.println("Zodiak Anda adalah " + zodiak);

        input.close();
    }
}

Penjelasan Source Code :
Kode di atas adalah program Java yang meminta pengguna memasukkan tanggal lahir dalam format DD/MM, dan kemudian program akan menentukan zodiak berdasarkan tanggal lahir yang dimasukkan. 
1.	import java.util.Scanner;: Ini adalah pernyataan impor yang mengimpor kelas Scanner dari paket java.util. Kelas Scanner digunakan untuk membaca input dari pengguna.
2.	public class CekZodiak {: Ini adalah deklarasi class dengan nama "CekZodiak". Setiap program Java memerlukan setidaknya satu class dengan nama yang sama dengan nama file Java. Class ini akan berisi metode main yang merupakan titik awal eksekusi program.
3.	public static void main(String[] args) {: Ini adalah deklarasi metode main. Metode main adalah metode yang akan dijalankan ketika program dimulai. Parameter String[] args adalah argumen baris perintah yang dapat diterima oleh program.
4.	Scanner input = new Scanner(System.in);: Ini adalah pembuatan objek Scanner yang akan digunakan untuk membaca input dari keyboard (System.in).
5.	System.out.print("Masukkan tanggal lahir (format DD/MM): ");: Ini mencetak pesan ke layar untuk meminta pengguna memasukkan tanggal lahir dalam format DD/MM.
6.	String tanggalLahir = input.nextLine();: Ini membaca input dari pengguna dalam bentuk string dan menyimpannya dalam variabel tanggalLahir.
7.	String[] parts = tanggalLahir.split("/");: Ini memecah string tanggalLahir menjadi bagian-bagian yang dipisahkan oleh tanda "/" (garis miring) dan menyimpannya dalam array parts.
8.	int tanggal = Integer.parseInt(parts[0]);: Ini mengambil tanggal dari array parts, mengonversinya ke tipe data integer, dan menyimpannya dalam variabel tanggal.
9.	int bulan = Integer.parseInt(parts[1]);: Ini mengambil bulan dari array parts, mengonversinya ke tipe data integer, dan menyimpannya dalam variabel bulan.
10.	String zodiak = "";: Ini adalah deklarasi variabel zodiak yang akan digunakan untuk menyimpan nama zodiak.
11.	Program kemudian menggunakan serangkaian pernyataan if dan else if untuk menentukan zodiak berdasarkan tanggal dan bulan yang dimasukkan. Setiap pernyataan if dan else if memeriksa apakah tanggal dan bulan yang dimasukkan cocok dengan tanggal dan bulan yang sesuai dengan zodiak tertentu.
12.	System.out.println("Zodiak Anda adalah " + zodiak);: Setelah zodiak ditentukan, program mencetak pesan yang menyatakan zodiak yang sesuai dengan tanggal lahir yang dimasukkan oleh pengguna.
13.	input.close();: Ini adalah pernyataan untuk menutup objek Scanner setelah selesai digunakan.
14.	Program ini akan terus berjalan, meminta pengguna memasukkan tanggal lahir, dan kemudian menentukan zodiak berdasarkan tanggal lahir tersebut. Hasil zodiak akan ditampilkan ke layar, dan program akan terus berjalan hingga pengguna mengakhiri program.


4. Buatlah sebuah variabel dengan tipe data array, kemudian tampilkan semua nilai dalam variabel tersebut menggunakan perulangan for.
Jawab :

public class array {
    public static void main(String[] args) {
        // Membuat sebuah array dengan tipe integer
        int[] numbers = {2, 4, 8, 16, 32};

        // Menggunakan perulangan for untuk menampilkan semua nilai dalam array
        for (int i = 0; i < numbers.length; i++) {
            System.out.println("Nilai ke-" + i + ": " + numbers[i]);
        }
    }
}

Penjelasan Source Code :
1.	public class array {: Ini adalah deklarasi class dengan nama "array". Setiap program Java memerlukan setidaknya satu class dengan nama yang sama dengan nama file Java. Class ini akan berisi metode main yang merupakan titik awal eksekusi program.
2.	public static void main(String[] args) {: Ini adalah deklarasi metode main. Metode main adalah metode yang akan dijalankan ketika program dimulai. Parameter String[] args adalah argumen baris perintah yang dapat diterima oleh program.
3.	int[] numbers = {2, 4, 8, 16, 32};: Ini adalah deklarasi array dengan nama numbers. Array ini berisi nilai-nilai integer (bilangan bulat) yang diberikan dalam kurung kurawal {}. Jadi, array numbers akan berisi [2, 4, 8, 16, 32].
4.	for (int i = 0; i < numbers.length; i++) {: Ini adalah deklarasi perulangan for. Perulangan ini akan berjalan dari i sama dengan 0 hingga i kurang dari numbers.length. numbers.length adalah panjang (jumlah elemen) dari array numbers.
5.	System.out.println("Nilai ke-" + i + ": " + numbers[i]);: Di dalam perulangan, program mencetak nilai-nilai dalam array numbers. Pesan yang dicetak mencakup indeks ke-i (dimulai dari 0) dan nilai yang ada di indeks tersebut. Misalnya, jika i adalah 0, maka program akan mencetak "Nilai ke-0: 2", karena 2 adalah nilai yang ada di indeks ke-0 dalam array numbers.



