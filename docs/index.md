# AI-агенты и Harness-инженерия

## Каталог курсов на русском языке

Русские переводы курсов по инженерии AI-агентов, harness-дизайну и построению надёжных автономных систем. Все материалы переведены с сохранением кода, архитектурных паттернов и практических упражнений.

---

## Курсы

### 🏗️ Строим AI-кодинг агент: каркас (harness) с нуля

**Источник:** [Build Your Own AI Coding Agent Harness](https://vercel.com/academy/build-ai-agent-harness) — Vercel Academy, автор Joel Hooks

**О чём:** Полный курс по построению каркаса AI-кодинг-агента на TypeScript + AI SDK v6. От простого чатбота с одним инструментом до полноценного агента с субагентами, песочницами, управлением контекстом и расширяемостью. Каждый шаг существует потому, что предыдущий что-то сломал.

**Что изучите:**
- Агент-лупа: как превратить чатбота в агента одним инструментом
- Дизайн инструментов: 5-секционный контракт, паттерн «фабрика», approval gates
- Системный промпт: структурированные инструкции, динамическая композиция, AGENTS.md
- Абстракция песочницы: один интерфейс — local / in-memory / cloud
- Управление контекстом: pruning, bounded output, cache control
- Субагенты: Explorer (только чтение) и Executor (полные инструменты)
- Жизненный цикл: state machine, snapshot/restore, durable workflows
- Human-in-the-loop: askUser, протокол «ищи → спрашивай → действуй»
- Планирование: todo tool, grep-first, контракт верификации
- Поверхности: CLI, стриминг, веб — один агент, разные рендереры
- Расширяемость: event bus, skills, custom tools

**Объём:** 38 уроков, 11 модулей

**Стек:** TypeScript, AI SDK v6, Zod v3, just-bash, Vercel Sandbox/Workflow

🌐 **Сайт:** [galaersh-ai.github.io/ai-agent-harness-guide](https://galaersh-ai.github.io/ai-agent-harness-guide/)
📁 **Код:** [github.com/galaersh-ai/ai-agent-harness-guide](https://github.com/galaersh-ai/ai-agent-harness-guide)

---

### 📁 Строим файлового агента: анализ транскриптов через bash

**Источник:** [Building Filesystem Agents](https://vercel.com/academy/filesystem-agents) — Vercel Academy, авторы Cameron Youngblood и Malte Ubl

**О чём:** Практический курс по построению агента, который анализирует данные через файловую систему. Вместо векторного поиска или набивания всего в промпт — структурируй данные как файлы, дай агенту bash, и модель использует те же навыки, что и для навигации по коду.

**Что изучите:**
- Почему файловые системы работают для AI-агентов
- Определение ToolLoopAgent с bash-инструментом
- Подключение Vercel Sandbox для изолированного выполнения
- Загрузка данных и инструкций для агента
- Тестирование с реальными вопросами

**Объём:** 6 уроков, 2 секции

**Стек:** TypeScript, AI SDK, Vercel Sandbox, AI Gateway, Zod

🌐 **Сайт:** [galaersh-ai.github.io/filesystem-agents-guide](https://galaersh-ai.github.io/filesystem-agents-guide/)
📁 **Код:** [github.com/galaersh-ai/filesystem-agents-guide](https://github.com/galaersh-ai/filesystem-agents-guide)

---

### 🎓 Инженерия Harness: почему сильные модели терпят неудачу

**Источник:** [Learn Harness Engineering](https://walkinglabs.github.io/learn-harness-engineering/en/) — WalkingLabs

**О чём:** Теория и практика harness-инженерии — дисциплины, которая делает AI-кодинг-агентов надёжными. Основан на исследованиях OpenAI, Anthropic и Awesome Harness Engineering. Не про то, как сделать модель умнее, а про то, как построить среду, в которой любая модель работает лучше.

**Что изучите:**
- Почему capable-агенты всё равно терпят неудачу (gap между бенчмарками и реальностью)
- Что такое harness на самом деле (всё вне весов модели)
- Репозиторий как единый источник истины
- Почему один гигантский файл инструкций не работает
- Непрерывность между сессиями и state management
- Инициализация как отдельная фаза
- Почему агенты берутся слишком за многое и объявляют победу рано
- Feature lists как примитивы харнеса
- E2E тестирование и обсервабильность
- От ручного промптинга к автономным циклам и граф-инжинирингу
- Разборы дизайна: Pi, Claude Code, Codex, DeepSeek

**Объём:** 15 лекций + 8 проектов + библиотека шаблонов + навыки + разборы дизайна

**Стек:** AGENTS.md, feature_list.json, claude-progress.md, Codex, Claude Code

🌐 **Сайт:** [galaersh-ai.github.io/learn-harness-engineering-guide](https://galaersh-ai.github.io/learn-harness-engineering-guide/)
📁 **Код:** [github.com/galaersh-ai/learn-harness-engineering-guide](https://github.com/galaersh-ai/learn-harness-engineering-guide)

---

## Порядок изучения

Для тех, кто только начинает:

1. **Строим файлового агента** (6 уроков) — быстрый старт, минимальный агент
2. **Строим AI-кодинг агент** (38 уроков) — полный каркас с нуля
3. **Инженерия Harness** (15 лекций + проекты) — теория и продвинутые практики

---

## О переводе

Перевод выполнен с использованием [Hermes Agent](https://hermes-agent.nousresearch.com/) и модели **mimo** (Xiaomi).

**Переводчик:** Ершова Галина

Все материалы являются переводами-адаптациями открытых курсов и распространяются с разрешения авторов оригиналов. Код в примерах оставлен на английском языке как в оригинале. Промты и инструкции AI-моделей переведены на русский с сохранением структуры.

---

## Ссылки

- [AI SDK документация](https://sdk.vercel.ai/docs)
- [OpenAI: Harness engineering](https://openai.com/index/harness-engineering/)
- [Anthropic: Effective harnesses for long-running agents](https://www.anthropic.com/engineering/effective-harnesses-for-long-running-agents)
- [Anthropic: Harness design for long-running application development](https://www.anthropic.com/engineering/harness-design-for-long-running-agents)
- [Awesome Harness Engineering](https://github.com/anthropics/awesome-harness-engineering)
