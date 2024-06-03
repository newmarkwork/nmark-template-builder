# Сборка GULP/WEBPACK

## Используемые модули:

- gulp : таск-менеджер

### PUG

- gulp-pug : шаблонизатор PUG
- gulp-diffable-html : HTML-форматтер
- gulp-htmlhint : валидатор HTML-кода. Файл с кофигурацией: .htmlhintrc

### SCSS

- sass, gulp-sass : препроцессор SASS
- gulp-autoprefixer : создание CSS-префиксов
- gulp-clean-css : минификация CSS

### SERVER

- browser-sync : запуск локального сервера

### JS

- @babel/core : компилятор кода ES6 в ES5
- gulp-better-rollup : плагин, который позволяет нам использовать Rollup.
- rollup - сборщик модулей JavaScript, который позволяет нам использовать ES6 в нашем коде
- rollup-plugin-babel : плагин Rollup, который интегрирует Babel в процесс объединения
- rollup-plugin-node-resolve : плагин Rollup, позволяющий использовать сторонние модули в node_modules
- rollup-plugin-commonjs : плагин Rollup, преобразующий модули CommonJS в ES6(чтобы мы могли без проблем импортировать их)
- gulp-uglify : минификация JavaScript
- gulp-strip-debug : удаление операторов консоли, предупреждений и отладчика из кода JavaScript

### IMAGES AND SVGS

- gulp-svgstore : объединение SVG-файлов в один спрайт-файл

### OPTIMIZATION

- gulp-sharp-optimize-images : оптимизация и конвертация изображений
- gulp-purgecss : удаление неиспользуемого CSS
- gulp-svgmin : минификация SVG-файлов

### ДОПОЛНИТЕЛЬНЫЕ ПЛАГИНЫ

- del : удаление прежней сборки, перед запуском новой
- gulp-if : использование условий в тасках
- merge-stream : объединие несколько тасков в один
- gulp-plumber : вывода ошибок при сборке проекта
- gulp-rename : форматирование имени файла
- gulp-concat : конкатенация файлов
- gulp-newer : передача только тех исходных файлов, которые новее соответствующих файлов назначения.
- gulp-cheerio : манипуляция HTML и XML файлами
- gulp-replace : замена строк

## gulp.config.js

Файл, содержащий в себе все основные пути к ресурсам сборки

## gulpfile.js

Файл сборки. Импортирует в себя таски из папки "./gulp/tasks"

- для запуска в режиме разработки используем команду gulp start
- для сборки проекта используем команду gulp build