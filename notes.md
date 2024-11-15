Instalacja Django

```commandline
pip install django
```

Utworzenie struktury projektu
```commandline
django-admin startproject youtube
```


```commandline
W folderze youtube
python manage.py startapp ideas
```

polecenie "from django.db import models" umożliwia korzystanie z webowych funkcji, gdzie możemy tworzyć np fieldy:
```commandline
from django.db import models


class Idea(models.Model):
    title = models.CharField(max_length=255)
    description = models.TextField()
    youtube_url = models.URLField()
    
```

Django udostępnia wiele opcji, np. po utworzonym przez django settings.py mamy rózne settingsy do np. skonfigurowania bazy danych

23:00 -> https://www.youtube.com/watch?v=tU6OuVGygLU&list=PL3U271IN44UpfqNWsKQDGzhTimShPaXXy&ab_channel=KacperSieradzi%C5%84ski