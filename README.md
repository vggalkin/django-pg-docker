# Дипломный проект. Спринт 2
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

4. Коммитим и пушим
```console
git add .
git commit -m 'Add pipeline'
git tag -a -m 'Version 1.1.1' v1.1.1
git push origin master
git push origin v1.1.1
```
5. Заходим в на Github в Actions и наблюдаем процесс сборки и отправки в Docker registry

![github_pipeline_1](https://user-images.githubusercontent.com/3630798/197549500-29d82d2a-3b79-4ee9-868b-1fa6e0960305.png)

Завершено

![github_pipeline_2](https://user-images.githubusercontent.com/3630798/197549621-3907e13c-63fa-4aea-8bcf-aa2438eb4268.png)

6. Проверяем на DockerHub

![docker_hub](https://user-images.githubusercontent.com/3630798/197550234-1196a53f-1fc8-44ee-8b2f-6d1f9471635e.png)

## [Часть 2](https://github.com/vggalkin/Helm-charts)
