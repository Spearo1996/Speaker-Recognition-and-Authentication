# Speaker-Recognition-and-Authentication

## Libraries Used :
```bash
Python version - 2.7
sounddevice - to record sound  
scipy.io.wavfile - to read .wav file  
commands.getoutput - to use terminal results  
from commands import getoutput as gt  
numpy - for np arrays and their common functions  
matplotlib.pyplot - audio waveforms  
cPickle - t0 save models  
from scipy.io.wavfile import read as rd  
from sklearn.mixture import GaussianMixture as GMM  
from featureextraction import extract_features  
sklearn.mixture   
```

## How to use :
```bash
# Install the required Libraries

# Run main.py
python main.py

```
## Enter 2 for SignUp
![alt text](https://raw.githubusercontent.com/UtkarshBelwal/Speaker-Recognition-and-Authentication/master/images/SignUp.png)
```bash
- Enter your name
- Enter 1 to start recording your voice # 30 seconds of audio will be recorded (5 samples 6 seconds each)
- Enter passcode duration (seconds) # Passcode should have minimum 5 seconds for audible words
- Repeat your passcode 5 times # Speak after "go" is printed on the terminal

A plot of your raw audio and a plot of your audio after preprocessing will be shown
```
## Enter 3 for Changing your Passcode
![alt text](https://raw.githubusercontent.com/UtkarshBelwal/Speaker-Recognition-and-Authentication/master/images/ChangePassword.png)
```bash
- Enter your name
- Enter passcode duration (seconds) # Passcode should have minimum 5 seconds for audible words
- Repeat your passcode 5 times # Speak after "go" is printed on the terminal

A plot of your raw audio and a plot of your audio after preprocessing will be shown
```
## Enter 1 to Login
![alt text](https://raw.githubusercontent.com/UtkarshBelwal/Speaker-Recognition-and-Authentication/master/images/Login.png)
```bash
- Enter 1 to start recording your Passcode
If Authentication is successful:
  "Hello {your_name}, How are you ?"
will be shown on the terminal

If Authentication failed:
  "Hello {closest_model_name}
  Not Authenticated, Try again"
will be shown on the terminal
```
