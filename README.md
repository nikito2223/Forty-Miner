
## Сборка

Для сборки на Windows:

```Cmd
gradlew deploy
```


Для сборки на Linux:
```shell
./gradlew deploy
```

По окончании сборки все выходные файлы окажутся в директории artifacts, а также в местах для копирования.

## GitHub workflows

При `push` или `pull request` мод собирается на серверах гитхаба, после чего можно скачать полученные артифакты (`annotations`, `core`, `desktop`, `android`).

## Публикация на JitPack.io

Шаблон поддерживает возможность публикации на JitPack.
При сборке проекта в логи выводятся пути зависимостей мода.

Формирование пути зависимости:

`github.[mod group]:[subproject name]:[mod version]`
