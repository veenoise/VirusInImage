# Virus in image

This repository is for my activity in out Elective 1: Cybersecurity. The goal of this activity is to hide code inside an image using diffent tools and methods.

In this activity, I was able to hide code inside the image using the following:

- [x] echo
- [x] steghide
- [x] exiftool

## Steghide

![demoSteghide](https://github.com/user-attachments/assets/27d40ea5-bde4-4231-bdbe-1a540c759f9a)

I was able to insert the `secret.txt` inside the `PUPLogo_steghide.jpg` image. You can extract the `secret.txt` using the following command:

```bash
steghide extract -sf PUPLogo_steghide.jpg
```

There is no password set, press enter if prompted.

## Exiftool

![demoExif](https://github.com/user-attachments/assets/c27b7584-013e-4902-8e9e-fb62cca91690)

By manipulating the image's metadata, I was able to insert a text using the parameter `Author:` and set myself as the image's author.

## Echo

![demoEcho](https://github.com/user-attachments/assets/e1735ea0-70af-4f46-9167-ea2c62a0b3de)

Using the command below, I was able to insert a string at the latter part of the image (appeding).

```bash
echo -n "William Eduard M. Chua" >> PUPLogo_exiftool.jpg
```
