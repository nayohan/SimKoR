# SimKoR

 We provide korean sentence text similarity pair dataset using sentiment analysis corpus from [bab2min/corpus](https://github.com/bab2min/corpus).  
 This data crawling korean review from naver shopping website. we reconstruct subset of dataset to make our dataset.

## Dataset description
The original dataset description can be found at the link [[here]](https://github.com/bab2min/corpus/tree/master/sentiment).  


![그림6](https://user-images.githubusercontent.com/54879393/189065508-240b6449-6a26-463f-bd02-64785d76fa02.png)
In korean Contrastive Learning, There are few suitable validation dataset (only KorNLI). To create contrastive learning validation dataset, we changed original sentiment analysis dataset to sentence text similar dataset. Our simkor dataset was created by grouping pair of sentence. Each score [0,1,2,4,5] means how far the meaning is between sentences.

## Data Distribution
Our dataset class consist of text similarity score [0, 1,2,4,5]. each score consists of data of the same size.

<table>
<tr><th>Score</th><th>train</th><th>valid</th><th>test</th></tr>
<tr><th>5</th><th>4,000</th><th>1,000</th><th>1,000</th></tr>
<tr><th>4</th><th>4,000</th><th>1,000</th><th>1,000</th></tr>
<tr><th>2</th><th>4,000</th><th>1,000</th><th>1,000</th></tr>
<tr><th>1</th><th>4,000</th><th>1,000</th><th>1,000</th></tr>
<tr><th>0</th><th>4,000</th><th>1,000</th><th>1,000</th></tr>
<tr><th>All</th><th>20,000</th><th>5,000</th><th>5,000</th></tr>
</table>

## example
```
text1                                               text2                                                 label
고속충전이 안됨ㅠㅠ	                            집에매연냄새없앨려했는데 그냥창문여는게더 공기가좋네요	    5
적당히 맵고 괜찮네요	                            어제 시킨게 벌써 왔어요 ㅎㅎ 배송빠르고 품질양호합니다	    4
다 괜찮은데 배송이 10일이나 걸린게 많이 아쉽네요.    선반 설치하고 나니 주방 베란다 완전 다시 태어났어요~	    2
가격 싸지만 쿠션이 약해 무릎 아파요~ 반품하려구요~   튼튼하고 빨래도 많이 걸 수 있고 잘쓰고 있어요	            1
각인이 찌그저져있고 엉성합니다.	                    처음 해보는 방탈출이었는데 너무 재미있었어요.	            0
```

## Contributors
The main contributors of the work are: 
- [Jaemin Kim](https://github.com/kimfunn)\*
- [Yohan Na](https://github.com/nayohan)\*
- [Kangmin Kim](https://github.com/Gangsss)
- [Sangrak Lee](https://github.com/PangRAK)

\*: Equal Contribution

Hanyang University Data Intelligence Lab (http://dilab.hanyang.ac.kr/) providing support :heart:

You can access datasets in 🤗 [Hugging Face Datasets](https://huggingface.co/datasets/DILAB-HYU/SimKoR)

## License
<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

