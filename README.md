VLCAutoPlay

--------------------------------------------------------------------------
📌 Назначение
--------------------------------------------------------------------------
VLCAutoPlay — это графическая утилита для автоматического воспроизведения
плейлистов в VLC Media Player.  
Программа отслеживает выбранную папку с медиаконтентом (фото/видео/аудио) и
автоматически обновляет плейлист VLC при добавлении или удалении файлов.

Поддерживаются файлы:
VIDEO_EXT = [".mp4", ".avi", ".mkv", ".mov", ".mp3", ".wav", ".flac"]
PHOTO_EXT = [".jpg", ".jpeg", ".png", ".bmp", ".gif"]
 
--------------------------------------------------------------------------
⚙️ Основные возможности
--------------------------------------------------------------------------
- Возможность задать период воспроизведения слайда фото(значения сохраняются в config.json).
- Возможность задать время автозапуска(значения сохраняются в config.json).
- Автоматический запуск VLC с web-интерфейсом.
- Автоматическое наполнение плейлиста содержимым выбранной папки.
- Отслеживание изменений:
  * новые файлы → добавляются в конец плейлиста;
  * удалённые файлы → исключаются из плейлиста без ошибок;
  * если удалён текущий файл → VLC переключается на следующий.
- Кнопки управления: Старт, Стоп, Следующий, Предыдущий, Обновить плейлист.
- Кнопка открытия встроенной веб-панели VLC в браузере.
- Автоматическое воспроизведение после старта Windows
  (опция через установщик).

--------------------------------------------------------------------------
🚀 Логика работы
--------------------------------------------------------------------------
1. При первом запуске программа предложит задать:
   - пароль для web-интерфейса VLC (по умолчанию `1111`);
   - порт для web-интерфейса (по умолчанию `8080`).

   Эти параметры сохраняются в конфиге.

2. Пользователь выбирает:
   - папку с медиаконтентом;
   - путь к VLC (обычно `C:\Program Files\VideoLAN\VLC\vlc.exe`).
   - задает время показа слайдов;
   - задает время автостарта;

3. При нажатии **Старт**:
   - запускается VLC с web-интерфейсом;
   - очищается плейлист;
   - в него добавляются все файлы из выбранной папки;
   - запускается воспроизведение.

4. Если в папке происходят изменения:
   - добавленные файлы → автоматически в конец;
   - удалённые файлы → удаляются из VLC;
   - если удалён текущий файл → включается следующий.

5. При перезапуске ПК можно включить **автозапуск программы** через установщик.  
   Тогда она запустится, по времени автостарта GUI свернется и VLC начнет воспроизведение.

--------------------------------------------------------------------------
📂 Конфигурация
--------------------------------------------------------------------------
Конфиг хранится в:

    %APPDATA%\VLCAutoPlay\config.json

В нём сохраняются:
- путь к папке с контентом;
- путь к VLC;
- порт web-интерфейса;
- пароль web-интерфейса (в зашифрованном виде);
- время показа слайда фото;
- время автостарта.

--------------------------------------------------------------------------
License This project is licensed under the GNU General Public License v3.0 - 
see the LICENSE file for details.





Automatic VLC playback

--------------------------------------------------------------------------
📌 Appointment
--------------------------------------------------------------------------
VLC AutoPlay is a graphical utility for automatically playing
a playlist in a VLC media player.  
The program monitors the selected folder with media content (photo/video/audio) and
automated management systems include VLC for adding or deleting files.

Files are supported:
VIDEO_EXT = [".mp4", ".avi", ".mkv", ".mov", ".mp3", ".wav", ".flac"]
PHOTO_EXT = [".jpg", ".jpeg", ".png", ".bmp", ".gif"]

--------------------------------------------------------------------------
⚙️ Main features
--------------------------------------------------------------------------
- The ability to access all of this (the value is stored in the config.json file).
- The ability to find the necessary information (the value is stored in the config.json file).
- Automatic access to VLC with a web interface.
- Automatic filling of the playlist with the contents of the selected folder.
- Change tracking:
* New files → added to the end of the playlist;
  * deleted files → are excluded from the playlist without errors;
  * Elena udaltsovskaya → VLC switches to the next one.
- Control buttons: Start, Stop, Next, Previous, Refresh Playlist.
- The button to open the external VLC web panel in the browser.
- Automatic playback after Windows installation
  (option via the installer).

--------------------------------------------------------------------------
, The logic of the work
--------------------------------------------------------------------------
1. At the first launch, the program will prompt you to set:
   - for VLC web interface (default is `1111`);
   - for the web interface (default is `8080`).

   These parameters are saved in the config.

2. The user selects:
- a folder with media content;
   - the path to VLC (usually `C:\Program Files\VideoLAN\VLC\vlc.exe `).
   - sets the slide show time;
   - sets the auto-start time;

3. When you press **Start**:
- VLC is loaded with a web interface;
   - the playlist is being cleared;
   - all files from the selected folder are added to it.;
   - Playback starts.

4. If changes occur in the folder:
- added files → automatically at the end;
   - deleted files → delete from VLC;
   - if the current file is deleted, → the next one is included.

5. When restarting the PC, you can enable **program autorun** through the installer.  
   Then it will start, change the user interface and start playback.

--------------------------------------------------------------------------
📂 Configuration
--------------------------------------------------------------------------
The configuration is stored in:

    %APPDATA%\VLCAutoPlay\config.json

It stores:
- the path to the content folder;
- the path to VLC;
- via the web interface;
- the user of the web interface (in a hidden form);
- the time of the photo slide show;
- auto-start time.

--------------------------------------------------------------------------
License This project is licensed under the GNU General Public License version 3.0 -
see the LICENSE file for details.
