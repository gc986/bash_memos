# bash_memos
Мои заметки по командам BASH 

echo - Просто вывод сообщения. Нпример: <i>echo "hi all"</i>

Если хочется сменить цвет шрифта у выводимого текста, то нужно воспользоваться следущей конструкцией, например: <i>echo -en "\033[1;36m"</i>

Цвект можно задачать как тексту так и заднемо фону (https://techstop.github.io/bash-script-colors/):

# Regular Colors

| Value    | Color  |
| -------- | ------ |
| \e[0;30m | Black  |
| \e[0;31m | Red    |
| \e[0;32m | Green  |
| \e[0;33m | Yellow |
| \e[0;34m | Blue   |
| \e[0;35m | Purple |
| \e[0;36m | Cyan   |
| \e[0;37m | White  |

# Bold

| Value    | Color    |
| -------- | -------- |
| \e[1;30m | Black    |
| \e[1;31m | Red      |
| \e[1;32m | Green    |
| \e[1;33m | Yellow   |
| \e[1;34m | Blue     |
| \e[1;35m | Purple   |
| \e[1;36m | Cyan     |
| \e[1;37m | White    |
| \e[1m    | No Color |

# Underline

| Value    | Color    |
| -------- | -------- |
| \e[4;30m | Black    |
| \e[4;31m | Red      |
| \e[4;32m | Green    |
| \e[4;33m | Yellow   |
| \e[4;34m | Blue     |
| \e[4;35m | Purple   |
| \e[4;36m | Cyan     |
| \e[4;37m | White    |
| \e[4m    | No Color |

# Background

| Value  | Color  |
| ------ | ------ |
| \e[40m | Black  |
| \e[41m | Red    |
| \e[42m | Green  |
| \e[43m | Yellow |
| \e[44m | Blue   |
| \e[45m | Purple |
| \e[46m | Cyan   |
| \e[47m | White  |

# Expand Background Horizontally

| Value |   Color  |
| ----- | -------- |
| \e[K  | No Color |

# High Intensty

| Value    | Color  |
| -------- | ------ |
| \e[0;90m | Black  |
| \e[0;91m | Red    |
| \e[0;92m | Green  |
| \e[0;93m | Yellow |
| \e[0;94m | Blue   |
| \e[0;95m | Purple |
| \e[0;96m | Cyan   |
| \e[0;97m | White  |

# Bold High Intensty

| Value    | Color  |
| -------- | ------ |
| \e[1;90m | Black  |
| \e[1;91m | Red    |
| \e[1;92m | Green  |
| \e[1;93m | Yellow |
| \e[1;94m | Blue   |
| \e[1;95m | Purple |
| \e[1;96m | Cyan   |
| \e[1;97m | White  |

# High Intensty backgrounds

| Value     | Color  |
| --------- | ------ |
| \e[0;100m | Black  |
| \e[0;101m | Red    |
| \e[0;102m | Green  |
| \e[0;103m | Yellow |
| \e[0;104m | Blue   |
| \e[0;105m | Purple |
| \e[0;106m | Cyan   |
| \e[0;107m | White  |

# Reset

| Value | Color  |
| ----- | ------ |
| \e[0m | Reset  |

Если нужно выполнить несколько команд одну за одной и они должны быть не связаны между собой, то их нужно просто разделять знаком ; (точка с запятой). Например: <i>pwd;pwd</i>

Если нужно выполнить связанные команды одну за одно, то нужно воспользоваться командой &&. Например: <i>cd $dir && git checkout $target_branch</i>

Если нужно выполнить команду в фоне, просто в конце команды ставим знак &. Например: telegram&
