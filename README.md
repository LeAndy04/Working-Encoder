pip uninstall opencv-python #get rid of regular opencv, won't work with encoder.
pip install opencv-python-headless #install THIS, this is the one you want.

Go into encoder and find videolocation, replace videoLocation = r"VIDEOPATHHERE"
Run encoder for the json packets. YOU WILL NOT GET CONFIG FILE YET! Push json packets into main

Go into encoder and comment out lines 153 and 154 like this
#videoCapture.release()
#cv.destroyAllWindows()

Run encoder only for the config file. Commit and push into main.
You should have the json packets and config file.

