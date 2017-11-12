## List Comprehension

파이선에서 변환시킨 결과를 list 로 저장할 때 수식 채로 list 에 표현한다.

```python
# list
even_numbers = [x for x in range(5) if x % 2 == 0]
squares = [x * x for x in range(5)]
even_squars = [x * x for x in even_numbers]

# dict
square_dict = { x : x * x for in range(5) }

# set
square_set = { x * x for x in [1, -1] }
```
불필요한 값은 _로 표기
```python
zeros = [0 for _ in even_numbers]
```
여러 개의 for 을 포함 가능
```python
pairs = [(x, y)
        for x in range(10)
        for y in range(10)]
```
