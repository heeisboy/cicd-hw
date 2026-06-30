## Дополнительные материалы для выполнения домашних заданий из блока "Введение в DevOps"


- [Дополнительный материал для занятия "8.2. Что такое DevOps. СI/СD"](CICD/8.2-hw.md)

- [Дополнительный материал для занятия "8.3. GitLab"](https://github.com/netology-code/sdvps-materials/tree/main/gitlab)


## Домашнее задание к занятию «Что такое DevOps. СI/СD»

### Задание 1

Что нужно сделать:

    Установите себе jenkins по инструкции из лекции или любым другим способом из официальной документации. Использовать Docker в этом задании нежелательно.
    Установите на машину с jenkins golang.
    Используя свой аккаунт на GitHub, сделайте себе форк репозитория. В этом же репозитории находится дополнительный материал для выполнения ДЗ.
    Создайте в jenkins Freestyle Project, подключите получившийся репозиторий к нему и произведите запуск тестов и сборку проекта go test . и docker build ..

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

---

**Решение:**
- устанавливаем jenkins и golang
<img width="643" height="104" alt="image" src="https://github.com/user-attachments/assets/dd3b4519-c340-4898-bc0c-9fdf00cbef44" />

- запускаем jenkins Freestyle Project включая запуск тестов и сборку проекта ``` go test . && docker build . ``` соответственно
<img width="1024" height="278" alt="image" src="https://github.com/user-attachments/assets/fcb80c9d-6fbc-4873-81ba-95ff226a5ed3" />


---

### Задание 2

Что нужно сделать:

    Создайте новый проект pipeline.
    Перепишите сборку из задания 1 на declarative в виде кода.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

---

**Решение:**

- создаем новый проект pipeline
- переписываем сборку из задания 1 в виде кода
<img width="1266" height="431" alt="image" src="https://github.com/user-attachments/assets/b9e84159-ca14-4d0c-b038-9e83be0bffa3" />

- выполняем. все ок!
<img width="1007" height="310" alt="image" src="https://github.com/user-attachments/assets/9d36da45-a04c-4cbc-83bc-2fdb4b496480" />

---

### Задание 3

Что нужно сделать:

    Установите на машину Nexus.
    Создайте raw-hosted репозиторий.
    Измените pipeline так, чтобы вместо Docker-образа собирался бинарный go-файл. Команду можно скопировать из Dockerfile.
    Загрузите файл в репозиторий с помощью jenkins.

В качестве ответа пришлите скриншоты с настройками проекта и результатами выполнения сборки.

---

**Решение:**

- устанавливаем Nexus
- создаем raw (hosted) репозиторий
- изменяем pipeline и добавляем файл в репозиторий с помощью jenkins
<img width="1448" height="315" alt="image" src="https://github.com/user-attachments/assets/9a2c5d05-72f0-41ed-b6be-333cf275edf7" />
<img width="1905" height="533" alt="image" src="https://github.com/user-attachments/assets/3ca6ecc6-656e-4dd5-8489-3837aa9d9775" />

---

## Практическое задание с самопроверкой «GitLab»

---

### Задание 1

Что нужно сделать:

    Разверните GitLab локально, используя Vagrantfile и инструкцию, описанные в этом репозитории.
    Создайте новый проект и пустой репозиторий в нём.
    Зарегистрируйте gitlab-runner для этого проекта и запустите его в режиме Docker. Раннер можно регистрировать и запускать на той же виртуальной машине, на которой запущен GitLab.

**Решение:**
<img width="1409" height="472" alt="изображение" src="https://github.com/user-attachments/assets/7e9e5995-8535-40c3-bcc4-04b2f386612c" />

---

### Задание 2

Что нужно сделать:

    Запушьте репозиторий на GitLab, изменив origin. Это изучалось на занятии по Git.
    Создайте .gitlab-ci.yml, описав в нём все необходимые, на ваш взгляд, этапы.

**Решение:**
<img width="1384" height="633" alt="изображение" src="https://github.com/user-attachments/assets/3a06bffc-3023-4faa-aa7e-c3f334d26dda" />
<img width="1613" height="346" alt="изображение" src="https://github.com/user-attachments/assets/7cc0b366-b520-4cbd-947f-650827a703fd" />




