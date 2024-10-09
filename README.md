# POO_Latihan2
Nama:Wishnu Aqbil Ramadani Kelas: TI.23.A6

Jawaban!

Latihan 1

Apa yang harus didefinisikan sebelum membuat objek?

> Sebelum membuat objek, kita perlu mendefinisikan sebuah class sebagai rancangan atau blueprint dari objek yang akan kita buat.

Buatlah gambar diagram class dan dua buah objek dari class Person bernama Antor dan Riko!

> Class Diagram

![gambar](POO/POO1.png)

> Object Instances

> ![gambar](POO/POO2.png)    ![gambar](POO/POO3.png)
 
Buatlah gambar diagram objek AkunBank dengan instance method simpan Uang, ambilUang dan cekSaldo!

> Class Diagram

![gambar](POO/POO4.png)

> Object Instances

![gambar](POO/POO5.png)

Latihan 2

Buatlah kode program java untuk:

Mendeklarasikan class Person, dengan atribut Nama,JenisKelamin, Umur
Buatlah dua buah objek dari class Person bernama Anton dan Riko

package Person;

public class Person {
    private String nama;
    private String jenisKelamin;
    private int umur;

    // Constructor
    public Person(String nama, String jenisKelamin, int umur) {
        this.nama = nama;
        this.jenisKelamin = jenisKelamin;
        this.umur = umur;
    }

    // Getters and Setters
    public String getNama() {
        return nama;
    }

    public void setNama(String nama) {
        this.nama = nama;
    }

    public String getJenisKelamin() {
        return jenisKelamin;
    }

    public void setJenisKelamin(String jenisKelamin) {
        this.jenisKelamin = jenisKelamin;
    }

    public int getUmur() {
        return umur;
    }

    public void setUmur(int umur) {
        this.umur = umur;
    }

    // toString method to return a proper string representation of the object
    @Override
    public String toString() {
        return "Person [Nama=" + nama + ", Jenis Kelamin=" + jenisKelamin + ", Umur=" + umur + "]";
    }

    public static void main(String[] args) {
        // Create two objects from the Person class
        Person Anton = new Person("Anton", "Laki-laki", 25);
        Person Riko = new Person("Riko", "Laki-laki", 30);

        // Print the attributes of each object
        System.out.println("Anton's details:");
        System.out.println(Anton); // Automatically calls Anton's toString method

        System.out.println("\nRiko's details:");
        System.out.println(Riko); // Automatically calls Riko's toString method
    }
}

