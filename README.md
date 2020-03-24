# albert

아래 블로그를 보면 albert를 vocab.txt를  생성하는 것부터 pretrainng 및 fine tunning하는 법이 잘 나와 있다.
https://towardsdatascience.com/fine-tune-albert-with-pre-training-on-custom-corpus-f56ea3cfdc82
해당 블로그를 참조하여 naver 영화 리뷰에 대해 pretraining 및 fine tunning을 진행해 봄.

naver의 train data만 사용하여 vocab.txt 및 tfrecord file을 생성했고, train data를 각각 나누어 train, eval, test를 수행.
pretraining 및 fine tunning 모두 약 150000~180000번 정도 진행했고 각각 12시간 내외 걸린 듯.

최종 accuracy는 약 83%가 안되게 나왔는데 하이퍼파라미터 및 step을 변경하면 더 좋아질 것 같다. 
pretraining을 일반적인 corpus에 대해 진행하면 더 잘 나올 것 같은데 computing resource가 부족할 것 같아 naver train data로만 진행함.
