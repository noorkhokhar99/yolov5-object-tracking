# yolov5-object-tracking

### New Features
- YOLOv5 Object Tracking Using Sort Tracker
- Added Object blurring Option
- Added Support of Streamlit Dashboard
- Code can run on Both (CPU & GPU)
- Video/WebCam/External Camera/IP Stream Supported


### Pre-Requsities
- Python 3.9 

### Steps to run Code
- Clone the repository
```
git clone https://github.com/noorkhokhar99/yolov5-object-tracking.git
```

- Goto the cloned folder.
```
cd yolov5-object-tracking
```


```

- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```

- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```

```
- Run the code with mentioned command below.
```


#for detection only
python ob_detect.py --weights yolov5s.pt --source "your video.mp4"

#for detection of specific class (person)
python ob_detect.py --weights yolov5s.pt --source "your video.mp4" --classes 0

#for object detection + object tracking
python obj_det_and_trk.py --weights yolov5s.pt --source "your video.mp4"

#for object detection + object tracking + object blurring
python obj_det_and_trk.py --weights yolov5s.pt --source "your video.mp4" --blur-obj

#for object detection + object tracking + object blurring + different color for every bounding box
python obj_det_and_trk.py --weights yolov5s.pt --source "your video.mp4" --blur-obj --color-box

#for object detection + object tracking of specific class (person)
python obj_det_and_trk.py --weights yolov5s.pt --source "your video.mp4" --classes 0
```

- Output file will be created in the working-dir/runs/detect/exp with original filename

### Streamlit Dashboard
- If you want to run detection on streamlit app (Dashboard), you can use mentioned command below.

<b>Note:</b> Make sure, to add video in the <b>yolov5-object-tracking</b> folder, that you want to run on streamlit dashboard. Otherwise streamlit server will through an error.
```
python -m streamlit run app.py
```

# result 
<img src="https://github.com/noorkhokhar99/yolov5-object-tracking/blob/main/Screen%20Shot%201444-03-27%20at%2011.49.29%20PM.png">


