# shopify-image-repo
### Fall 2021 - Shopify Developer Intern Challenge Question
This program attempts to solve the shopify fall 2021 internship challenge, especially for the adding images part. For now 
the server supports ```.png```, ```.jpg```, and ```.gif``` and the size limit is 1MB.
### How to Run it
Make sure ```python3``` and ```flask``` (```pip install flask``` or ```pip3 install flask```) are installed.
Clone this repo by running ```git clone https://github.com/64g/shopify-image-repo.git```, and run ```sudo python server.py``` 
or ```python server.py```.
In your browser (Google Chrome is recommended) navigate to ```http://127.0.0.1:8080/```
### Test Cases
Sample test files are provided in ```tests``` folder. <br><br>
.png supporting test: Upload ```image1.png```. The image should appear in the web page <br>
.gif supporting test: Upload ```image2.gif```. The image should appear in the web page <br>
.jpg supporting test: Upload ```image3.jpg```. The image should appear in the web page <br>
File supporting negative test: Upload ```text.txt``` . The web page should throw bad request error, since this file is not a image. <br>
Multiple images uploading test: Upload ```image1.png```, ```image2.gif```, ```image3.jpg```. The images should appear in the web page <br>
File size negative test: Upload ```image.jpg``` . The web page should throw value transmitted exceeds the capacity limit error, since this file exceeds the size limit. <br>