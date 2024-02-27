# NYUDv2-IS
A dataset converted from NYUDv2 into COCO-style instance segmentation format 
![image](./img/img1.jpg)

```
Train   : 795 images
Val     : 654 images
Classes : 9
Size    : 640 × 480
Sensor  : Kinect V1
```

## Data preparation

NYUDv2 : https://api.onedrive.com/v1.0/shares/u!aHR0cHM6Ly8xZHJ2Lm1zL3UvcyFBdFEycWtVUmI4dlFya3FSZGtiUWg4cFloZ2dPP2U9U2dmRDRL/root/content

```
NYUDv2/
└── train/
    └── color/
└── val/
    └── color/
└── annotations/
    └── instances_train.json
    └── instances_val.json
└── depth/
└── hha/
```

## Data Format
```
annotation{
    "id": int,
    "image_id": int,
    "category_id": int,
    "segmentation": [polygon],
    "area": float,
    "bbox": [x,y,width,height],
    "iscrowd": 0 or 1,
}

categories[{
    "id": int,
    "name": str,
    "supercategory": str,
}]
```
