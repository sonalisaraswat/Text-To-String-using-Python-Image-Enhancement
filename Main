import pytesseract as tess
tess.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'
from PIL import Image,ImageEnhance

name = input()

enhancer = ImageEnhance.Sharpness(Image.open(str(name)))
enhancer.enhance(1.5).save(str(name))

enhancer = ImageEnhance.Brightness(Image.open(str(name)))
enhancer.enhance(1.5).save(str(name))

enhancer = ImageEnhance.Contrast(Image.open(str(name)))
enhancer.enhance(1.5).save(str(name))

text = tess.image_to_string(Image.open(str(name)))
print(text)
