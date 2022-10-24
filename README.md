# Спринт 2
## Часть 1
### Настройка пайплайна для сборки приложения по тэгу и отправки в DockerHub

1. Создаем секреты содержащие логин и пароль доступа к DockerHub

![github_secrets](https://user-images.githubusercontent.com/3630798/197543369-ff5e3fa8-1c64-484a-b488-252770217399.png)

2. Клонируем репазиторий на рабочую машину
```console
git clone git@github.com:vggalkin/django-pg-docker.git
cd django-pg-docker
```
3. Создаем файл пайплайна 

[Docker Image CD](.github/workflows/docker_image_cd.yml)
