# Project 2 : Person Tracking
Person Tracking merupakan Project ke-2 dari Indonesia.AI dalam menyelesaikan Bootcamp Computer Vision Specialist.

#### Author : Teguh Prasetyo

## Pendahuluan
Person tracking atau secara umum object tracking, merupakan pengaplikasian object detection pada video atau live video seperti pada CCTV, WebCam dan lain sebagainya. Teknologi ini merupakan bagian dari bidang AI yang banyak diaplikasikan dalam kehidupan sehari-hari yaitu Computer Vision, dimana computer dilatih untuk dapat mengenali image (citra). Pada person tracking computer dilatih untuk dapat mendeteksi wilayah pada citra (foto) yang merupakan manusia atau bagian tubuh manusia. Person tracking ini sangat bermanfaat dalam kehidupan sehari-hari, misalnya untuk mendeteksi jarak antar pedestrian ketika masa Pandemi Covid-19, menghitung jumlah pejalan kaki di pedestrian, menghitung jumlah pengunjung suatu mall atau toko, mendeteksi suhu tubuh yang diaplikasikan ke kamera termal dan lain sebagainya.

## Objektif

Project ini bertujuan untuk melakukan eksperimen dengan 2 algoritma Deep Learning untuk Object Detection populer yaitu Faster R-CNN dan YOLO dan mengoptimalkan penggunaannya dengan melakukan hyperparameter tuning. Kemudian dari hasil eksperimen tersebut akan dilakukan pengambilan kesimpulan algoritma terbaik.

## Dataset

Image dataset yang digunakan dalam project ini diperoleh dari [Roboflow](https://universe.roboflow.com/dudrn5704-naver-com/coco2017-3000-person-ver) terdiri dari 2700 images dan digunakan untuk mentraining model person tracking dengan YOLO v5, sedangkan dataset dari COCO2017 sebanyak 3500 images digunakan untuk mentraining model person tracking dengan YOLO V8. 

## Metodologi

Proses mendapatkan model dilakukan dengan beberapa tahapan sebagai berikut :
1. Sign in ke Reboflow
2. Upload/Clone Dataset ke Dataset Project di Roboflow
3. Menentukan Data Splitting, Data Augmentasi kemudian membuat code snippet untuk link dataset ke colaboratory
4. Create model YOLO v5 atau v8 melalui menu Model Library, kemudian memasukkan code snippet ke notebook model tersebut.
5. Menjalankan model cell demi cell hingga training dataset selesai
6. Menyimpan model weight
7. Melakukan inference dengan data foto yang baru dan video yang baru (file tidak termasuk dalam training/testing/validation)
8. Selesai

## Contact

Teguh Prasetyo

[Email](mailto:teguh.prasetyo33@gmail.com) | [Linkedin](https://id.linkedin.com/in/teguh-prasetyo-b4196879)
