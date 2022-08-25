# Golang Ubuntu

### Golang

Go adalah bahasa pemrograman yang dibuat di Google pada tahun 2009 oleh Robert Griesemer, Rob Pike, dan Ken Thompson. bahasa pemrograman sumber terbuka yang mudah, sederhana, efisien. Selain itu, Go memiliki level yang sama dengan Java.

1. Pertama-tama sama seperti sebelumnya, kita harus mendownload engine-nya terlebih dahulu.

        wget https://golang.org/dl/go1.16.5.linux-amd64.tar.gz && sudo su
      
image1

        rm -rf /usr/local/go && tar -C /usr/local -xzf go1.16.5.linux-amd64.tar.gz && exit

image1

2. Selanjutnya masukkan path go pada .bashrc

        sudo nano .bashrc

image1

        export PATH=$PATH:/usr/local/go/bin
      
image1

3. Jika sudah sekarang dapat verifikasi go dengan cara berikut.

        go version
      
image1

4. Sekarang kita akan membuat aplikasi sederhana menggunakan go. Kalian dapat menjalankan beberapa perintah berikut ini.

5. Buat sebuah file dengan nama index.go.

        nano index.go
      
6. Setelah itu masukkan script dibawah ini.

   __index.go__

        package main

        import "fmt"

        func main() {
          fmt.Println("Hello World!")
        }

image1

7. Sekarang jalankan aplikasi go dengan menggunakan perintah berikut.

        go run index.go
        
image1

8. Jika aplikasi kalian ingin di build, maka jalankan perintah berikut ini.

        go build index.go
        
image1

9. Jika sudah jalankan aplikasi dengan menggunakan perintah berikut.

        ./index
        
        
        
