# Описание #

> Субплагин предназначен для декодирования и просмотра изображений через интерфейс GDI+. Имеет ряд преимуществ, по сравнению с стандартным декодером GDI+ из комплекта PicView2:
    * Быстрое масштабирование/панорамирование без потери качества
    * Фоновое декодирование в отдельном потоке
    * Опережающее декодирование соседних изображений
    * Поддержка эскизов (thumbnail) для быстрого листания
    * Поворот и сохранение повернутых изображений
    * Автоповорот изображений по EXIF

> Требуется версия PicView2 модифицированная Maximus5, Mod16(+):<br>
<blockquote><a href='http://code.google.com/p/conemu-maximus5/'>http://code.google.com/p/conemu-maximus5/</a></blockquote>

<blockquote>Обсуждение:<br>
<a href='http://forum.farmanager.com/viewtopic.php?f=5&t=5434'>http://forum.farmanager.com/viewtopic.php?f=5&amp;t=5434</a></blockquote>

<h2>Загрузить</h2>

<ul><li><a href='http://far-plugins.googlecode.com/files/GDIPlus.v5.rar'>GDIPlus 1.0.5 decoder for PicView2 (PVD)</a></li></ul>

<hr />

<h1>История изменений</h1>

<h2>Ver 1.0.5</h2>

<ul><li>Улучшение качества отображения увеличенных изображений.</li></ul>

<ul><li>Возможность при просмотре отключать/включать сглаживание увеличенных изображений - Ctrl-T</li></ul>

<ul><li>Оптимизация поворотов: при повороте не делается повторного декодирования.</li></ul>

<h2>Ver 1.0.4</h2>

<ul><li>Возможность ручного поворота и сохранения повернутых изображений. Субплагин самостоятельно обрабатывает нажатия клавиш и поддерживает следующие команды:</li></ul>

<table><thead><th> >      </th><th> Поворот по часовой стрелке </th></thead><tbody>
<tr><td> <      </td><td> Поворот против часовой стрелки </td></tr>
<tr><td> Ctrl+> </td><td> X-Flip </td></tr>
<tr><td> Ctrl+< </td><td> Y-Flip </td></tr>
<tr><td> F2     </td><td> Сохранение </td></tr>
<tr><td> Alt+F2 </td><td> Альтернативное сохранение </td></tr></tbody></table>

<blockquote>Поддерживаются 2 метода сохранения повернутых изображений:<br>
<ol><li>Путем трансформации. Данный метод может приводить к потери качества для jpg изображений (о чем плагин предупредит)<br>
</li><li>Путем коррекции EXIF заголовка (только для форматов JPEG и TIFF)</li></ol></blockquote>

<blockquote>По умолчанию F2 сохраняет первым методом а Alt+F2 - вторым, умолчания можно изменить в настройках плагина.</blockquote>

<ul><li>Во время просмотра изображений плагин не блокирует файл изображения, как раньше (однако пока файл блокируется для анимированных изображений)</li></ul>

<ul><li>Различные оптимизации и исправления ошибок</li></ul>


<h2>Ver 1.0.3</h2>

<ul><li>Опциональный автоповорот по EXIF.</li></ul>


<h2>Ver 1.0.2</h2>

<ul><li>При 100% масштабе используется BitBlt вместо StretchBlt, не должно быть эффекта сглаживания</li></ul>

<ul><li>Опция "Decode on Reduce". При ее включении при уменьшении масштаба изображение декодируется в пониженном разрешении, вместо того чтобы масштабироваться при выводе. В некоторых случаях может наблюдаться улучшение качества изображения (а в других - наоборот, ухудшение, так что опция по умолчанию выключена)