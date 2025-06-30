# TrackNet-Sports

Player Re-identification Using YOLOv11 and Deep SORT

This project performs player tracking and re-identification in a 15-second sports video using YOLOv11 for object detection and Deep SORT for tracking.

🚀 Features

Player detection using a trained YOLOv11 model (best.pt)
Re-identification across frames with Deep SORT
Output annotated video with consistent IDs for each tracked player.

⚙️ Setup Instructions

1. Clone the Repository & Navigate
cd your-project-directory

2. Install Dependencies
Create a virtual environment (optional but recommended):
python3 -m venv venv
source venv/bin/activate

Install required packages:

pip install ultralytics opencv-python deep_sort_realtime
Note: If cv2 doesn't install correctly, ensure GTK support:
sudo apt-get install libgtk2.0-dev pkg-config


⚡ Running the Project

python player_reid_final.py

This will:
Load the YOLOv11 model
Run inference on 15sec_input_720p.mp4
Apply Deep SORT to track players.
Output output.mp4 with bounding boxes and track IDs

✅ Output

Bounding boxes around players
Re-identified player IDs retained across frames
