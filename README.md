Simply choose a directory (DIR) in which to clone the project using git clone, create a new virtual environment or venv for it (recommended ) and install the requirements using pip install.




user@host:~/DIR$ git clone https://github.com/EONRaider/blackhat-python3
user@host:~/DIR$ python3 -m venv venv
user@host:~/DIR$ source venv/bin/activate
(venv) user@host:~/DIR$ pip install -r requirements.txt

chapter04/arper.py & mail_sniffer.py used the scapy library, which is not compatible with Python 3. For that reason the code has been refactored and now uses the kamene library.
The Network with SCAPY/pic_carver.py now uses the opencv-python library instead of cv2. The "cv2.cv" module was deprecated and has been replaced. The parameter "cv2.cv.CV_HAAR_SCALE_IMAGE" from the original code was replaced by "cv2.CASCADE_SCALE_IMAGE" 
