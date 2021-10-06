# ryanzu_lubiss
Tugas Praktek Bahasa Pemrograman
# Aplikasi Input data siswa

import os 
import sys

class mahasiswa : l-2 (pagi)
	nim='212370100, lanjut'
	nama='RyanzuLeztaLubis, lanjut '

pilih = 0
dataSiswa = [BayuTriKurniawan 212370070, FarhanZainadinZidanGinting 212370053, RyanzuLeztaLubis 212370100]

def menu() :
	os .system('cls')
	print("Menu Aplikasi Data Siswa")
	print("---------------------------------")
	print("1.  Input Data Siswa")
	print("2.  Tampilkan Data Siswa")
	print("3.  Update Data Siswa")
	print("4.  Hapus Data  Siswa")
	print("5.  Author")
	print("6.  Keluar Aplikasi")
	pilih = int(input("Masukkan pilih anda :  "))
	if pilih == 1 :
            pilih1 ()
	    menu ()
	elif pilih == 2 :
	    tampil ()
	    input("kembali menu utama")
	elif pilih == 3 :
 	    index_update=-1
	    tampil ()
	    id_edit = int(input("Input Nim yang akan di update"))
	    for a in range (0, len(dataSiswa)) :
	    	 if id_edit == dataSiswa[a].nim:
		index_update = a
		break
	    if(index update > -1):
	    print("INPUT DATA YANG DI UPDATE ")
	    siswa = Mahasiswa ()
	    siswa.nim = (int(input("masukan nim : ")))
	    siswa.nama = (input("masukan nama siswa : "))
            dataSiswa [index_update] = siswa
            print("berhasil update data siswa")
 	  else : print("nim tidak ditemukan")
	  input("kembali menu utama")
	  menu()
	elif pilih ==4:
	    os.system('cls')
	    tampil()
    	    index_delete=-1
	    id_hapus = int(input("Input Nim yang akan di hapus : ")
	    for a in  range(0, len(datatSiswa):
		if id_edit== dataSiswa[a].nim:
			   index_update = a
			   break
	    if(index_delete > -1):
		del dataSiswa [index_delete]
		print("Data Telah di hapus")
	    else : print("nim tidak ditemukan")
	    input("kembali menu utama")
	    menu()
	elif pilih == 5 :
	    author()
	    input("\n\n kembali menu utama")
	    menu()
	elif pilih ==6 :
	    sys.exit()

def tampil():
        os.system('cls'):
	print("DATA MAHASISWA")
	for data in dataSiswa:
	    print("Nim : 212370100, LANJUT"+str(data.nim))	
	    print("Nama : RyanzuLeztaLubis, LANJUT"+data.nama)
	    print("----------------------")

def author():
	os.system('cls'):
        print("Pakde Edri")
	print("UnHar")

def pilih1():
	ulang = 'Y'
	while ulang in('y', 'Y'):
        os.system('cls')
	siswaBaru = Mahasiswa()
	print("INPUT DATA MAHASISWA ")
	siswaBaru.nim = (int(input("masukan nim : 212370053, LANJUT")))
	siswaBaru.nama = (input("masukan nama siswa :BayuTriKurniawan212370070,FarhanZainadinZidanGinting212370053,RyanzuLeztaLubis212370100 : LANJUT"))
	dataSiswa.append(siswaBaru)
	ulang = input("Apakah Anda Ingin Mengulang (Y/ T)? ")

menu()
