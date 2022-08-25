# Golang Ubuntu

### Golang

Go adalah bahasa pemrograman yang dibuat di Google pada tahun 2009 oleh Robert Griesemer, Rob Pike, dan Ken Thompson. bahasa pemrograman sumber terbuka yang mudah, sederhana, efisien. Selain itu, Go memiliki level yang sama dengan Java.

1. Pertama-tama sama seperti sebelumnya, kita harus mendownload engine-nya terlebih dahulu.

        wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
      
![image](https://user-images.githubusercontent.com/40049149/186692466-b6a9abbe-44df-4a44-bad5-305099cc1c84.png)

        rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit

![image](https://user-images.githubusercontent.com/40049149/186693158-cca15b0e-0be4-46dc-a210-e13ed91c78e9.png)

2. Selanjutnya masukkan path go pada __.bashrc__

        sudo nano .bashrc

![image](https://user-images.githubusercontent.com/40049149/186693900-2f96ef53-3d18-4da1-bfad-2d1eba57784b.png)

        export PATH=$PATH:/usr/local/go/bin
      
![image](https://user-images.githubusercontent.com/40049149/186693795-34d964d1-2081-4ee9-b80b-2779bc3b65f3.png)

3. Jika sudah sekarang dapat verifikasi go dengan cara berikut.

        exec bash
        go version
      
![image](https://user-images.githubusercontent.com/40049149/186694757-28d97af6-f400-4d4b-92e7-db1810115d7c.png)

4. Sekarang kita akan membuat aplikasi sederhana menggunakan go. Kalian dapat menjalankan beberapa perintah berikut ini.

5. Buat sebuah file dengan nama __index.go__.

        nano index.go
        
![image](https://user-images.githubusercontent.com/40049149/186695203-8f58fc1c-677c-48f7-b043-957f22c3f57e.png)

6. Setelah itu masukkan script dibawah ini.

   __index.go__

        package main

        import "fmt"

        func main() {
          fmt.Println("Hello World!")
        }

![image](https://user-images.githubusercontent.com/40049149/186695104-327bec28-3b2d-44b7-a27d-3c13debabf46.png)

7. Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.

        go run index.go
        
![image](https://user-images.githubusercontent.com/40049149/186695340-be15f181-1c50-495a-bd26-a4032a9fc04a.png)

8. Jika aplikasi kalian ingin di build, maka jalankan perintah berikut ini.

        go build index.go
        
![image](https://user-images.githubusercontent.com/40049149/186695529-8ee8601b-3f6d-49c6-a5e9-0071f1c91b43.png)

9. Jika sudah jalankan aplikasi dengan menggunakan perintah berikut.

        ./index
        
![image](https://user-images.githubusercontent.com/40049149/186695629-f06c3106-073e-4653-85c4-2d044450d047.png)
        
