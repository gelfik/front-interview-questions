# Вопросы для собеседования на позицию frontend разработчика

## Оглавление:

- [TypeScript, JavaScript](#typescript-javascript)
    * [Каковы основные особенности TypeScript?](#typescript-javascript-main-features)
    * [В чем преимущества использования TypeScript?](#typescript-javascript-benefits)
    *
    * [Какие типы данных в TypeScript?](#typescript-javascript-data-types)
    * [Как объявить переменную в TypeScript?](#typescript-javascript-variable)
    * [Как проверить на null или undefined?](#typescript-javascript-null-undefined)
    * [Как преобразовать строку в число с помощью TypeScript?](#typescript-javascript-convert)
    *
    *
    * [Что такое интерфейс в TypeScript?](#typescript-javascript-interface)
    * [Что такое type(тип) в TypeScript?](#typescript-javascript-type)
    * [Что такое дженерики в TypeScript?](#typescript-javascript-generics)
    *
    * [Что такое классы в TypeScript?](#typescript-javascript-classes)
    * [Как управлять доступом к методам и переменным класса?](#typescript-javascript-default-modifier)
    * [Что такое getters/setters? Как их использовать?](#typescript-javascript-getter-setter)
    * [Что такое переопределение метода в TypeScript?](#typescript-javascript-override)
    * [Как вызвать конструктор базового класса из дочернего класса в TypeScript?](#typescript-javascript-constructor)
    *
    * [Что такое JSX?](#typescript-javascript-jsx)
- [React](#react)
- [Next](#next)
- [Mobx](#mobx)
- [Axios](#axios)
- [Antd](#antd)
- [CSS, SCSS, SASS](#css-scss-sass)

## TypeScript, JavaScript

<section name="typescript-javascript-main-features">
<details>
<summary><b>Каковы основные особенности TypeScript?</b></summary>

- **Кроссплатформенность**: Компилятор TypeScript можно установить в любой операционной системе: Windows, macOS и Linux.
- Объектно-ориентированный язык: TypeScript предоставляет все стандартные функции ООП, такие, как классы, интерфейсы и
  модули.
- **Статическая типизация**: TypeScript использует статическую типизацию и помогает проверять типы во время компиляции.
  Таким образом, вы можете обнаружить ошибки при написании кода без запуска скрипта.
- **Необязательная статическая типизация**: TypeScript также допускает использование динамической типизации, если вы
  привыкли к ней в JavaScript.
- **Манипуляции с DOM**: Вы можете использовать TypeScript для управления DOM для добавления или удаления элементов
  клиентской веб-страницы.

</details>
</section>

<section name="typescript-javascript-benefits">
<details>
<summary><b>В чем преимущества использования TypeScript?</b></summary>

- TypeScript вносит порядок в код.
- Проще дебажить код, т.к. ошибки видны до компиляции еще во время написания кода.
- Статическая типизация TypeScript делает код более читабельным и структурированным чем JavaScript.
- Возможность использования на разных платформах как в клиентских, так и в серверных проектах благодаря универсальной
  транспиляции.

</details>
</section>
<br>

<section name="typescript-javascript-data-types">
<details>
<summary><b>Какие типы данных в TypeScript?</b></summary>

- **Number**: используется для представления значений чисел. Все числа в TypeScript хранятся как значения с плавающей
  запятой.
- **String**: представляет собой последовательность символов, хранящуюся как код Unicode UTF-16. Строки заключаются в
  одинарные или двойные кавычки.
- **Boolean**: логический тип данных. Имеет значение true или false.
- **Object**: данные с парой ключ-значение.
- **Array**: тип обозначающий массивы.
- **Enum**: перечисления.
- **Symbol**: тип данных, экземпляры которого уникальны и неизменяемы.
- **Null**: Null представляет переменную, значение которой не определено.
- **Undefined**: литерал, который является отправной точкой всех переменных.
- **Never**: тип для переменной, у которой отсутствие значение.
- **Void**: тип, присвоенный методам, не имеющим возвращаемого значения.
- **Any**: произвольный тип.

</details>
</section>

<section name="typescript-javascript-variable">
<details>
<summary><b>Как объявить переменную в TypeScript?</b></summary>

Вы можете создавать переменные тремя способами: `var`, `let` и `const`.

`var` - это старый стиль объявления переменных.

`let` - это способ объявления переменных в TypeScript по умолчанию. По сравнению с `var` `let` уменьшает количество
ошибок времени компиляции и повышает читаемость кода.

```typescript
let num: number = 1;
```

`const` создает постоянную переменную, значение которой не может измениться. Он использует те же правила области
видимости, что и let, и помогает снизить общую сложность программы.

```typescript
const num: number = 100;
```

</details>
</section>

<section name="typescript-javascript-null-undefined">
<details>
<summary><b>Как проверить на null или undefined?</b></summary>

Рекомендуется проверять `== null` как на `undefined`, так и `null`.
Также Nullish Coalescing (оператор `??`) помогает проверить, является ли переменная `null` или `undefined`.
С оператором `??` вместо длинной проверки

```typescript
message = undefined;

function getMessage() {
  if (this.message !== null && this.message !== undefined) {
    return "default message";
  }
  return this.message;
}
```

можно написать так:

```typescript
message = undefined;

function getMessage() {
  return this.message ?? 'Default message';

}
```

</details>
</section>

<section name="typescript-javascript-convert">
<details>
<summary><b>Как преобразовать строку в число с помощью TypeScript?</b></summary>

Подобно JavaScript, вы можете использовать функции `parseInt` или `parseFloat` для преобразования строки в целое число
или число с плавающей запятой соответственно. Вы также можете использовать унарный оператор `+` для преобразования
строки в наиболее подходящий числовой тип, «3» становится целым числом 3, а «3.14» становится вещественным числом 3.14.
</details>
</section>
<br>

<section name="typescript-javascript-interface">
<details>
<summary><b>Что такое интерфейс в TypeScript?</b></summary>

Интерфейс определяет свойства и методы, которые объект должен реализовать. Другими словами, интерфейс - это определение
кастомного типа данных, но без реализации.

```typescript
interface IEmployee {
  empCode: number;
  empName: string;
  getSalary: (number) => number; // arrow function
  getManagerName(number): string;
}
```

</details>
</section>

<section name="typescript-javascript-type">
<details>
<summary><b>Что такое type(тип) в TypeScript?</b></summary>

Тип определяет свойства и методы, которые объект должен содержать. Другими словами, тип - это определение кастомного
типа данных, но без реализации.

```typescript
type IEmployee = {
  empCode: number;
  empName: string;
  getSalary: (number) => number; // arrow function
  getManagerName(number): string;
}
```

</details>
</section>

<section name="typescript-javascript-generics">
<details>
<summary><b>Что такое дженерики в TypeScript?</b></summary>

Generics - это инструмент, который позволяет создавать компоненты, которые можно переиспользовать. Он создает компонент,
который может работать с различными типами данных. Это позволяет пользователям использовать свои собственные типы.
Generics гарантируют, что программа масштабируемой в долгосрочной перспективе.

```typescript
function identity<T>(arg: T): T {
  return arg;
}

let output1 = identity<string>("myString");
let output2 = identity<number>(100);
```

</details>
</section>
<br>

<section name="typescript-javascript-classes">
<details>
<summary><b>Что такое классы в TypeScript?</b></summary>

Классы представляют собой общие поведения и атрибуты группы связанных объектов.

Например, нашим классом может быть `Student`, у каждого из которых есть метод `attendClass`. С другой стороны, `John`
является отдельным экземпляром типа `Student` и может иметь дополнительные уникальные поведения, такие
как `attendExtracurricular`.

Вы объявляете классы с помощью ключевого слова `class`:

```typescript
class Student {
  studCode: number;
  studName: string;

  constructor(code: number, name: string) {
    this.studName = name;
    this.studCode = code;
  }
}
```

</details>
</section>

<section name="typescript-javascript-default-modifier">
<details>
<summary><b>Как управлять доступом к методам и переменным класса?</b></summary>

По умолчанию все члены класса в TypeScript являются `public` (общедоступными).

- `public` - доступны в определяющих их классах, их потомках, а также к ним можно обращаться через экземпляр или, в
  случае статических членов, через ссылку на класс.

```typescript
class Animal {
  public nickname: string;

  constructor() {
    this.nickname = 'animal';
  }
}

class Bird extends Animal {
  constructor() {
    super();
    super.nickname = 'bird';
  }
}

let animal: Animal = new Animal();
animal.nickname = 'newanimal';

let bird: Bird = new Bird();
bird.nickname = 'newbird';
```

- `private` - доступны только контексту класса, в котором они определены.

```typescript
class Animal {
  private metainfo: string;

  constructor() {
    this.metainfo = '...';
  }
}

class Bird extends Animal {
  constructor() {
    super();
    super.metainfo = 'bird'; // Error
  }
}

let animal: Animal = new Animal();
animal.metainfo = 'newanimal'; // Error

let bird: Bird = new Bird();
bird.metainfo = 'newbird'; // Error
```

- `protected` - доступны только контексту класса, в котором они определены, а также всем его потомкам. Попытка
  обратиться к членам, помеченным как `protected`, снаружи, приведет к возникновению ошибки.

```typescript
class Animal {
  protected isUpdate: boolean;

  constructor() {
    this.isUpdate = false;
  }
}

class Bird extends Animal {
  constructor() {
    super();
    super.isUpdate = false;
  }
}

let animal: Animal = new Animal();
animal.isUpdate = true; // Error

let bird: Bird = new Bird();
bird.isUpdate = true; // Error
```

</details>
</section>

<section name="typescript-javascript-getter-setter">
<details>
<summary><b>Что такое getters/setters? Как их использовать?</b></summary>

Геттеры и сеттеры - это особые типы методов, которые помогают делегировать различные уровни доступа к частным переменным
в зависимости от потребностей программы.

Геттеры позволяют ссылаться на значение, но не могут его редактировать. Сеттеры позволяют изменять значение переменной,
но не видеть ее текущее значение. Это важно для достижения инкапсуляции.

Например, новый работодатель может получить количество сотрудников в компании, но не имеет разрешения устанавливать
количество сотрудников.

```typescript
const fullNameMaxLength = 10;

class Employee {
  private _fullName: string = "";

  get fullName(): string {
    return this._fullName;
  }

  set fullName(newName: string) {
    if (newName && newName.length > fullNameMaxLength) {
      throw new Error("fullName has a max length of " + fullNameMaxLength);
    }

    this._fullName = newName;
  }
}

let employee = new Employee();
employee.fullName = "Bob Smith";

if (employee.fullName) {
  console.log(employee.fullName);
}
```

</details>
</section>

<section name="typescript-javascript-override">
<details>
<summary><b>Что такое переопределение метода в TypeScript?</b></summary>

Переопределение метода - это процесс, в котором методы базового класса переопределяются в дочернем классе.

```typescript
class Person {
  doEat() {
    console.log("Person eats food.");
  }
}

class Employee extends Person {
  doEat() {
    console.log("Employee eats food.");
  }
}

let emp = new Employee();
emp.doEat(); // Output: Employee eats food.
```

</details>
</section>

<section name="typescript-javascript-constructor">
<details>
<summary><b>Как вызвать конструктор базового класса из дочернего класса в TypeScript?</b></summary>

Вы можете использовать функцию `super()` для вызова конструктора базового класса.

```typescript
class Animal {
  name: string;

  constructor(theName: string) {
    this.name = theName;
  }

  move(distanceInMeters: number = 0) {
    console.log(`${ this.name } moved ${ distanceInMeters }m.`);
  }
}

class Snake extends Animal {
  constructor(name: string) {
    super(name);
  }

  move(distanceInMeters = 5) {
    console.log("Slithering...");
    super.move(distanceInMeters);
  }
}
```

</details>
</section>
<br>

<section name="typescript-javascript-jsx">
<details>
<summary><b>Что такое JSX?</b></summary>

JSX - это встраиваемый XML-подобный синтаксис, который позволяет создавать HTML. TypeScript поддерживает встраивание,
проверку типов и компиляцию JSX непосредственно в JavaScript.
</details>
</section>

## React

## Next

## Mobx

## Axios

## Antd

## CSS, SCSS, SASS
