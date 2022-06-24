<h1 align="center">NOTFLIX на русском</h1>
<p align="center">стриминг торрентов прямо из коммандной строки на Linux и macOS</p>

### Как это работает

Это шелл скрипт. Он парсит rutor и получает магнет ссылку.
После использует [peerflix](https://github.com/mafintosh/peerflix) для стримитнга видео по этой ссылке.

Для использования достаточно набрать ```notflixru <название фильма>```, будет предложен выбор файла/серии, а после воспроизведение запустится автоматически. По умолчанию выбран проигрыватель VLC, вы можете поменять в коде на другой. Также нужно учитывать, что rutor доступен без VPN далеко не везде. Есть также второй источник nyaa.si, можно переключить при необходимости.

## Зависимости

* [peerflix](https://github.com/mafintosh/peerflix) - Программа для стриминга торрентов `sudo npm install peerflix -g`
* [WARP](https://1.1.1.1/) - позволяет получать доступ к заблокированным страницам, инструкция по его установке тут: https://developers.cloudflare.com/warp-client/get-started/
## Установка

### cURL
cURL **notflixru** в ваш **$PATH** и выдайте разрешения для запуска.

```sh
sudo curl -sL "https://raw.githubusercontent.com/rouol/notflixru/master/notflixru" -o /usr/local/bin/notflixru
sudo chmod +x /usr/local/bin/notflixru
```
- Для обновления, просто сделайте `curl` снова, в повторном `chmod` нет необходимости.
- Для удаления программы, просто удалите `notflix` из вашего **$PATH**, например `sudo rm -f /usr/local/bin/notflixru`.

*Для пользователей macOS: необходимо установить полноценный grep, например с помощью homebrew так: ```brew install grep```. После установки нужно также добавить новый grep в ваш **$PATH**, выполнив команду

```echo 'export PATH="/usr/local/opt/grep/libexec/gnubin:$PATH"' >> ~/.bashrc``` или ```~/.zshrc``` в зависимости от вашей среды.

* Спасибо [Bugswriter](https://github.com/Bugswriter) за реализацию для английской аудитории, эта программа построена оригинальном [notflix](https://github.com/Bugswriter/notflix).
* Thanks to [Bugswriter](https://github.com/Bugswriter) for implementing for English audiences, this program is built by the original [notflix](https://github.com/Bugswriter/notflix).

## License
...
