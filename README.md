<div align="center">

<img src="assets/icon.png" alt="Blockfield Logo" width="128" height="128" />

# BLOCKFIELD DISTRIBUTIONS
### Официальные дистрибутивы игрового клиента и сервера Blockfield

*«Высадка. Захват. Доминация.»*

[![Latest Release](https://img.shields.io/github/v/release/netherg-io/blockfield-releases?label=Релиз&style=for-the-badge&color=2ea44f)](https://github.com/netherg-io/blockfield-releases/releases)
[![Minecraft](https://img.shields.io/badge/Minecraft-1.21.1%20Fabric-orange?style=for-the-badge)](https://fabricmc.net/)
[![Java](https://img.shields.io/badge/Java-21%20%2F%20Temurin-red?style=for-the-badge)](https://adoptium.net/)
[![Launcher](https://img.shields.io/badge/Официальный%20Лаунчер-Windows%20%7C%20Linux-blue?style=for-the-badge)](https://github.com/netherg-io/blockfield-launcher-releases)
[![Docker](https://img.shields.io/badge/Docker-GHCR-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://github.com/orgs/netherg-io/packages?repo_name=blockfield-releases)

<br />

[**📥 Скачать сборки**](#-дистрибутивы-и-загрузка) • [**О проекте**](#-о-проекте-blockfield) • [**Клиент**](#-установка-клиента) • [**Сервер**](#-развертывание-сервера) • [**Docker**](#-docker-контейнеры) • [**Целостность**](#-проверка-целостности-sha-256) • [**Поддержка**](#-поддержка)

</div>

---

## 🚀 Дистрибутивы и загрузка

В данном репозитории публикуются полные официальные дистрибутивы проекта **Blockfield**, собранные и верифицированные в рамках единого автоматизированного CI/CD пайплайна GitHub Actions.

> [!IMPORTANT]
> **Для большинства игроков рекомендуется использовать [Blockfield Launcher](https://github.com/netherg-io/blockfield-launcher-releases).**  
> Он работает автономно («из коробки»), автоматически настраивает среду Java, проверяет целостность модов и моментально обновляет клиент в 1 клик.
> Пакеты ниже предназначены для пользователей сторонних лаунчеров (Prism, Modrinth, MultiMC), ручной установки, а также для администраторов и разработчиков серверов.

### 🎮 Клиентские сборки (Для игроков)

| Формат / Пакет | Файл | Назначение | Ссылка на загрузку |
| :--- | :--- | :--- | :--- |
| **Официальный лаунчер** | `.exe` / `.AppImage` / `.deb` / `.rpm` | Рекомендуемый автономный лаунчер со встроенным Java runtime и автообновлениями | [**Скачать лаунчер**](https://github.com/netherg-io/blockfield-launcher-releases/releases/latest) |
| **Prism Launcher / MultiMC** | `Blockfield-prism.zip` | Готовый импортируемый инстанс с автообновлением через Packwiz Bootstrap и автоподключением | [**Скачать ZIP**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield-prism.zip) |
| **Modrinth Modpack** | `Blockfield.mrpack` | Стандартный пакет Modrinth для Modrinth App, Prism Launcher, ATLauncher | [**Скачать mrpack**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield.mrpack) |
| **Полный архив клиента** | `Blockfield-client.zip` | Полный архив модов, конфигов и параметров для ручной распаковки в `.minecraft` | [**Скачать ZIP**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield-client.zip) |

---

### 🛠️ Серверные дистрибутивы (Для хостинга и администраторов)

| Компонент | Тип / Тег | Описание | Ссылка / Команда |
| :--- | :--- | :--- | :--- |
| **Standalone Server** | `Blockfield-server.zip` | Готовый выделенный сервер Fabric 1.21.1 со скриптами запуска (`start.sh` / `start.bat`) | [**Скачать ZIP**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield-server.zip) |
| **Шаблоны миров** | `world-seed.zip` | Базовые шаблоны хаба, лобби и карт секторов (world-seed-v1) | [**Скачать ZIP**](https://github.com/netherg-io/blockfield-releases/releases/download/world-seed-v1/world-seed.zip) |
| **Docker: Сервер** | `ghcr.io/netherg-io/blockfield-server:latest` | Готовый оптимизированный контейнер выделенного игрового сервера | `docker pull ghcr.io/netherg-io/blockfield-server:latest` |
| **Docker: Веб-зеркало** | `ghcr.io/netherg-io/blockfield-web:latest` | Образ веб-портала и локального зеркала синхронизации файлов packwiz | `docker pull ghcr.io/netherg-io/blockfield-web:latest` |
| **Манифест и хеши** | `build.json` / `SHA256SUMS` | Полный инвентарь сборки, коммиты исходников и контрольные суммы | [**Страница Releases**](https://github.com/netherg-io/blockfield-releases/releases) |

> [!TIP]
> Все версии архивов и контрольные суммы (`SHA256SUMS`) доступны на странице [**Releases**](https://github.com/netherg-io/blockfield-releases/releases).

---

## 🎯 О проекте Blockfield

**Blockfield** — это масштабный командный тактический PvP-проект на базе платформы **Minecraft (1.21.1 Fabric)**:

- 🚩 **Контроль секторов**: динамический захват и тактическое удержание стратегических рубежей.
- 🎖️ **6 специализированных классов**: штурмовик, снайпер, медик, инженер, поддержка и разведчик — каждый со своим уникальным комплектом снаряжения и механиками.
- 🚜 **Военная техника**: наземная бронетехника и транспорт для быстрой переброски пехоты и огневого подавления.
- ⚡ **Операция «Железный фронт»**: проработанный театр военных действий, динамические контратаки и слаженное командное взаимодействие.
- 🌐 **Публичный игровой сервер**: `minecraft.play.nether.pp.ua:25565`

---

## 📦 Установка клиента

<details open>
<summary><b>1. Prism Launcher / MultiMC (Рекомендуемый альтернативный способ)</b></summary>

Сборка `Blockfield-prism.zip` сконфигурирована с предстартовым скриптом **Packwiz Bootstrap**. При каждом запуске инстанс автоматически проверяет актуальность модов на сервере обновлений и выполняет прямое подключение к игровому серверу.

1. Установите [Prism Launcher](https://prismlauncher.org/) (или MultiMC).
2. Скачайте архив [**Blockfield-prism.zip**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield-prism.zip).
3. В лаунчере нажмите **«Добавить сборку»** (*Add Instance*) → **«Импорт»** (*Import*) → выберите скачанный `.zip`.
4. Убедитесь, что в настройках инстанса выбрана **Java 21** и выделено минимум **4 ГБ ОЗУ**.
5. Запустите инстанс — загрузчик синхронизирует моды и сразу подключится к серверу!

</details>

<details>
<summary><b>2. Modrinth App / лаунчеры с поддержкой .mrpack</b></summary>

1. Скачайте файл [**Blockfield.mrpack**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield.mrpack).
2. В Modrinth App перейдите во вкладку инстансов и нажмите кнопку **«Import from file»** / перетащите `.mrpack` в окно приложения.
3. Дождитесь загрузки всех зависимостей и модов.
4. Адрес сервера для подключения: `minecraft.play.nether.pp.ua:25565`.

</details>

<details>
<summary><b>3. Ручная установка (Стандартный .minecraft)</b></summary>

1. Установите чистый клиент **Minecraft 1.21.1**.
2. Установите [Fabric Loader 1.21.1](https://fabricmc.net/use/installer/) (рекомендуется версия загрузчика 0.16.x+).
3. Скачайте архив [**Blockfield-client.zip**](https://github.com/netherg-io/blockfield-releases/releases/latest/download/Blockfield-client.zip).
4. Распакуйте содержимое архива в директорию вашей игры (`.minecraft` в `%appdata%` на Windows или `~/.minecraft` на Linux).
5. Запустите профиль Fabric 1.21.1. В меню сетевой игры подключитесь к адресу: `minecraft.play.nether.pp.ua:25565`.

</details>

---

## 🖥️ Развертывание сервера

### Автономный сервер (Standalone Archive)

Для запуска выделенного сервера требуется установленная **Java 21 LTS** (рекомендуется Eclipse Temurin).

#### Запуск на Linux / macOS
```bash
# 1. Создайте директорию сервера и распакуйте архив
mkdir -p /srv/blockfield && cd /srv/blockfield
unzip /path/to/Blockfield-server.zip

# 2. Примите лицензионное соглашение Minecraft EULA
echo "eula=true" > eula.txt

# 3. Сделайте скрипт запуска исполняемым и запустите сервер
chmod +x start.sh
./start.sh
```

#### Запуск на Windows
```cmd
:: 1. Распакуйте Blockfield-server.zip в любую постоянную папку
:: 2. Создайте файл eula.txt со строкой eula=true
:: 3. Запустите start.bat
```

> [!NOTE]
> - По умолчанию сервер запускается с выделением до 6 ГБ ОЗУ (`-Xms512M -Xmx6G`). Вы можете изменить параметры памяти в файле `start.sh` или `start.bat`.
> - Сервер слушает стандартный порт **25565** (TCP и UDP). Убедитесь, что порт открыт в брандмауэре.
> - При первом запуске автоматически подгружаются недостающие библиотеки Fabric Loader.

---

## 🐳 Docker контейнеры

Официальные образы публикуются в реестре **GitHub Container Registry (GHCR)**:

```bash
# Игровой выделенный сервер Blockfield
docker pull ghcr.io/netherg-io/blockfield-server:latest

# Веб-сервер / зеркало раздачи packwiz
docker pull ghcr.io/netherg-io/blockfield-web:latest
```

### Пример `docker-compose.yml`

```yaml
services:
  blockfield-server:
    image: ghcr.io/netherg-io/blockfield-server:latest
    container_name: blockfield-server
    restart: unless-stopped
    ports:
      - "25565:25565/tcp"
      - "25565:25565/udp"
    volumes:
      - ./server-data:/data
    environment:
      - MEMORY=6G
      - EULA=true
```

Запуск:
```bash
docker compose up -d
```

---

## 🔒 Проверка целостности (SHA-256)

Каждый релиз снабжен файлом `SHA256SUMS` со всеми криптографическими контрольными суммами дистрибутивов.

Для проверки скачанных архивов выполните команду в терминале:

```bash
# Linux / macOS
sha256sum -c SHA256SUMS --ignore-missing

# Windows (PowerShell)
Get-FileHash Blockfield-client.zip -Algorithm SHA256
```

Файл `build.json` содержит детальный инвентарь сборки, включая точные хэши каждого мода и SHA-коммиты исходных репозиториев:
- Репозиторий мода: `netherg-io/blockfield-mod`
- Серверная конфигурация: `netherguy4/minecraft-server`
- Модпак и дистрибуция: `netherg-io/blockfield-modpack`

---

## 💻 Системные требования

| Параметр | Клиент (Минимальные) | Клиент (Рекомендуемые) | Выделенный сервер |
| :--- | :--- | :--- | :--- |
| **ОС** | Windows 10/11 x64, Linux, macOS | Windows 10/11 x64, современный Linux | Linux x64 (Ubuntu / Debian / RHEL) |
| **Java Runtime** | Java 21 (Temurin 21) | Java 21 (Temurin 21) | Java 21 LTS 64-bit |
| **Процессор** | 2 ядра / 4 потока (Intel / AMD) | 4+ ядра (i5 / Ryzen 5+) | 4+ ядра с высокой однопоточной частотой |
| **ОЗУ** | 4 ГБ (выделено в игре: 3 ГБ) | 8+ ГБ (выделено в игре: 4–6 ГБ) | 6–8 ГБ оперативной памяти |
| **Видеокарта** | OpenGL 4.4 / Vulkan совместимая | Дискретная NVIDIA / AMD / Arc | Не требуется (headless) |
| **Сеть** | Широкополосный доступ | Стабильное соединение с низким пингом | 100 Мбит/с+ с белым IP-адресом |

---

## ❓ Часто задаваемые вопросы

<details>
<summary><b>Какая версия Java требуется для работы?</b></summary>
Для клиента и сервера Blockfield требуется <b>Java 21</b>. Мы рекомендуем использовать сборку <a href="https://adoptium.net/">Eclipse Temurin 21 (LTS)</a>. Если вы используете официальный <a href="https://github.com/netherg-io/blockfield-launcher-releases">Blockfield Launcher</a>, Java загружается и настраивается автоматически.
</details>

<details>
<summary><b>Какой IP-адрес используется для подключения к игре?</b></summary>
Основной публичный сервер проекта: <code>minecraft.play.nether.pp.ua:25565</code>. В инстансе Prism Launcher и официальном лаунчере адрес сервера уже преднастроен.
</details>

<details>
<summary><b>Как правильно обновить standalone-сервер на новую версию?</b></summary>
Ни в коем случае не распаковывайте новый архив поверх запущенного сервера! Остановите сервер, сделайте резервную копию папок <code>world</code> и <code>playerdata</code>, после чего замените папку <code>mods/</code> и обновленные файлы конфигураций из нового релиза.
</details>

<details>
<summary><b>Где взять чистые шаблоны карт и хаба?</b></summary>
Готовые шаблоны секторов и спавна без данных игроков доступны в релизе <a href="https://github.com/netherg-io/blockfield-releases/releases/tag/world-seed-v1">world-seed-v1</a> (архив <code>world-seed.zip</code>).
</details>

<details>
<summary><b>Куда сообщать о багах и ошибках сборки?</b></summary>
Обо всех обнаруженных неисправностях в модах или дистрибутивах создавайте обращение во вкладке <a href="https://github.com/netherg-io/blockfield-releases/issues">Issues</a> с приложением логов (<code>latest.log</code>, <code>crash-reports</code>) и хеша сборки из <code>build.json</code>.
</details>

---

<div align="center">

**[Blockfield Project](https://github.com/netherg-io)** • 2026

</div>
