### 데이터 소개

마스크 유/무 구별

### 사용된 하이퍼파라미터 
- epoch 2
- batch-size 30
- weights yolov5m.pt
- patience 0

      python3 src/yolov5/train_xpu.py --data /home/intel/Downloads/mask/data.yaml --weights yolov5m.pt --epochs 2 --patience 0  --batch 30  --name rps_yolov5m_xpu_mask


### 트레이닝 결과
```sh
  Model summary: 212 layers, 20861016 parameters, 0 gradients, 47.9 GFLOPs
                 Class     Images  Instances          P          R      mAP50   mAP50-95: 
                   all        576        400      0.702      0.653      0.727      0.433
                  mask        576        139      0.832      0.426      0.638      0.348
               no-mask        576        141      0.515      0.858      0.781      0.465
                unkown        576        120      0.761      0.675      0.763      0.486
```

### inference 예제




