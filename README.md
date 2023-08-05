# Project 2 : Person Tracking
Person Tracking merupakan Project ke-2 dari Indonesia.AI dalam menyelesaikan Bootcamp Computer Vision Specialist.

#### Author : Teguh Prasetyo

## Pendahuluan
Person tracking atau secara umum object tracking, merupakan pengaplikasian object detection pada video atau live video seperti pada CCTV, WebCam dan lain sebagainya. Teknologi ini merupakan bagian dari bidang AI yang banyak diaplikasikan dalam kehidupan sehari-hari yaitu Computer Vision, dimana computer dilatih untuk dapat mengenali image (citra). Pada person tracking computer dilatih untuk dapat mendeteksi wilayah pada citra (foto) yang merupakan manusia atau bagian tubuh manusia. Person tracking ini sangat bermanfaat dalam kehidupan sehari-hari, misalnya untuk mendeteksi jarak antar pedestrian ketika masa Pandemi Covid-19, menghitung jumlah pejalan kaki di pedestrian, menghitung jumlah pengunjung suatu mall atau toko, mendeteksi suhu tubuh yang diaplikasikan ke kamera termal dan lain sebagainya.

## Objektif

Project ini bertujuan untuk melakukan eksperimen dengan 2 algoritma Deep Learning untuk Object Detection populer yaitu Faster R-CNN dan YOLO dan mengoptimalkan penggunaannya dengan melakukan hyperparameter tuning. Kemudian dari hasil eksperimen tersebut akan dilakukan pengambilan kesimpulan algoritma terbaik.

## Dataset

Image dataset yang digunakan dalam project ini diperoleh dari [Roboflow](https://universe.roboflow.com/dudrn5704-naver-com/coco2017-3000-person-ver) terdiri dari 2700 images.

#############

|
|
V
Belum di edit

## Metodologi

Training model deep learning menggunakan library keras dan tensorflow. Lebih detail dapat dilihat pada notebook.

Dalam proses penyelesaian tugas eksperimen dibuat bertahap, sehingga tahapannya membuat eksperimen dengan VGG-19 dahulu melalui eksperimen 1, 2 dan 3. Hasil terbaik dari eksperimen dengan VGG-19 tersebut kemudian di gunakan Model parameternya untuk pengerjaan dengan algoritma ResNet-50 dan GoogleNet (Inception-V3) untuk perbandingan.

Berikut List Filenya :

VGG-19 
* Eksperimen 1 : nama file -> Face Recognition tf vgg epoch 10 Exp 1 @ Teguh.ipynb
* Eksperimen 2 : nama file -> Face Recognition tf vgg epoch 10 Exp 2 @ Teguh.ipynb
* Eksperimen 3 : nama file -> Face Recognition tf vgg epoch 20 Exp 3 @ Teguh.ipynb

Pada eksperimen menggunakan VGG-19, hasil terbaik adalah pada Eksperimen 2, sehingga untuk algoritma ResNet dan GoogleNet menggunakan parameter yang sama dengan VGG-19 eksperimen 2.

ResNet-50
* Eksperimen 2 : nama file -> Face Recognition tf resnet epoch 10 Exp 2 @ Teguh.ipynb

GoogleNet (Inception-V3)
* Eksperimen 2 : nama file -> Face Recognition tf inceptionv3 epoch 10 Exp 2 @ Teguh.ipynb

## Hasil

![Perbandingan Algoritma VGG-Resnet-Googlenet](https://github.com/tprasetyo/Face-Recognition/assets/72024376/71327b82-49f9-47e8-8088-ae61dc0706f3)

Hasil terbaik adalah dengan menggunakan algoritma ResNet-50 dengan accuracy 0.95.

Catatan: Training menggunakan CPU dengan IDE VSCode 

## Kesimpulan

* Penggunaan Transfer Learning pada task Gender Classification dapat memberikan hasil akurasi yang tinggi 
* Tuning parameter seperti jumlah dense layer, fine tuning, loss function, dll bisa memiliki pengaruh terhadap hasil akurasi
* Transfer Learning bisa mendapatkan akurasi yang cukup baik walaupun hanya menggunakan data yang lebih sedikit.

## Contact

Teguh Prasetyo

[Email](mailto:teguh.prasetyo33@gmail.com) | [Linkedin](https://id.linkedin.com/in/teguh-prasetyo-b4196879)
