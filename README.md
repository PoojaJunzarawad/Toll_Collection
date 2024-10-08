---

# Toll Collection System

This project demonstrates a toll collection system using OpenCV for image processing, Tesseract for OCR, and FreeGLUT for OpenGL rendering.

## Step 1: Install Necessary Dependencies

Make sure you have the required libraries installed. Open a terminal and run the following commands:

```bash
sudo apt install build-essential cmake pkg-config
sudo apt install libopencv-dev
sudo apt install tesseract-ocr libtesseract-dev libleptonica-dev
sudo apt install freeglut3 freeglut3-dev
sudo apt install libglu1-mesa libglu1-mesa-dev mesa-common-dev
sudo apt install tesseract-ocr-eng
```

## Step 2: Copy the Code

Save the following code as `toll_collection.cpp`:

```cpp
// Add toll_collection.cpp C++ code here
```

## Step 3: Compile the Program

Run the following command to compile the program:

```bash
g++ -o toll_collection toll_collection.cpp -lGL -lGLU -lglut `pkg-config --cflags --libs opencv4` -ltesseract -llept
```

## Step 4: Run the Program

Execute the compiled program with:

```bash
./toll_collection
```

## Step 5: Interact with the Program

Use the keyboard as described in the code comments:

- Press `1-9` to add different types of vehicles.
- Press `Space Bar` to start/stop the vehicle movement.
- Press `Enter` to process an image for license plate detection.
- Press `i` for instructions.
- Press `p` for toll prices.
- Press `q` to exit and show the total collected toll.
