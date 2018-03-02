# lab2

## Laboratory work II

Данная лабораторная работа посвещена изучению утилит для разработки проектов

## Tasks

- [ ] 1. Ознакомиться со ссылками учебного материала
- [ ] 2. Выполнить инструкцию учебного материала
- [ ] 3. Составить отчет и отправить ссылку личным сообщением в **Slack**
 
## Tutorial

```bash
$ export GITHUB_USERNAME=<имя_пользователя>
$ export GIST_TOKEN=<сохраненный_токен>
$ alias edit=<nano|vi|vim|subl>
```

```ShellSession
$ mkdir -p ${GITHUB_USERNAME}/workspace
$ cd ${GITHUB_USERNAME}/workspace
$ pwd
$ cd ..
$ pwd
```

```ShellSession
$ mkdir -p workspace/tasks/
$ mkdir -p workspace/projects/
$ mkdir -p workspace/reports/
$ cd workspace
```

```ShellSession
# Debian
$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
$ tar -xf node-v6.11.5-linux-x64.tar.xz
$ rm -rf node-v6.11.5-linux-x64.tar.xz
$ mv node-v6.11.5-linux-x64 node
```

```ShellSession
$ ls node/bin 
$ echo ${PATH}
$ export PATH=${PATH}:`pwd`/node/bin
$ echo ${PATH}
$ mkdir scripts
$ cat > scripts/activate<<EOF
export PATH=\${PATH}:`pwd`/node/bin
EOF
$ source scripts/activate
```

```ShellSession
$ npm install -g gistup
$ ls node/bin
```

```ShellSession
$ cat > ~/.gistup.json <<EOF
{
  "token": "${GIST_TOKEN}"
}
EOF
```

## Report

```ShellSession
$ export LAB_NUMBER=02
$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
$ mkdir reports/lab${LAB_NUMBER}
$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
$ cd reports/lab${LAB_NUMBER}
$ edit REPORT.md
$ gistup -m "lab${LAB_NUMBER}"
```

## Links

### Unix commands

- [ar](https://en.wikipedia.org/wiki/Ar_(Unix)) - архиватор
- [cat](https://en.wikipedia.org/wiki/Cat_(Unix)) - считывает файлы и записывает их в стандартный вывод
- [cd](https://en.wikipedia.org/wiki/Cd_(command)) - перейти в директорию, в которой находились до перехода в текущую директорию
- [cp](https://en.wikipedia.org/wiki/Cp_(Unix)) - скопировать файл
- [cut](https://en.wikipedia.org/wiki/Cut_(Unix)) - выбрать из каждой строки файла нужную часть
- [echo](https://en.wikipedia.org/wiki/Echo_(command)) -  вывести строку текста в терминал
- [env](https://en.wikipedia.org/wiki/Env_(shell)) - печать списка переменных среды или запуска другой утилиты в измененной среде без необходимости изменять существующую среду
- [ex](https://en.wikipedia.org/wiki/Ex_(editor)) - онлайн-редактор
- [file](https://en.wikipedia.org/wiki/File_(command)) - распознавание типа данных, содержащихся в файле компьютера
- [find](https://en.wikipedia.org/wiki/Find) -  найти файлы и директории
- [ls](https://en.wikipedia.org/wiki/Ls) - отобразить содержимое текущей директории
- [man](https://en.wikipedia.org/wiki/Man_page) - форматирование и выводcdd справочных страниц
- [mkdir](https://en.wikipedia.org/wiki/Mkdir) - создать новый каталог
- [mv](https://en.wikipedia.org/wiki/Mv) - перемещение одного или нескольких файлов или каталогов из одного места в другое
- [nm](https://en.wikipedia.org/wiki/Nm_(Unix)) - используется для проверки файлов и для отображения содержимого этих файлов или метаинформации, хранящейся в них
- [ps](https://en.wikipedia.org/wiki/Ps_(Unix)) - выводит текущие активные процессы
- [pwd](https://en.wikipedia.org/wiki/Pwd) - печать списка переменных среды или запуска другой утилиты в измененной среде без необходимости изменять существующую среду
- [rm](https://en.wikipedia.org/wiki/Rm_(Unix)) - удаление объектов
- [sed](https://en.wikipedia.org/wiki/Sed) - преобразовывает текст
- [touch](https://en.wikipedia.org/wiki/Touch_(Unix)) - обновить дату доступа и дату изменения файла или каталога

### Package Managers

- [apt](http://help.ubuntu.ru/wiki/apt) | [dnf](https://en.wikipedia.org/wiki/DNF_(software)) | [yum](https://fedoraproject.org/wiki/Yum/ru) - позволяют управлять программными пакетами
- [brew](https://brew.sh) | [linuxbrew](http://linuxbrew.sh) - устанавливают нужные пользователю пакеты (brew-mcOS;linuxsrew-Linux)
- [npm](https://docs.npmjs.com) - пакетный менеджер для javascript

### Software

- [curl](https://www.gitbook.com/book/bagder/everything-curl/details) - позволяет взаимодействовать с множеством различных серверов по множеству различных протоколов с синтаксисом URL.
- [wget](https://www.gnu.org/software/wget/manual/wget.pdf) - консольная программа для загрузки файлов по сети.
- [clang](https://clang.llvm.org) - фронтенд для языков программирования C, C++ 
- [g++](https://gcc.gnu.org/onlinedocs/gcc-4.0.2/gcc/G_002b_002b-and-GCC.html) - компилятор
- [make](https://en.wikipedia.org/wiki/Make_(software)) - создает исполняемые программы и библиотеки из исходного кода
- [open](https://developer.apple.com/legacy/library/documentation/Darwin/Reference/ManPages/man1/open.1.html) - открывает файл
- [openssl](https://www.openssl.org) - криптографический пакет 
- [nano](https://www.nano-editor.org) - консольный текстовый редактор 
- [tree](https://linux.die.net/man/1/tree) - рекурсивный каталог 
- [vim](http://www.vim.org) - текстовый редактор
