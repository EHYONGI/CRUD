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

3. DB에 반영
``` bash   
python manage.py migrate
```
 
4. superuser 생성
``` bash
python manage.py createsuperuser
```

5. admin에 모델 등록
``` python
from django.contrib import admin
from .models import Post

# Register your models here.
admin.site.register(Post)
```