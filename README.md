# My Hyprland Dotfiles 🖥️

Мои конфигурационные файлы для Hyprland и окружения. Тут всё что нужно для комфортной работы: тайловый WM, красивый бар, быстрый терминал и удобный лаунчер.



<img width="2560" height="1080" alt="2026-03-16-175116" src="https://github.com/user-attachments/assets/f9e32289-a2d9-40de-b877-861d32d97e51" />

<img width="2560" height="1080" alt="2026-03-16-175236" src="https://github.com/user-attachments/assets/f87b13e3-a137-4c59-963b-04ec88064539" />

# config_hyprland<img width="2560" height="1080" alt="2026-03-11-181743" src="https://github.com/user-attachments/assets/f55f6e71-e62a-4263-a14a-319bba6b0f2f" />


ОБОИ ЕСТЬ У МЕНЯ В ДРУГОМ РЕПОЗИТОРИИ
<img width="1920" height="1080" alt="07  Gruvbox Retro" src="https://github.com/user-attachments/assets/3e46e544-5e44-45cf-9c7b-4b022e941b92" />

![170737-apelsin-yabloko-apple_watch-ios-kompyuter_imac-3840x2160](https://github.com/user-attachments/assets/f5792468-7620-4f7b-8919-1bb26345d3df)

![176221-apelsin-dizajn-dnevnoe_vremya-priroda-lazurnyj-3840x2160](https://github.com/user-attachments/assets/4be88801-1507-44f7-a563-e36f205f46eb)

![Airbrush-image-enhancer-1773599216901](https://github.com/user-attachments/assets/4afb8ea7-427e-4bd2-8525-f1b93f532014)


## 🔥 Горячие клавиши

### Основные
- `Super + Q` — закрыть окно (Alacritty) [citation:1]
- `Super + R` — открыть Rofi (запуск программ)
- `Super + W` — поменять обои (указываете путь сами)
- `Super + L` — заблокировать экран

### Окна и рабочие столы
- `Super + 1-9` — переключиться по рабочим сталам
- `Super + Shift + 1-9` — переместить окно на рабочиый стол
- `Super + Left/Right` — навигация по окнам
- `Super + F` — сделать окно на весь экран

### Внешний вид
- `Super + Shift + S` — скриншот области (через grim+slurp)

## 🎨 Waybar

Панель показывает:
- Рабочие пространства (с подсветкой активного) 
- Текущее окно
- Загрузку RAM
- Громкость (pulseaudio)
- Часы 
- Bluetooth
- язык
- тип подключения к сети

Кастомизация в `waybar/style.css` (цвета, отступы, шрифты).

## 🖥️ Alacritty

Быстрый терминал без лишних наворотов (нет вкладок — они в tmux) [citation:3][citation:10]. Настройки:
- Шрифт: Hack Nerd Font (или JetBrains Mono)
- Прозрачность (если включена)
- Цветовая схема (подобрана под общую тему)
- Размер окна и отступы [citation:7]

## 🔍 Rofi

Использую как:
- Лаунчер программ (`rofi -show drun`)
- Переключатель окон (`rofi -show window`)
- Выполнение команд (`rofi -show run`)

В конфиге настроены тема, прозрачность и иконки [citation:8]. Wayland работает через XWayland или нативный бэкенд [citation:4].

## 🛠 Установка

```bash
# Клонируем репозиторий
git clone <ссылка на твой репозиторий> ~/dotfiles

# Копируем конфиги (или создаем симлинки)
ln -s ~/dotfiles/hypr ~/.config/hypr
ln -s ~/dotfiles/waybar ~/.config/waybar
ln -s ~/dotfiles/alacritty ~/.config/alacritty
ln -s ~/dotfiles/rofi ~/.config/rofi

# Убедись что шрифты стоят (Hack Nerd Font обязательно!)
