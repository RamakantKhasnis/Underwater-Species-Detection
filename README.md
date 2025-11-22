# 🐠 Underwater Species Detection using YOLOv8  
### ✔️ Dataset from Roboflow | ✔️ Custom YOLOv8 Training | ✔️ Research Paper Published

This project focuses on **detecting underwater species** such as fish, jellyfish, sharks, and other aquatic life using **YOLOv8**, a state-of-the-art object detection model.  
The project includes dataset preprocessing, training scripts, validation, and inference code.  
You can run the model fully on **VS Code** + **Python**.

---

## 📌 **Features**
- 🐟 Detect multiple underwater species  
- 🧠 Trained using **YOLOv8**  
- 🧾 Published research paper  
- 🗂 Clean dataset structure (`train/`, `valid/`, `test/`)  
- 🚀 Ready-to-run training, testing & inference scripts  
- 🎥 Supports images + videos  

---

## 📂 **Project Structure**
underwater_species_detection/
│
├── data/
│ ├── data.yaml
│ ├── train/
│ ├── valid/
│ ├── test/
│
├── src/
│ ├── train.py
│ ├── predict.py
│ ├── utils.py
│
├── notebook/
│ └── UnderwaterSpeciesYOLO.ipynb
│
├── .gitignore
└── README.md

---

## 🐠 **Dataset**
Dataset used:  
**Aquarium Combined Dataset (Raw - YOLOv8 Format)**  
Provided by **Roboflow**

🔗 **Download Dataset:**  
https://public.roboflow.com/object-detection/aquarium/2

Once downloaded, extract it into:

/data/

---

## 🔧 **Installation**
Clone the repo:git clone https://github.com/RamakantKhasnis/Underwater-Species-Detection.git

cd Underwater-Species-Detection

Create a virtual environment:

python3 -m venv .venv
source .venv/bin/activate

Install dependencies:
pip install ultralytics
pip install opencv-python
pip install matplotlib
---

## 🚀 **Training the Model**

Run:

yolo detect train data=data/data.yaml model=yolov8n.pt epochs=50 imgsz=640


or use the provided script:
python src/train.py


---

## 🔍 **Testing the Model**

After training, run:



python src/predict.py --image path_to_image.jpg


This generates outputs in:



runs/detect/predict/


---

## 📝 **Research Paper**
This project is backed by a **published research paper** on underwater species identification using YOLOv8.



---

## 🎯 **Use Cases**
- Marine biology research  
- Automated analysis of underwater videos  
- Wildlife monitoring  
- Smart surveillance for coral reefs  
- Fish species classification  

---

## 🤝 **Contributions**
Pull requests are welcome.  
If you want enhancements, feel free to open an issue.

---

## ⭐ **Support**
If you found this project helpful, please give it a **⭐ on GitHub!**






