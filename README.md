```
# Ujian Akhir Semester 
<br>Mata Kuliah  : Dasar Pemrograman
<br>Nama  : Imelia Destriani
<br>NIM  : 1227050057
<br>Jurusan  :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
  
       Matriks adalah kumpulan bilangan atau simbol yang tertata rapi menurut baris dan kolom berbentuk segi empat. Bilangan-bilangan atau simbol-simbol yang terdapat
    dalam suatu matriks disebut dengan elemen-elemen matriks. Suatu matriks biasanyadiberi nama dengan huruf kapital dan ditulis tebal. Elemen-elemen matriks biasanya
    diberi nama dengan huruf kecil yang sama dengan nama matriks tersebut disertai 2 indeks bawah yang menunjukkan letaknya di dalam matriks. Indeks pertamamenunjukkan
    baris sedangkan indeks kedua menunjukkan kolom. Jika salah satudari baris dan kolom suatu matriks jumlahnya hanya satu maka elemen matrikstersebut hanya memiliki
    satu indeks. Matriks yang hanya memiliki satu indeks disebut dengan vektor.
        Dalam bahasa pemrograman, suatu matriks direpresentasikan oleh array 2 dimensi sedangkan vektor direpresentasikan oleh array 1 dimensi. Elemen-elemen array
    biasanya ditulis dengan huruf besar disertai indeksnya yang berada di dalam kurung. Terdapat perbedaan mengenai cara penulisan indeks array antara bahasa C++
    dan bahasa pemrograman lain. Elemen-elemen matriks yang dinotasikan dengan a (ij) tertulis A(i,j) dalam bahasa Fortran dan A[i][j] dalam bahasa C++

## Source Code

  1. Input, bnyknya baris kolom banyak baris dan banyak data
     Tukar baris jadi kolom kolom jadi baris
     
     #include <iostream>
     using namespace std;

     int main (){
	      string nama = "Imelia Destriani";
	      string nim = "1227050057";
	
	      cout<<"========================="<<endl;
	      cout<<"Nama : "<<nama<<endl;
	      cout<<"NIM  : "<<nim<<endl;
	      cout<<"========================="<<endl<<endl;
	
	      int A [20][20];
	      int b, k, i, j;
	      cout << "Masukkan jumlah baris : ";
	      cin >> b;
	      cout << "Masukkan jumlah kolom : ";
	      cin >> k;
	
	      cout<<endl;
	
	      for (i=0;i<=b-1;i++) {
		      for(j=0;j<=k-1;j++) {
			      cout << "Masukkan nilai (" << i << "." << j << ") : ";
			      cin >> A [i][j];
		      }
	      }
	
	      cout<<endl;
	
	      cout << "Nilai yang diinputkan : \n";
	      for(int i = 0; i < b; i++){
		      for(int j = 0; j < k; j++){
			      cout<<A[i][j]<<"\t";
		      }
		      cout<<endl;
	      }
	
	      cout<<endl;
	
	      cout << "Nilai setelah diacak : "<<endl;
  	      for (int i = 0; i < b ; i++) {
   		      for (int j = 0; j < k; j++) {
     		      cout << A [j][i] << "\t";
   		      }
   		      cout << endl;
  	      }
      }


  2. Baris dan kolom tentukan banyaknya dan isikan data dan beda akhirnya, tampilkan bilangan habis dibagi 3,5,7

    
      #include <iostream>
      using namespace std;

      int main(){
	      string nama = "Imelia Destriani";
	      string nim = "1227050057";
	
    
	      cout<<"========================="<<endl;
	      cout<<"Nama : "<<nama<<endl;
	      cout<<"NIM  : "<<nim<<endl;
	      cout<<"========================="<<endl<<endl;
	
        int A [20][20], b, k, i, j, baris, kolom;

   
        cout<<"Masukkan jumlah baris : "; cin>>b;
        cout<<"Masukkan jumlah kolom : "; cin>>k;
        cout << endl;

        for(i = 0; i < b; i++){
            for(j = 0; j < k; j++){
               cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
               cin >> A [i][j];
              }
             cout << endl;
          }

   	    cout << "Nilai yang diinputkan : \n";
	      for(int i = 0; i < b; i++){
		      for(int j = 0; j < k; j++){
			      cout<<A[i][j]<<"\t";
		      }
		      cout<<endl;
	      }
	
       cout << "\nBilangan yang habis dibagi 3 : ";
       for(i = 0; i < b ; i++){
            for(j = 0; j < k; j++){
                if(A [i][j] % 3 == 0){
                    cout << A [i][j] << " ";
                 }
              }
	      }
	      cout << endl;
        cout << "\nBilangan yang habis dibagi 5 : ";
        for(i = 0; i < b ; i++){
            for(j = 0; j < k; j++){
                if(A [i][j] % 5 == 0){
                cout << A [i][j] << " ";
               }
		      }
        }
        cout << endl;


        cout << "\nBilangan yang habis dibagi 7 : ";
        for(i = 0; i < b ; i++){
              for(j = 0; j < k; j++){
                 if(A [i][j] % 7 == 0){
                 cout << A [i][j] << " ";
             }
    	     }
	      }
        cout << endl;
      }


## Output

    1. Input, bnyknya baris kolom banyak baris dan banyak data
       Tukar baris jadi kolom kolom jadi baris
    
       =========================
       Nama : Imelia Destriani
       NIM  : 1227050057
       =========================

       Masukkan jumlah baris : 2
       Masukkan jumlah kolom : 2

       Masukkan nilai (0.0) : 1
       Masukkan nilai (0.1) : 2
       Masukkan nilai (1.0) : 6
       Masukkan nilai (1.1) : 7

       Nilai yang diinputkan :
       1       2
       6       7

       Nilai setelah diacak :
       1       6
       2       7

       --------------------------------
       Process exited after 8.325 seconds with return value 0
       Press any key to continue . . .
       
       
       
  2.  Baris dan kolom tentukan banyaknya dan isikan data dan beda akhirnya, tampilkan bilangan habis dibagi 3,5,7
  
      =========================
      Nama : Imelia Destriani
      NIM  : 1227050057
      =========================

      Masukkan jumlah baris : 2
      Masukkan jumlah kolom : 2

      Baris 1, kolom 1 = 1
      Baris 1, kolom 2 = 3

      Baris 2, kolom 1 = 5
      Baris 2, kolom 2 = 7

      Nilai yang diinputkan :
      1       3
      5       7

      Bilangan yang habis dibagi 3 : 3

      Bilangan yang habis dibagi 5 : 5

      Bilangan yang habis dibagi 7 : 7

      --------------------------------
      Process exited after 3.918 seconds with return value 0
      Press any key to continue . . .
