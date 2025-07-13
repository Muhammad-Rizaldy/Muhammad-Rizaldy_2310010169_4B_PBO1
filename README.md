# Proyek Akhir Pemrograman Berbasis Objek 1

Proyek ini adalah contoh sederhana aplikasi pengolahan data calon polisi menggunakan Java sebagai tugas akhir dari mata kuliah pemrograman berbasis objek 1.

## Deskripsi

Aplikasi ini menerima input berupa nama, umur, golongan, dan nilai tes calon polisi, dan memberikan output berupa status kelulusan berdasarkan syarat umur dan nilai minimal.

Aplikasi ini mengimplementasikan beberapa konsep penting dalam pemrograman berorientasi objek (OOP) seperti Class, Object, Atribut, Method Constructor, Method Mutator, Method Accessor, Encapsulation, Inheritance, Overriding, Seleksi, Perulangan, IO Sederhana, Array, dan Error Handling.

## Penjelasan Kode

Berikut adalah bagian kode yang relevan dengan konsep OOP yang dijelaskan:

1. **Class** adalah template atau blueprint dari object. Pada kode ini, CalonPolisi, PolisiLulus, dan PenerimaanPolisi adalah contoh dari class.

```bash
public class CalonPolisi {
    ...
}

public class PolisiLulus extends CalonPolisi {
    ...
}

public class PenerimaanPolisi {
    ...
}
```

2. **Object** adalah instance dari class. Pada kode ini,daftar[i] = new PolisiLulus(...) adalah contoh pembuatan object.

```bash
daftar[i] = new PolisiLulus(nama, umur, golongan, nilai);
```

3. **Atribut** adalah variabel yang ada dalam class. Pada kode ini, nama, umur, golongan, dan nilaiTes adalah contoh atribut.

```bash
private String nama;
private int umur;
private String golongan;
private double nilaiTes;
```

4. **Constructor** adalah method yang pertama kali dijalankan pada saat pembuatan object. Pada kode ini, constructor ada di dalam class CalonPolisi dan PolisiLulus.

```bash
public CalonPolisi(String nama, int umur, String golongan, double nilaiTes) {
    ...
}

public PolisiLulus(String nama, int umur, String golongan, double nilaiTes) {
    super(nama, umur, golongan, nilaiTes);
}
```

5. **Mutator** atau setter digunakan untuk mengubah nilai dari suatu atribut. Pada kode ini, setNama, setUmur, setGolongan, dan setNilaiTes adalah contoh method mutator.

```bash
public void setNama(String nama) { this.nama = nama; }
public void setUmur(int umur) { this.umur = umur; }
public void setGolongan(String golongan) { this.golongan = golongan; }
public void setNilaiTes(double nilaiTes) { this.nilaiTes = nilaiTes; }
```

6. **Accessor** atau getter digunakan untuk mengambil nilai dari suatu atribut. Pada kode ini,getNama, getUmur, getGolongan, dan getNilaiTes adalah contoh method accessor.

```bash
public String getNama() { return nama; }
public int getUmur() { return umur; }
public String getGolongan() { return golongan; }
public double getNilaiTes() { return nilaiTes; }
```

7. **Encapsulation** adalah konsep menyembunyikan data dengan membuat atribut menjadi private dan hanya bisa diakses melalui method. Pada kode ini, atribut nama, umur, golongan, dan nilaiTes dienkapsulasi dan hanya bisa diakses melalui method getter dan setter.

```bash
private String nama;
private int umur;
private String golongan;
private double nilaiTes;
```

8. **Inheritance** adalah konsep di mana sebuah class bisa mewarisi property dan method dari class lain. Pada kode ini, PolisiLulus mewarisi CalonPolisi dengan sintaks extends.

```bash
public class PolisiLulus extends CalonPolisi {
    ...
}
```

9. **Polymorphism** adalah konsep di mana sebuah nama dapat digunakan untuk merujuk ke beberapa tipe atau bentuk objek berbeda. Ini memungkinkan metode-metode dengan nama yang sama untuk berperilaku berbeda tergantung pada tipe objek yang mereka manipulasi, polymorphism bisa berbentuk Overloading ataupun Overriding. Pada kode ini, method statusKelulusan() di PolisiLulus merupakan override dari method di class induk (walaupun tidak dituliskan di superclass).

```bash
public String statusKelulusan() {
    if (getNilaiTes() >= 75 && getUmur() >= 18) {
        return "Lulus";
    } else {
        return "Tidak Lulus";
    }
}
```

10. **Seleksi** adalah statement kontrol yang digunakan untuk membuat keputusan berdasarkan kondisi. Pada kode ini, digunakan seleksi if else dalam method statusKelulusan.

```bash
if (getNilaiTes() >= 75 && getUmur() >= 18) {
    return "Lulus";
} else {
    return "Tidak Lulus";
}
```

11. **Perulangan** adalah statement kontrol yang digunakan untuk menjalankan blok kode berulang kali. Pada kode ini, digunakan loop for untuk meminta input dan menampilkan data.


```bash
for (int i = 0; i < jumlah; i++) {
    ...
}
```

12. **Input Output Sederhana** digunakan untuk menerima input dari user dan menampilkan output ke user. Pada kode ini, digunakan class Scanner untuk menerima input dan method System.out.println untuk menampilkan output.

```bash
Scanner input = new Scanner(System.in);
System.out.print("Nama: ");
System.out.println(p.getNama());
```

13. **Array** adalah struktur data yang digunakan untuk menyimpan beberapa nilai dalam satu variabel. Pada kode ini, PolisiLulus[] daftar = new PolisiLulus[jumlah]; adalah contoh penggunaan array.

```bash
PolisiLulus[] daftar = new PolisiLulus[jumlah];
```

14. **Error Handling** digunakan untuk menangani error yang mungkin terjadi saat runtime. Pada kode ini, digunakan try catch untuk menangani input tidak valid.


```bash
try {
    ...
} catch (NumberFormatException e) {
    System.out.println("Input harus berupa angka!");
}
```

## Usulan nilai

| No  | Materi         |  Nilai  |
| :-: | -------------- | :-----: |
|  1  | Class          |    5    |
|  2  | Object         |    5    |
|  3  | Atribut        |    5    |
|  4  | Constructor    |    5    |
|  5  | Mutator        |    5    |
|  6  | Accessor       |    5    |
|  7  | Encapsulation  |    5    |
|  8  | Inheritance    |    5    |
|  9  | Polymorphism   |   10    |
| 10  | Seleksi        |    5    |
| 11  | Perulangan     |    5    |
| 12  | IO Sederhana   |   10    |
| 13  | Array          |   15    |
| 14  | Error Handling |   15    |
|     | **TOTAL**      | **100** |

## Pembuat

Nama: Muhammad Rizaldy
NPM: 2310010169
