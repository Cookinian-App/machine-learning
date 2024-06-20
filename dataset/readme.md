# Cookinian ML

## Object Detection Dataset

We annotate the dataset according to the name of each object. Currently, the dataset included 13 classes:

- _Ayam_
- _Bawang Merah_
- _Bawang Putih_
- _Cabai Hijau_
- _Cabai Merah_
- _Daging Sapi_
- _Ikan_
- _Nasi_
- _Tahu_
- _Telur_
- _Tempe_
- _Tomat_
- _Wortel_

We collected **5200 images**, with a _minimum of 500 labels per class_.

![Contoh gambar dari dataset](link gambar)

## Dataset Preprocessing

The dataset is stored on [**Roboflow**](https://www.roboflow.com). **Roboflow** is a popular tool for preprocessing datasets for object detection.

On **Roboflow**, the dataset undergoes two stages: **preprocessing and data augmentation**. During preprocessing, images are _auto-oriented and resized to 320x320 pixels_. For data augmentation, each image is _rotated twice between 15 degrees and -15 degrees_. Finally, we have **8242 training images, 514 test images, and 516 validation images**.

Here's [our **Roboflow project**](link projek).

## Dataset Export

After augmentation, we export the dataset into **.tfrecord format**, which will be used during modeling. The **.tfrecord dataset** can be found [here](link gdrive).

In addition to the **.tfrecord format**, we also exported the dataset in **VOC format** for image testing. The **VOC dataset** can be found [here](link gdrive juga).
