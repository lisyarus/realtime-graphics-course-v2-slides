1. Введение
	1. Разделы компьютерной графики
	2. О чём этот курс
	3. История и современное состояние графических API
	4. Подробнее про место WebGPU среди современных API, wgpu-native
	5. Инициализация WebGPU: библиотека SDL3, instance, device, queue, surface texture
	6. Полезные ресурсы: www.w3.org/TR/webgpu/, GPU Gems, SIGGRAPH
	Практика: рисуем треугольник
2. Конвейер, проекции, шейдеры
	1. Растеризация
	2. Графический конвейер
	3. Шейдеры, язык шейдеров WGSL
	4. Интерполяция атрибутов
	5. Push-constants (immediates)
	6. Аффинное пространство, аффинные преобразования
	7. Однородные координаты, матрицы аффинных преобразований
	Практика: рисуем вращающийся разноцветный треугольник
3. Основы рендеринга в WebGPU, часть 1
	1. Пайплайны
	2. Вершины и атрибуты: форматы, дубликация вершин
	3. Вершинные буферы
	4. Типы примитивов
	5. Индексный буффер, индексированный рендеринг, primitive restart
	6. Instanced рендеринг
	Практика: рисуем кривые Безье
4. Основы рендеринга в WebGPU, часть 2
	1. Камера и виды проекции
	2. Буфер глубины, тест глубины
	3. Perspective-corrent интерполяция атрибутов
	Практика: рисуем модель stanford bunny
5. Текстуры
	1. Текстуры, texture view
	2. Виды текстур: 1D/2D/3D, cubemap
	3. Samplers
	3. Bind группы
	5. Фильтрация текстур, tricubic interpolation
	6. Mipmaps
	7. Анизотропная фильтрация
	8. Выбор mipmap, dFdx/dFdy
	9. Форматы изображений, libpng, libjpeg, stb_image
	10. Сжатые текстуры
	Практика: рисуем текстурированный квадрат
6. Основы рендеринга в WebGPU, часть 3
	1. Blending
	2. Stencil буфер, stencil тест
	3. Render-to-texture
	4. Постобработка кадра
	Практика: рисуем модель stanford dragon с пост-обработкой
7. Освещение
	1. Физика света
	2. Уравнение распространения света (уравнение рендеринга)
	3. Описание материалов поверхностей
	4. Модели освещения
	5. Виды источников света
	Практика: рисуем модель blender suzanna с освещением
8. Тени, часть 1
	1. Теория теней
	2. Алгоритм shadow volumes
	3. Геометрические шейдеры
	4. Compute шейдеры
	5. Алгоритм shadow mapping
	Практика: реализуем алгоритм shadow mapping с PCF и размытием
9. Тени, часть 2
	1. Convolusion shadow maps: ESM, VSM
	2. Shadow mapping на больших сценах: PSM, CSM
	3. Ambient occlusion
	Практика: реализуем алгоритм variance shadow mapping с размытием
10. Advanced освещение
	1. Normal mapping
	2. Material mapping
	3. Environment mapping
	4. Отражения
	5. Много источников света: storage buffers, deferred shading
	Практика: реализуем алгоритмы normal mapping и environment mapping
11. Цветокоррекция
	1. HDR
	2. Tone mapping
	3. Коррекция гаммы, sRGB
	4. Color banding
	5. Dithering
	Практика: реализуем систему частиц на compute шейдерах
12. AA, Volume rendering
	1. Antialiasing: MSAA, SMAA, FXAA
	2. Уравнение объёмного рендеринга (volume rendering)
	3. Рассеяние, фазовая функция
	4. Алгоритмы объёмного рендеринга: slicing, splatting, raymarching
	Практика: рисуем рассеивающее облако
13. Анимации
	1. Easing functions
	2. Keyframe анимации
	3. Bitmap анимации
	4. Кватернионы
	5. Иерархии объектов и преобразований
	6. Скелетная анимация
	7. Physics-based animation, inverse kinematics
	Практика: рисуем анимированную 3D модель
14. Оптимизация
	1. Поиск bottleneck'а
	2. Timestamp queries
	3. Основные техники: batching, instancing, LOD
	4. Frustum culling, SAT, BSP
	5. Occlusion culling
	Практика: рисуем много моделей с LOD и frustum culling, меряем производительность
15. Рендеринг текста
	1. Представление текста: кодировки, шрифты, глифы, лигатуры
	2. Библиотеки: harfbuzz, freetype
	3. Растровые шрифты
	4. Векторные шрифты
	5. SDF/MSDF шрифты
	Практика: рисуем текст MSDF-шрифтом
