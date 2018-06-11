# Barcode-extraction-for-paypal
The app takes input an image checks if its a valid tracking document or not and returns the tracking document in text format

Extracting Content From Image
To run this Module pip 9.0.3 and python 3.5 must be setup
```sh
pip install -r requirements.txt
./run.sh
```
About the Indiviaual Modules
## 1-Resize.py
It opens the image and resizes it to a particular size which is the thresholding criteria for tesseract
## 2-Findcontours.py
It finds all possible contours in an image(Contours are region with same light intensity)
## 3-barcodes
Localises the area below the top 5 contours
## 4-rotate.py
Straightens the image if rotated
## 5-rotate.py
Straightens the image if rotated with 90-theta
## 6-NlP.py
Does natural processing of the text validates it and returns barcode if present
## 7-Main.py
Combines all the modules
