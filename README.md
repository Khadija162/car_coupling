# car_coupling

A simple convolutional neural network (CNN) regression model will be used, with images paired with x-coordinate labels derived from the bounding boxes. The task here is not to detect a bounding box, but to predict the horizontal location (x) of the coupling.

car_coupling_finder/

├── data/

    └── train/                   # Extract Images with their corresponding annotations


├── scripts/

    └── prepare_data.py         # This file helps convert the dataset from labelme data format to images as well as x.

    └── train.py                #Allows the training of the CNN model

    └── predict.py              # Script used for performing inference in relation to ./find_couplings


├── model/

    └── coupling_net.pth        # # Trained model (after training process)

├── find_couplings              # The main interface for use from the command line, whether used within a bash shell or through a Python shell.

├── requirements.txt

├── Dockerfile

├── README.md
