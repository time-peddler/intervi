## question 1
./analyst_question1.ipynb

## question 2
./analyst_question2.ipynb

## question 3

```sql
select City 
from Stu
group by City
having count(Name) > 3
```

## question 4

```python3
import re
from collections import Counter

text = """Mr. Dursley was the director of a firm called Grunning, which made drills. He was a big, beefy man with hardly any neck, although he did have a very large mustache. Mrs. Dursley was thin and blonde and had nearly twice the usual amount of neck, which came in very useful as she spent so much of her time craning over garden fences, spying on the neighbors."""

# 分词
words = re.findall(r"\w+", text.lower()) 

# 统计词频
word_count = Counter(words)  

# 获取前3高频词
top3_words = word_count.most_common(3)

print(top3_words)
```

## question 5

##### ANSWER:
regex_pattern = None
尝试了很多办法，确实不会。

## question 6

##### 1.在淘宝上搜索“马克杯”产品,按销量排名，找出销量前10名产品的销售量,分别为20万+ 2万+10万+50万+10万+5000+5万+2万+3万+2万，共约100W。
##### 2.通过这10个样本粗略估计淘宝马克杯类产品的年销售量,销量前10名产品销量100万,则全年全站约为1000万个。
##### 3.可以引进的产品有：
* https://item.taobao.com/item.htm?abbucket=6&id=620401452086&ns=1&spm=a21n57.1.0.0.1957523cAzIHws
* https://detail.tmall.com/item.htm?abbucket=6&id=718683283225&ns=1&spm=a21n57.1.0.0.1957523cAzIHws

##### 4.理由如下：
* 销量可观
* 外形设计优美大方,能够吸引女性消费群体
* 客户评价较为中肯,如不易破损,容量适中,防烫手等

## question 7

##### 管理方式及理由：
- 分析类目内马克杯的历史销量、价格区间、消费群体等数据,了解类目整体情况。
- 根据销量和用户评分,找到类目内口碑及销量较好的前10名卖家,与他们深入合作。提供更好的服务及资源支持,鼓励他们增加更多优质产品。
- 与优质新卖家开展新品试销合作,邀请优秀设计师参与,丰富马克杯在类目内的样式及价格层级。
- 定期开展马克杯类目促销活动,针对不同节日、群体开展定向营销,进一步扩大销量。
