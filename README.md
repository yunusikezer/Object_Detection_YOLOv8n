# train-yolov8-custom-dataset-step-by-step-guide

<p align="center">

    
   
</a>
</p>

## dataset

If you want to train yolov8 with your own dataset, this is what you should do:



1. Download your dataset for object detection or you can use your own data. You can download it from [Roboflow](https://public.roboflow.com), [Kaggle](https://www.kaggle.com/datasets) and [Google cloud](https://console.cloud.google.com/marketplace/browse?filter=solution-type:dataset&_ga=2.176674853.121651961.1691138448-1707843902.1691138448&pli=1).
</a>
</p>
    If you have a annotatied data you can directly train your images after some structre arrangement. But if you don`t. No worries you can easly annotate your data with [CVAT](https://www.cvat.ai)

2. Go to **prepare_data** directory.
3. Execute **create_image_list_file.py**.
4. Execute **downloader.py**.

       python downloader.py $IMAGE_LIST_FILE --download_folder=$DOWNLOAD_FOLDER

5. Execute **create_dataset_yolo_format.py**, changing **DATA_ALL_DIR** by **$DOWNLOAD_FOLDER**.
