# tesseract-ocr-s-simple-using
tesseract-ocr's simple using

# download tesseract
```
<!-- introduction -->
https://github.com/tesseract-ocr/tesseract
<!-- Install Tesseract via pre-built binary package -->
https://github.com/UB-Mannheim/tesseract/wiki
```

# install pytesseract


# using tesseract-ocr via python code
```
import pytesseract
from PIL import Image

pytesseract.pytesseract.tesseract_cmd = r'D:\Tesseract-OCR\tesseract.exe'

image = Image.open("image.jpg")
<!-- core code -->
text = pytesseract.image_to_string(image,lang='eng',config='--psm 11')
print(text)
```