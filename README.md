##latihan1.cpp : Susun algoritma untuk menginput bilangan sebanyak - banyaknya sampai kondisi dimasukkan angka 0 (nol).

**Alur algoritma**
1. Mendeklarasikan variabel 'int max, a;' sebagai variable input.
2. Membaca input dari keyboard 'cin >> a;'
3. Membandingkan nilai variable (max<a)
            			 max=a;

**Flowchart Program**
![Flowchart](https://raw.githubusercontent.com/raihan11/Praktikum4/master/Latihan1.cpp/Flowchart1.jpg)

**Screenshoot**
![Screenshoot](https://raw.githubusercontent.com/raihan11/Praktikum4/master/Latihan1.cpp/Screenshoot1.png)

**code program lengkap**
'''c++
#include <iostream>
using namespace std;
int main()
{
    int max, a;
    max=0;

    do{
        cout << "masukkan bilangan : "; cin >> a;
        if (max<a)
            max=a;
    } while (a!=0);
    cout << "bilangan terbesar adalah; " <<max<< endl;
    return 0;
}


###latihan2.cpp : Susun algoritma untuk menginput sejumlah N barang, dengan rindian dua buah bilangan bulat yang masing - masing merupakan jumlah dan harga satuan suatu barang yang dibeli.

**Alur algoritma**
1. Mendeklarasikan variabel 'int jumlah_beli=0,total_beli=0,x,y,a;' sebagai variable input.
2. Membaca input dari keyboard 'cin >> a >> jumlah_beli >> harga'
3. Membandingkan nilai variable  harga=0,harga_barang=0,total=0,bayar=0,diskon;

**Flowchart Program**
![Flowchart](https://raw.githubusercontent.com/raihan11/Praktikum4/master/Latihan2.cpp/flowchart2.jpg)

**Screenshoot**
![Screenshoot](https://raw.githubusercontent.com/raihan11/Praktikum4/master/Latihan2.cpp/Screenshoot2.png)

**code program lengkap**
'''c++
#include <iostream>
using namespace std;
int main ()
{
     cout<< "Tugas Praktikum4"<< "Program Menghitung Total Belanja"<< endl;
     cout<< "====================================================="<< endl;
     int jumlah_beli=0,total_beli=0,x,y,a;
     long int
     harga=0,harga_barang=0,total=0,bayar=0,diskon;
     cout<< "Masukan Jumlah Barang (N) : "; cin>>y;
     x=1;

     while(x<=y)
     {
         cout<< "Barang Ke-"; cin>>a;
         cout<< "Masukan Banyaknya Barang: "; cin>>jumlah_beli;
         cout<< "Masukan Harga Barang:Rp"; cin>>harga;
         harga_barang = harga*jumlah_beli;
         total=total + harga_barang;
         total_beli += jumlah_beli;
         x++;
    }
    if(total>=1000000)
    {

        diskon=total*10/100;
    }
    else if (total>500000&&total<1000000)
    {

        diskon=total*5/100;
    }else{
    diskon=0;
    }# Praktikum4
