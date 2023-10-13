# NYUDv2-IS
A dataset converted from NYUDv2 into COCO-style instance segmentation format

```
Train : 795 images

Val : 654 images

Classes : 9

Resolution : 640 × 480
```

## Data preparation
https://drive.google.com/drive/folders/1sTvlA5n69tb0gJmAlyvOynNZfCl4dRoq?usp=sharing

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
