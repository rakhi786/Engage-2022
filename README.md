# Engage2022
 ## Face Mask Recognition System Using Flask and Tensorflow
 This is project under Microsoft Engage 2022 Mentorship programme aimed at using Computer Vision to detect face mask in real time.The detector created is pretty   accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient and can be used in embeded systems. The project runs on the server whose backend is built using Flask.
 This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed.
 
 ## Project Structure
  #### The structure of the project was as follows -
  1. The project uses caffe based implementation for face and gender detection . The gender detection model is work by Gil Levi and Tal Hassner. Link to the [research paper](https://talhassner.github.io/home/publication/2015_CVPR)
  2. A model was trained on the dataset to sucessfully detect mask on the face using Keras 
  3. The project was then deployed using Flask to run on a webserver.
  4. To improve the fps we have used a custom based I/O technique using threading and added FPS count implementation to calculate fps.
  
  ## 🚀&nbsp; Installation
1. Clone the repo
```
$ git clone https://github.com/rakhi786/Engage-2022.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'venv' or anything you wish. Prefer this option if you want to directly test it using the terminal otherwise install all the dependencies directly on you machine 
3. Preferable Use Linux based OS or in Windows use Anaconda Prompt ([link to install Anaconda](https://www.anaconda.com/products/distribution) ) . To install virtual environment on Windows use the following command
```
$ pip install virtualenv
```
4. To Start Virtual Environment on Windows (use Anaconda Prompt )
```
$ virtualenv venv
$ .\venv\Scripts\activate

```
5. To start Virtual Environment on Linux based OS
```
$ sudo apt install python3-venv
$ python3 -m venv venv
$ source venv/bin/activate
```
6. Linux Users make sure LibGL library is already installed on your system as it is OpenCV dependency. To install it run the following command 
   in your terminal before starting the virtual environment
 ```
 $ sudo apt-get update
 $ sudo apt install -y libgl1-mesa-glx
 ```
7. Now your virtual environment will start. Run the following command to install all the dependencies. Linux Users use pip3 command instead of pip.
```
$ pip install -r requirements.txt
```
7. Run the following command to start the server 
```
$ flask run
```
8. Now Head onto the following server [http://127.0.0.1:5000/](http://127.0.0.1:5000/) or the server mentioned in the command line to access the webpage .
### Optional Features
#### Frame Rate Per Second 
   1. To analyze frames rate per second run the following command. Linux users use python3 instead of python in the terminal
   ```
   $ python Fps_Analysis.py  
   ```
#### Training 
   1. If you want to train the model using your own dataset run the following command. Linux users use python3 instead of python in the terminal
   ```
   $ python train.py --datatset <name of the dataset folder>  
   ```
> **Feel free to contribute ✨**.   
