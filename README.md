# NYUDv2-IS
NYUDv2 dataset for COCO-style Instance Segmentation

## Dataset preparation
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
