1. First, obtain varied images of toy cars in the desired location
2. Label these images utilizing the Label Studios Software. 
3. Run these images through the Augments_9PerImage to increase the variety. If more images are desired, the number of augments per image can be changed by modifying the num_augmentations variable inside the file. 
4. Then, upload these new images and labels into Google Colab. If images are not uploading, utilize tools such as XnConvert to reduce quality and size of images
5. Upload directly to open source Google Colab(Train_YOLO_Models.ipynb) and follow the instructions to train the AI model
6. Upon concluding training, move the downloaded file with the AI model onto the Raspberry Pi
7. Establish a venv and install necessary packages on Raspberry Pi (install ultralytics ncnn)
8. Import index1.html and yolo_web_testing_headless_with_live.py to Raspberry Pi
9. Start running server using: python3 yolo_web_testing_headless_with_live.py --model=my_model4_ncnn_model --source=usb0 --resolution=1280x640 --headless
