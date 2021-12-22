## Этот документ описывает структуру файла styles.xml

В файле styles.xml все стили для компонентов должны быть в виде иерархии.

```
​```xml
<style name="Base" />
<style name="Base.Component">
...
</style>

<style name="Component" parent="Base.Component" />

<style name="Base.Component.Icon"/>
<style name="Icon" parent="Base.Component.Icon"/>
<style name="Icon.Circle"/>

<style name="Base.Component.Text"/>
<style name="Text" parent="Base.Component.Text" />

<style name="Base.Component.Input" />
<style name="Input" parent="Base.Component.Input" />
<style name="Input.Underline"/>
<style name="Input.Default"/>

​```
```



Ключевым элементом иерархии должен выступать объект с именем Base, из него уже вытекают остальные объекты стилей (Icon, Text, Button, Input и прочие).



