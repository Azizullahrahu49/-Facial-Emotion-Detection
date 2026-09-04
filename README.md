# -Facial-Emotion-Detection
This project is a Flask web application that detects facial emotions in real-time using a YOLOv8 model
- Disgusted
- Surprised
- Angry
- Sad
- Happy
- Scared
- Neutral

# -Table of Contents
- Installation
- Usage
- Project Screenshots
- Training Your Own Model
- Project Structure
- License

# -Installation
1. **Clone the repository**: \
```
git clone https://github.com/Azizullahrahu49/facial-emotion-detection.git
cd facial-emotion-detection
```
2. **Set up a virtual environment:**
```
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
```
3. **Install the required dependencies:**
```
pip install -r requirements.txt
```
# -Usage
1. **Run the Flask app:**
```
python app.py
```
2. **Open your web browser and navigate to:**
```
http://127.0.0.1:5000/
```
3. **Upload an image or start the webcam to detect emotions.**

# -Project Screenshots
<img width="1117" height="743" alt="a9354881-051c-488c-ac68-fab837488ebf" src="https://github.com/user-attachments/assets/4041e55b-0106-48b2-b676-9b3fa83546a2" />
<img width="1116" height="742" alt="result" src="https://github.com/user-attachments/assets/3453ea9b-c293-47df-a490-6601558a095d" />

# -Training Your Own Model
If you want to train your own model, follow these steps:
1. **Prepare your dataset**: Ensure your dataset is labeled and formatted correctly for YOLOv8.
2. **Train the model**:
```
python train/train.py
```
The model after training will get stored in the runs directory, copy the .pt file of the model, and paste the file into the model directory.

# -Project Structure
app.py: The main Flask application file.

requirements.txt: List of dependencies required for the project.

templates/: Directory containing HTML templates.

static/: Directory for static files like uploaded images.

models/: Directory containing the trained YOLOv8 model.

train/: Directory containing the training script.

README.md: This documentation file.

# -Acknowledgments
**Roboflow** provided us with a platform for dataset annotation.\
**Ultralytics**, for their pre-trained YOLOv8 weights.

# -License
This project is licensed under the MIT License. See the LICENSE file for details.

Feel free to contribute to this project by opening issues or submitting pull requests. Happy coding!
