# Хук useFetch

Переиспользуемый и типизированный React-хук для выполнения HTTP-запросов с поддержкой query-параметров, обработки ошибок, загрузки и отмены запросов.

## Установка

Просто скопируйте файл useFetch.tsx в ваш проект. Внешние зависимости отсутствуют.

## API

useFetch<T>(url: string)
Параметры:
url — базовый URL, по которому будет отправлен запрос.

**Возвращает:**
data: T | null — полученные данные.

isLoading: boolean | null — состояние загрузки.

error: string | null — сообщение об ошибке (если произошла).

refetch: (options?: { params?: Record<string, string> }) => void — ручной вызов запроса с возможностью указать параметры.

---

# useHover

Хук `useHover` позволяет отслеживать наведение мыши на DOM-элемент.

Хук возвращает объект с:

- `hovered` — булевое значение, указывающее, наведена ли мышь на элемент.
- `ref` — ссылка, которую необходимо установить на нужный элемент.

Под капотом хук использует `addEventListener` для `mouseover` и `mouseout`, а также `useRef` для отслеживания DOM-узла.

---

# useViewportSize Hook

`useViewportSize` — это кастомный хук для получения текущих размеров окна (ширины и высоты) в браузере и автоматического обновления этих значений при изменении размера окна.

## Установка

Чтобы использовать хук `useViewportSize` в своём проекте, скопируйте файл с хуком в свой проект.

---

# useLocalStorage Hook

`useLocalStorage` — это кастомный React хук для работы с данными в `localStorage`. Он позволяет легко сохранять, извлекать и удалять данные из `localStorage`, при этом синхронизируя состояние компонента с хранилищем.

## Установка

Для использования этого хука, просто скопируйте файл в ваш проект и импортируйте его в компоненты, где вам нужно работать с `localStorage`.
