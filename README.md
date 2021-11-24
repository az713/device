# device

DEVOPS-17, ПРОЕКТНАЯ РАБОТА 3\n
Abay Zhumageldinov
========================
Git workflow
-------------------------
Расположение кода - code.py

Main – это всегда актуальная версия существующего кода. 

Для каждого нового компонента или функциональности создается отдельная feature-ветка, которая отличается от обычной только префиксом feature/. Это обеспечивает независимую разработку.

Все новые изменения вносятся напрямую в ветку Main через PR. После их должен проверить технический руководитель и провести слияние с веткой Main.

Код который развернут на продакшене помечается меткой prod. Таким образом, работающий продукт и master-код – это не одно и то же.

Install
-------------------------
git clone https://github.com/az713/device

Datasheet for newbies
-------------------------
Начало новой ветки:

git checkout master
git pull
git checkout -b название_нового_бранча

Коммит: 

git add . добавь все в свою локальную репу 

Сохранить - git commit -m "some commit message"

Загрузить свою ветку в репозиторий - git push origin название_ветки

Название можно проверить в IDE или через git status

Финальный мердж:

git checkout master
git pull origin master
git merge название_твоей_ветки
git push origin master