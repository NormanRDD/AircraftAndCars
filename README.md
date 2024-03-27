# testtask
Подправлены шрифты

App.vue

// Заменено имя переменной data на items, инициализированная с помощью reactive // В виду того что ref больше расчитана для реактивности примитивных данных нежели для массивов и объектов. // Так же и для selectedItem

// Заменен интерфейс any на предназначенный для этого Product

// В операторе switch использованы константы вместо жестко закодированных строковых значений.

ItemList.vue

// Пропсы items определены через defineProps для ясности и типобезопасности. // Эмиттер click определен через defineEmits для ясности и типобезопасности. // selectedItem определен с помощью reactive // Добавлен комментарий для обработчика onClick, чтобы пояснить его назначение. // Убрана дублирование стилей для класса .itemSelected и .item.

ItemContent.vue
// Заменено Watch на Computed свойство
// Заменен ref на reactive для объекта innerItem. // Добавлен обработчик addItem для добавления нового элемента. // Обновлен наблюдатель watch, чтобы пересоздавать реактивный объект innerItem при изменении props.item.
## Project setup
```
yarn install
```

### Compiles and hot-reloads for development
```
yarn serve
```

### Compiles and minifies for production
```
yarn build
```

### Lints and fixes files
```
yarn lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
