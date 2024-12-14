# CSE597_Project

This is the repository for my final project for course CSE 597: Vision and Language.

**The code is NOT mine**, and completely belongs to **authors of GitHub Link** https://github.com/chunmeifeng/SPRC, and the paper "Yang Bai, Xinxing Xu, Yong Liu, Salman Khan, Fahad Khan, Wangmeng Zuo, Rick Siow Mong Goh, Chun-Mei Feng. Sentence Level Prompts benefit Composed Image Retrieval". 

To run this code:

```
pip install -r requirements.txt
```

```
python src/blip_fine_tune_2.py \
   --dataset {'CIRR' or 'FashionIQ'} \
   --blip-model-name 'blip2_cir_align_prompt' \
   --num-epochs {'50' for CIRR, '30' for fashionIQ} \
   --num-workers 4 \
   --learning-rate {'1e-5' for CIRR, '2e-5' for fashionIQ} \
   --batch-size 128 \
   --transform targetpad \
   --target-ratio 1.25  \
   --save-training \
   --save-best \
   --validation-frequency 1 
```
