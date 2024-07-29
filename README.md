# Model

1. 모델 정의
``` python
# models.py
class Post(models.Model):
    title = models.CharField(max_leng=100)
    content = models.TextField()
```

2. 번역본 생성
``` bash
python manage.py makemigrations
```