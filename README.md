[English](#english) · [Українська](#ukrainian)

<a id="english"></a>

# Lumo Router

**Spend less time choosing AI settings. Stay in your coding workflow.**

Lumo is a local Mac app that helps choose a model and reasoning effort for coding tasks in Codex and Claude Code. Keep using your existing coding tool; Lumo handles routing between it and your configured provider.
<img width="2172" height="724" alt="image" src="https://github.com/user-attachments/assets/356f6814-61b3-4cf6-a46c-c19280dbf994" />


## Why use Lumo?

Not every task needs the same amount of AI effort. Renaming a variable, investigating a failing test, and planning a cross-file refactor are different jobs. Always choosing the strongest settings can be unnecessary; always choosing the lightest settings may not fit a difficult task.

Lumo helps you balance that trade-off without making a new settings decision every time:

- **Less manual model selection.** Automatic routing chooses among eligible profiles for your configured provider, account, and settings.
- **Reasoning matched to the work.** A profile combines a model with a reasoning-effort level—how much thinking it is asked to do.
- **Visibility instead of guesswork.** Inspect the chosen model, effort, routing reason, request usage, latency, and estimated API cost in the local panel.
- **Control when you need it.** Make an explicit model choice or disable automatic selection when you want predictable settings.
- **A reversible setup.** Client settings are backed up during connection; Disconnect and the included recovery app help you return to standard configuration.

**The goal is a better balance of quality, waiting time, and usage—not guaranteed savings or better answers.** Routing adds classifier work and may add latency or cost. Measure the results on your own tasks.

## When it helps

| Your situation | How Lumo can help |
| --- | --- |
| You alternate between small edits and demanding debugging | Avoid treating every new task as if it needs identical model settings. |
| You are unsure which model and reasoning level to pick | Start with automatic routing rather than comparing options for every task. |
| You want to understand what your coding assistant actually uses | Review routing decisions and request metrics in one panel. |
| You want to experiment, but keep an escape hatch | Switch to explicit selection or disconnect and restore standard client settings. |

**It may not be for you yet** if you require a fully notarized installer, guaranteed live-account compatibility, an offline model, or exactly one fixed model for every task. This is an experimental build.

## How it works

**Your coding tool → Lumo on your Mac → your configured AI provider → back to your tool.**

For eligible new sessions, Lumo evaluates the available profiles and selects one within your configured restrictions. Existing sessions keep their model; reasoning can adapt on new user turns where the model supports it. It does not arbitrarily switch providers or models in the middle of a running tool sequence.

**Local routing does not mean offline AI.** Model requests go to your selected provider. When automatic classification is used, task context is also sent to the configured classifier. Use only accounts and code you are authorized to use with those providers.

## Languages

This download guide is available in **English and Ukrainian** using the links at the top. These are documentation languages; this does not promise a bilingual app interface or specific model-language capabilities.

## [⬇ Download for Mac — Apple Silicon](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.dmg)

**Mac with an M1 / M2 / M3 / M4 or newer Apple Silicon chip · macOS 14+**

Installers for Intel Macs, Windows, and Linux are not available here yet.
To check your Mac, open the Apple menu → **About This Mac** → **Chip**.

## Install in 3 steps

1. **Download and open the DMG.** Drag **Lumo Router.app** into **Applications**.
2. **Open Lumo Router from Applications.** Its icon appears in the menu bar near the clock; there may be no separate Dock window.
3. **Connect your own account or API key**, then connect Codex / Claude through the Lumo panel. Connecting backs up and changes the selected client's settings; follow the prompts and restart the client if requested.

**No Git, Node.js, Terminal, repository cloning, or Lumo website signup required.**
Codex / Claude must be installed separately. API access requires your own key and is billed separately from subscriptions.

### Important: before your first launch

This is an **experimental test build**, signed ad hoc, **without an Apple Developer ID signature or Apple notarization**.
macOS may block the first launch. Only if you trust this source and have verified the file:
after attempting to launch it, open **System Settings → Privacy & Security**;
if **Open Anyway** is offered, use it to confirm the launch.
Do not disable Gatekeeper, antivirus software, or system protection.
If macOS reports malware or offers no Open Anyway button, stop and report the issue.

ChatGPT-plan mode is experimental: availability and compatibility depend on your account and client.
Tests using local API mocks do not guarantee compatibility with a live account.

### Updates and disconnecting

- To update, download the new DMG, choose **Quit** in Lumo, replace the app in Applications, and open it again. Automatic updates are not available yet.
- Your settings stay on your Mac in `~/.lumo-router`; this repository does not contain them.
- Use **Disconnect** in Lumo to restore the client's standard configuration.
- For emergency Codex recovery, copy **both apps** from the DMG into the same Applications folder, then launch **Restore Standard Codex.app**. The recovery app asks for confirmation and does not automatically overwrite conflicting settings.

### Other downloads

- [ZIP instead of DMG](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.zip)
- [All versions and release notes](https://github.com/volyapers17/lumo-router-downloads/releases)
- [SHA-256 checksums for the latest version](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/SHA256SUMS.txt)
- [Report an issue](https://github.com/volyapers17/lumo-router-downloads/issues/new)

Checksums help verify file integrity; they are not a substitute for an Apple signature.
Optional Terminal command for comparison: `shasum -a 256 ~/Downloads/Lumo-Router-macOS-arm64.dmg`.

This public repository contains only instructions and installers. Source code,
personal keys, OAuth tokens, local settings, and request history are not published here.

---

[English ↑](#english) · [Українська](#ukrainian)

<a id="ukrainian"></a>

# Lumo Router

**Менше часу на вибір налаштувань ШІ. Більше уваги роботі над кодом.**

Lumo — локальний застосунок для Mac, який допомагає обирати модель та рівень міркування для завдань у Codex і Claude Code. Ви працюєте у звичному інструменті, а Lumo маршрутизує запити між ним і налаштованим провайдером.

## Навіщо використовувати Lumo?

Не кожне завдання потребує однакових зусиль від ШІ. Перейменування змінної, пошук причини невдалого тесту й планування рефакторингу кількох файлів — різні задачі. Найпотужніші налаштування можуть бути зайвими для простих змін, а найлегші — недостатніми для складної роботи.

Lumo допомагає знаходити баланс без постійного ручного вибору:

- **Менше ручного перемикання моделей.** Автоматична маршрутизація обирає серед допустимих профілів для вашого провайдера, облікового запису й налаштувань.
- **Рівень міркування під завдання.** Профіль поєднує модель і reasoning effort — рівень зусиль, який модель має витратити на обмірковування.
- **Прозорість замість здогадок.** Локальна панель показує обрану модель, рівень міркування, причину вибору, використання токенів, затримку й орієнтовну вартість API.
- **Контроль за потреби.** Явно оберіть модель або вимкніть автоматичний вибір, якщо потрібні передбачувані налаштування.
- **Можливість повернутися назад.** Під час підключення створюється резервна копія налаштувань клієнта; Disconnect та окремий застосунок відновлення допомагають повернути стандартну конфігурацію.

**Мета — збалансувати якість, час очікування та використання ресурсів, а не гарантувати економію чи кращі відповіді.** Класифікація створює додаткову роботу й може збільшувати затримку або вартість. Перевіряйте результат на власних завданнях.

## Коли це корисно

| Ваша ситуація | Чим допоможе Lumo |
| --- | --- |
| Ви чергуєте невеликі правки зі складним налагодженням | Нові завдання не обов'язково отримуватимуть однакові налаштування моделі. |
| Ви не знаєте, яку модель і рівень міркування обрати | Почніть з автоматичної маршрутизації замість порівняння опцій для кожного завдання. |
| Ви хочете розуміти, що саме використовує помічник | Переглядайте рішення маршрутизації й показники запитів в одній панелі. |
| Ви хочете експериментувати, але мати шлях назад | Оберіть модель вручну або від'єднайте клієнт і відновіть стандартні налаштування. |

**Поки що Lumo може вам не підійти**, якщо потрібні нотаризований Apple установник, гарантована сумісність із реальним обліковим записом, офлайн-модель або незмінна модель для всіх задач. Це експериментальна збірка.

## Як це працює

**Ваш інструмент для коду → Lumo на вашому Mac → налаштований провайдер ШІ → назад до інструмента.**

Для нових сесій, які підтримують маршрутизацію, Lumo оцінює доступні профілі й обирає один у межах налаштованих обмежень. Поточні сесії зберігають свою модель; рівень міркування може змінюватися з новими повідомленнями користувача, якщо модель це підтримує. Lumo не перемикає довільно провайдера чи модель посеред виконання послідовності інструментів.

**Локальна маршрутизація не означає офлайн-ШІ.** Запити надсилаються обраному провайдеру. За автоматичної класифікації контекст завдання також надсилається налаштованому класифікатору. Використовуйте лише ті облікові записи й код, які ви маєте право передавати цим провайдерам.

## Мови

Цей посібник із завантаження доступний **англійською та українською** — перемикайтеся посиланнями вгорі. Це мови документації, а не обіцянка двомовного інтерфейсу застосунку чи певних мовних можливостей моделі.

## [⬇ Завантажити для Mac — Apple Silicon](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.dmg)

**Mac із чипом M1 / M2 / M3 / M4 або новішим Apple Silicon · macOS 14+**

Готових установників для Intel Mac, Windows і Linux тут поки немає.
Перевірити свій Mac: меню Apple → **Про цей Mac / About This Mac** → **Чип / Chip**.

## Встановлення за 3 кроки

1. **Завантажте й відкрийте DMG.** Перетягніть **Lumo Router.app** у **Applications / Програми**.
2. **Відкрийте Lumo Router з Applications.** Значок з'явиться в рядку меню біля годинника; окремого вікна в Dock може не бути.
3. **Підключіть власний обліковий запис або API-ключ**, а потім Codex / Claude через панель Lumo. Підключення створює резервну копію й змінює налаштування обраного клієнта; дотримуйтеся підказок і за потреби перезапустіть клієнт.

**Не потрібні Git, Node.js, Terminal, клонування репозиторію чи реєстрація на сайті Lumo.**
Codex / Claude встановлюються окремо. Для API потрібен власний ключ; використання API оплачується окремо від підписок.

### Важливо перед першим запуском

Це **експериментальна тестова збірка** з підписом ad hoc, **без підпису Apple Developer ID та нотаризації Apple**.
macOS може заблокувати перший запуск. Лише якщо ви довіряєте джерелу та перевірили файл:
після спроби запуску відкрийте **Системні параметри → Приватність і безпека / System Settings → Privacy & Security**;
якщо доступна кнопка **Open Anyway**, підтвердьте запуск.
Не вимикайте Gatekeeper, антивірус чи системний захист.
Якщо macOS повідомляє про шкідливе ПЗ або кнопки Open Anyway немає, зупиніться й повідомте про проблему.

Режим ChatGPT-plan експериментальний: доступність і сумісність залежать від облікового запису та клієнта.
Тести з локальними імітаціями API не гарантують сумісності з реальним обліковим записом.

### Оновлення та від'єднання

- Для оновлення завантажте новий DMG, завершіть Lumo через **Quit**, замініть застосунок в Applications і відкрийте знову. Автоматичного оновлення поки немає.
- Налаштування залишаються на вашому Mac у `~/.lumo-router`; цей репозиторій їх не містить.
- Для повернення стандартної конфігурації клієнта використовуйте **Disconnect** у Lumo.
- Для аварійного відновлення Codex скопіюйте **обидва застосунки** з DMG в одну папку Applications і запустіть **Restore Standard Codex.app**. Застосунок відновлення запитує підтвердження й не перезаписує конфліктні налаштування автоматично.

### Інші завантаження

- [ZIP замість DMG](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/Lumo-Router-macOS-arm64.zip)
- [Усі версії та примітки до випусків](https://github.com/volyapers17/lumo-router-downloads/releases)
- [Контрольні суми SHA-256 актуальної версії](https://github.com/volyapers17/lumo-router-downloads/releases/latest/download/SHA256SUMS.txt)
- [Повідомити про проблему](https://github.com/volyapers17/lumo-router-downloads/issues/new)

Контрольні суми допомагають перевірити цілісність файлу, але не замінюють підпис Apple.
Необов'язкова команда Terminal для порівняння: `shasum -a 256 ~/Downloads/Lumo-Router-macOS-arm64.dmg`.

Цей публічний репозиторій містить лише інструкції та установники. Вихідний код,
особисті ключі, OAuth-токени, локальні налаштування та історія запитів тут не публікуються.
