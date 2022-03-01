<h1 align="center">NOTFLIX на русском</h1>
<p align="center">стриминг торрентов прямо из коммандной строки на Linux и macOS</p>

### Как это работает

Это шелл скрипт. Он парсит rutor и получает магнет ссылку.
После использует [peerflix](https://github.com/mafintosh/peerflix) для стримитнга видео по этой ссылке.

## Зависимости

* [peerflix](https://github.com/mafintosh/peerflix) - Программа для стриминга торрентов `sudo npm install peerflix -g`

## Установка

### cURL
cURL **notflixru** в ваш **$PATH** и выдайте разрешения для запуска.

```sh
$ sudo curl -sL "https://github.com/rouol/notflixru/blob/master/notflixru" -o /usr/local/bin/notflixru
$ sudo chmod +x /usr/local/bin/notflixru
```
- Для обновления, просто сделайте `curl` снова, в повторном `chmod` нет необходимости.
- Для удаления программы, просто удалите `notflix` из вашего **$PATH**, например `sudo rm -f /usr/local/bin/notflixru`.

*Для пользователей macOS: необходимо установить полноценный grep, например с помощью homebrew так: ```brew install grep```. После установки нужно также добавить новый grep в ваш **$PATH**, выполнив команду

```echo 'export PATH="/usr/local/opt/grep/libexec/gnubin:$PATH"' >> ~/.bashrc``` или ```~/.zshrc``` в зависимости от вашей среды.

* Спасибо [Bugswriter](https://github.com/Bugswriter) за реализацию для английской аудитории, эта программа построена оригинальном [notflix](https://github.com/Bugswriter/notflix).
* Thanks to [Bugswriter](https://github.com/Bugswriter) for implementing for English audiences, this program is built by the original [notflix](https://github.com/Bugswriter/notflix).

## License
...
