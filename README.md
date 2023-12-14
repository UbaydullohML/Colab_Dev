# Table of Contents
* [Google drive](#google_drive)

## Google_drive
how to mounting, accessing from drive folder

    from google.colab import drive
    drive.mount('/content/drive')

and copytree to google drive folder 

    import shutil
    import os

    #source_file_path = '/content/sample.txt'

    source_dir_path = '/content/yolov7'
    destination_folder_path = '/content/drive/MyDrive/yolov7/yolov7onnx'

    # Check if the directory exists at the destination
    if os.path.exists(destination_folder_path):
        print(f"The directory {destination_folder_path} already exists.")
    else:
        # shutil.copy(source_file_path, destination_folder_path)
        shutil.copytree(source_dir_path, destination_folder_path)

![image](https://github.com/UbaydullohML/Colab_Dev/assets/75980506/ab3a49e2-bbc1-4f0a-9825-1d90d8251848)

