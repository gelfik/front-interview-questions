# Вопросы для собеседования на позицию frontend разработчика

## Оглавление:

- ### [TypeScript, JavaScript](#typescript-javascript)
  #### Общие вопросы
    * [Каковы основные особенности TypeScript?](#typescript-javascript-main-features)
    * [В чем преимущества использования TypeScript?](#typescript-javascript-benefits)
  #### Типы данных
    * [Какие типы данных в TypeScript?](#typescript-javascript-data-types)
    * [Как проверить на null или undefined?](#typescript-javascript-null-undefined)
    * [В чем разница между any и unknown?](#typescript-javascript-diff-any-and-unknown)
    * [Как преобразовать строку в число с помощью TypeScript?](#typescript-javascript-convert)
    * [Что такое promise и какие состояния у него есть?](#typescript-javascript-promise)
    * [Как и когда нужно использовать enum?](#typescript-javascript-enum)
  #### Область видимости и замыкание
    * [Как объявить переменную в TypeScript?](#typescript-javascript-variable)
    * [Что такое замыкание?](#typescript-javascript-circuit)
  #### Типазация
    * [Что такое интерфейс в TypeScript?](#typescript-javascript-interface)
    * [Что такое type(тип) в TypeScript?](#typescript-javascript-type)
    * [В чем разница между типом (type) и интерфейсом (interface)?](#typescript-javascript-diff-interface-and-type)
    * [Какие коллекции поддерживает TypeScript?](#typescript-javascript-collections)
    * [Что такое дженерики в TypeScript?](#typescript-javascript-generics)
    * [Перечисли утилитарные типы, которые знаешь?](#typescript-javascript-utilitarian-types)
  #### Классы
    * [Что такое классы в TypeScript?](#typescript-javascript-classes)
    * [Как управлять доступом к методам и переменным класса?](#typescript-javascript-default-modifier)
    * [Что такое getters/setters? Как их использовать?](#typescript-javascript-getter-setter)
    * [Что такое переопределение метода в TypeScript?](#typescript-javascript-override)
    * [Как вызвать конструктор базового класса из дочернего класса в TypeScript?](#typescript-javascript-constructor)
- ### [React](#react)
    * [Что такое JSX?](#react-jsx)
    * [Перечислите основные хуки?](#react-all-hooks)
    * [Что такое методы жизненного цикла компонента?](#react-lifecycle)
    * [Как обрабатывать события?](#react-detect-events)
    * [Что такое условный рендеринг?](#react-conditional-rendering)
    * [Что такое ключи (keys) в списках React-элементов и зачем они нужны?](#react-keys-in-array)
    * [Что такое "управляемые компоненты" (controlled components)?](#react-controlled-components)
    * [Как создать форму?](#react-create-form)
    * [Как реализовать условное добавление класса к элементу?](#react-conditional-add-class)
    * [Что такое фрагменты (fragments)?](#react-fragments)
    * [Что такое HOC (Higher-Order Component)?](#react-hoc)
    * [Что такое порталы (portals)?](#react-portals)
    * [Каким образом можно оптимизировать рендеринг компонентов?](#react-optimize)
    * [Как работает библиотека React Router?](#react-router)
    * [Как работает CSS-модули (CSS Modules)?](#react-css-modules)
    * [Что такое Styled Components, и как оно используется?](#react-styled-components)
    * [Какие особенности имеют хуки useEffect и useLayoutEffect?](#react-useeffect-and-uselayouteffect)
    * [Как работает "ленивая загрузка" (lazy loading) компонентов?](#react-lazy-loading)
- ### [Next](#next)
- ### [Mobx](#mobx)
- ### [Axios](#axios)
- ### [Antd](#antd)
- ### [CSS, SCSS, SASS](#css-scss-sass)
    * [Что такое препроцессоры?](#css-scss-sass-preprocessor)

## TypeScript, JavaScript

### Общие вопросы

<details name="typescript-javascript-main-features">
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

<details name="typescript-javascript-benefits">
<summary><b>В чем преимущества использования TypeScript?</b></summary>

- TypeScript вносит порядок в код.
- Проще дебажить код, т.к. ошибки видны до компиляции еще во время написания кода.
- Статическая типизация TypeScript делает код более читабельным и структурированным чем JavaScript.
- Возможность использования на разных платформах как в клиентских, так и в серверных проектах благодаря универсальной
  транспиляции.

</details>
<br>

### Типы данных

<details name="typescript-javascript-data-types">
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

<details name="typescript-javascript-null-undefined">
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

<details name="typescript-javascript-diff-any-and-unknown">
<summary><b>В чем разница между any и unknown?</b></summary>

unknown присваивается самому себе или any , а any — чему угодно.
</details>

<details name="typescript-javascript-convert">
<summary><b>Как преобразовать строку в число с помощью TypeScript?</b></summary>

Подобно JavaScript, вы можете использовать функции `parseInt` или `parseFloat` для преобразования строки в целое число
или число с плавающей запятой соответственно. Вы также можете использовать унарный оператор `+` для преобразования
строки в наиболее подходящий числовой тип, «3» становится целым числом 3, а «3.14» становится вещественным числом 3.14.
</details>

<details name="typescript-javascript-promise">
<summary><b>Что такое promise и какие состояния у него есть?</b></summary>

Promise (обещание) — это объект, представляющий завершение (или неудачу) асинхронной операции и её результат. Он
позволяет ассоциировать обработчики с асинхронным действием, тем самым избавляя от необходимости использовать обратные
вызовы (callback-функции). Они упрощают работу с асинхронными операциями, такими как AJAX-запросы или чтение файлов,
позволяя написать код, который проще понять и поддерживать.

Состояния:

1. Pending (Ожидание): Начальное состояние; асинхронная операция не завершена.
2. Fulfilled (Исполнено): Операция завершена успешно, и promise возвращает результат.
3. Rejected (Отклонено): Операция завершена с ошибкой, и promise возвращает причину отказа.

```typescript
let promise = new Promise(function(resolve, reject) {
  // Эмуляция асинхронной операции, например, запроса к серверу
  setTimeout(() => {
    // Условие успешного выполнения операции
    if (/* условие успеха */) {
      resolve("данные получены");
    } else {
      reject("ошибка при получении данных");
    }
  }, 1000);
});

promise.then((res) => {
  console.log(res);
}).catch((err) => {
  console.log(err);
});
```

Promise поддерживает цепочки вызовов (`then`), что позволяет организовывать асинхронный код последовательно и
читабельно. Кроме того, существуют вспомогательные методы, такие как `Promise.all`, `Promise.race`, `Promise.resolve`,
и `Promise.reject`, которые облегчают работу с группами асинхронных операций.

Promise — это способ организации асинхронного кода, который предоставляет более удобный и понятный интерфейс для работы
с асинхронными операциями, чем традиционные callback-функции. У каждого обещания есть три состояния: ожидание, исполнено
и отклонено, которые помогают управлять результатом асинхронных операций.
</details>

<details name="typescript-javascript-enum">
<summary><b>Как и когда нужно использовать enum?</b></summary>

В TypeScript `enum` представляют собой структуры данных постоянной длины, которые содержат набор констант. `Enum` полезны при присвоении свойств или значений, которые могут быть только определенным количеством возможных значений. Одним из распространенных примеров является значение масти одной карты в колоде игральных карт. Есть только 4 масти и не существует других возможных значений, и эти значения вряд ли изменятся. По этой причине `enum` было бы эффективным и ясным способом описания возможных мастей карты.
</details>
<br>

### Область видимости и замыкание

<details name="typescript-javascript-variable">
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

<details name="typescript-javascript-circuit">
<summary><b>Что такое замыкание?</b></summary>

Замыкание — это функция, которая запоминает своё лексическое окружение даже после того, как она выполняется вне своей
области видимости. Другими словами, функция, объявленная в определённой области видимости, сохраняет доступ к переменным
этой области, даже когда она вызывается за пределами своего первоначального контекста.

Это важно по нескольким причинам:

1. **Инкапсуляция данных:** Позволяют скрыть переменные внутри функции, делая их недоступными извне, кроме как через
   другую функцию, созданную в той же области видимости.
2. **Сохранение состояния:** Позволяют сохранять состояние между вызовами функции, без использования глобальных
   переменных.
3. **Каррирование и функциональное программирование:** Облегчают каррирование и другие техники функционального
   программирования, позволяя функциям работать с переменными, которые были в их области видимости в момент создания.

```typescript
function создатьСчетчик() {
  let количество = 0; // переменная количество "замкнута" внутри функции увеличить

  function увеличить() {
    количество += 1;
    return количество;
  }

  return увеличить;
}

const счетчик = создатьСчетчик();
console.log(счетчик()); // 1
console.log(счетчик()); // 2
```

В этом примере, функция `увеличить` имеет доступ к переменной `количество`, даже после того как `создатьСчетчик`
завершила выполнение. Это происходит благодаря механизму замыканий: `увеличить` "запоминает" переменные, которые были в
её области видимости в момент создания.

Замыкание — это когда функция запоминает и имеет доступ к переменным из своей области видимости, даже после того, как
она выполняется в другом контексте. Это позволяет функциям сохранять данные между вызовами и обеспечивать инкапсуляцию
состояния, что очень полезно для создания приватных переменных и управления состоянием в программе.
</details>
<br>

### Типазация

<details name="typescript-javascript-interface">
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

<details name="typescript-javascript-type">
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

<details name="typescript-javascript-diff-interface-and-type">
<summary><b>В чем разница между типом (type) и интерфейсом (interface)?</b></summary>

Во многих ситуациях type и interface взаимозаменяемы.

- Интерфейсы поддерживают декларативное слияние, а псевдонимы типов нет
- Типы пересечения и объединения. Можно использовать интерфейсы и псевдонимы для этих операций, но результат пересечения
  или объединения может быть только псевдоним типа
- Интерфейсы поддерживают наследование. `extends`
- Объявить новый кортеж с помощью interface нельзя

</details>

<details name="typescript-javascript-collections">
<summary><b>Какие коллекции поддерживает TypeScript?</b></summary>

**Массивы**
```typescript
let num: number[] = [1, 2, 3];
const numToo: Array<number> = [1, 2, 3];
```

**Tuples**
```typescript
const life: [string, number] = ["everything", 42];
```

**Объекты**
```javascript
const planet: { name: string; position: number } = {
	name: "earth",
	position: 3,
};
```

**Map**
```typescript
const planet = new Map<string, string>();
planet.set("name", "earth");
planet.set("position", "1");

console.log(planet);
// Map { 'name' => 'earth', 'position' => '1' }
```

**Set**
Набор - это упорядоченный список значений без дубликатов.
```typescript
const planet = new Set<string>();
planet.add("earth");

console.log(planet);
// Set { 'earth' }
```

**WeakMap**
```typescript
const planet = { bodyType: "planet" }
const weakMap = new WeakMap<{ bodyType: string }, string>();
weakMap.set(planet, "earth");
// Обьекты внутри `WeakMap` удаляются из `weakMap` при удалении обьекта, на который они ссылаются
weakMap.has(planet) // true
planet = null
weakMap.has(planet) // false
```

**WeakSet**
```typescript
let john = { name: "earth" };
const weakSet = new WeakSet<{ name: string }>();
weakSet.add(john);
// Обьекты внутри `weakSet` удаляются из `weakSet` при удалении обьекта, на который они ссылаются
weakSet.has(john) // true
john = null
weakSet.has(john) // false
```
</details>

<details name="typescript-javascript-generics">
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

<details name="typescript-javascript-utilitarian-types">
<summary><b>Перечисли утилитарные типы, которые знаешь?</b></summary>

- `Awaited<T>` - это специальный тип, который может быть использован для обозначения типа, который будет возвращен из асинхронной функции.
```typescript
async function getData(): Promise<string> {
    return 'hello';
}

let awaitedData: Awaited<ReturnType<typeof getData>>;
// теперь awaitedData может быть 'hello'
```

- `Partial<T>` - делает все свойства объекта типа T необязательными.
```typescript
interface Person {
  name: string;
  age: number;
}

let partialPerson: Partial<Person>;
// теперь partialPerson может быть { name?: string; age?: number; }
```

- `Required<T>` - делает все свойства объекта типа T обязательными.
```typescript
interface Person {
  name?: string;
  age?: number;
}

let requiredPerson: Required<Person>;
// теперь requiredPerson может быть { name: string; age: number; }
```

- `Readonly<T>` - делает все свойства объекта типа T доступными только для чтения.
```typescript
interface Point {
  x: number;
  y: number;
}

let readonlyPoint: Readonly<Point>;
// теперь readonlyPoint может быть { readonly x: number; readonly y: number; }
```

- `Record<Keys, Type>` - создает тип, который является записью с ключами, определенными в первом параметре, и значениями типа, определенного во втором параметре.
```typescript
type Keys = 'a' | 'b' | 'c';
type RecordType = Record<Keys, number>;

let record: RecordType;
// теперь record может быть { a: number, b: number, c: number }
```

- `Pick<T, K extends keyof T>` - выбирает свойства объекта типа T с ключами, указанными в K.
```typescript
interface Person {
  name: string;
  age: number;
}

let pickedPerson: Pick<Person, 'name'>;
// теперь pickedPerson может быть { name: string; }
```

- `Omit<T, K extends keyof T>` - выбирает свойства объекта типа T, исключая те, которые указаны в K.
```typescript
interface Person {
  name: string;
  age: number;
}

let omittedPerson: Omit<Person, 'age'>;
// теперь omittedPerson может быть { name: string; }
```

- `Exclude<UnionType, ExcludedMembers>` - исключает определенные типы из объединенного типа.
```typescript
type A = 'a' | 'b' | 'c';
type B = Exclude<A, 'a' | 'b'>;
// теперь B это 'c'
```

- `Extract<Type, Union>` - извлекает из типа Type только те типы, которые присутствуют в Union.
```typescript
type A = 'a' | 'b' | 'c';
type B = 'a' | 'b';
type C = Extract<A, B>;
// теперь C это 'a' | 'b'
```

- `NonNullable<Type>` - извлекает тип из Type, исключая null и undefined.
```typescript
let value: string | null | undefined;
let nonNullableValue: NonNullable<typeof value>;
// теперь nonNullableValue это string
```

- `Parameters<Type>` - извлекает типы аргументов функции Type.
```typescript
function foo(a: string, b: number) {}
type FooParameters = Parameters<typeof foo>;
// теперь FooParameters это [string, number]
```

- `ConstructorParameters<Type>` - извлекает типы аргументов конструктора Type.
```typescript
class Foo {
    constructor(a: string, b: number) {}
}
type FooConstructorParameters = ConstructorParameters<typeof Foo>;
// теперь FooConstructorParameters это [string, number]
```

- `ReturnType<Type>` - извлекает тип возвращаемого значения функции Type.
```typescript
function foo(): string { return 'hello'; }
type FooReturnType = ReturnType<typeof foo>;
// теперь FooReturnType это string
```

- `InstanceType<Type>` - извлекает тип экземпляра класса Type.
```typescript
class Foo { x: number }
type FooInstance = InstanceType<typeof Foo>;
// теперь FooInstance это { x: number }
```

- `ThisParameterType<Type>` - извлекает тип this из функции Type.
```typescript
class Foo {
    x: number;
    method(this: this): void { }
}
type ThisType = ThisParameterType<Foo["method"]>;
// теперь ThisType это Foo
```

- `OmitThisParameter<Type>` - определяет функцию без типа this.
```typescript
class Foo {
    x: number;
    method(this: this): void { }
}
type MethodType = OmitThisParameter<Foo["method"]>;
// теперь MethodType это () => void
```

- `ThisType<Type>` - добавляет тип this к функции Type.
```typescript
class Foo {
    x: number;
    method(): void { }
}
type MethodType = ThisType<Foo["method"]>;
// теперь MethodType это (this: Foo) => void
```
</details>
<br>

### Классы

<details name="typescript-javascript-classes">
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

<details name="typescript-javascript-default-modifier">
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

<details name="typescript-javascript-getter-setter">
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

<details name="typescript-javascript-override">
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

<details name="typescript-javascript-constructor">
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
<br>

## React

<details name="react-jsx">
<summary><b>Что такое JSX?</b></summary>

JSX - это встраиваемый XML-подобный синтаксис, который позволяет создавать HTML. TypeScript поддерживает встраивание,
проверку типов и компиляцию JSX непосредственно в JavaScript.
</details>

<details name="react-all-hooks">
<summary><b>Перечислите основные хуки</b></summary>

- **useState** - управления состоянием в функциональных компонентах
- **useEffect** - выполнения побочных эффектов в функциональных компонентах (например, для получения данных или подписки на события)
- **useContext** - доступа к значению контекста React в функциональном компоненте
- **useRef** - создания изменяемых ссылок на элементы или значения, которые сохраняются во время рендеринга
- **useCallback** - мемоизации функций для предотвращения ненужных повторных рендеров
- **useMemo** - запоминания значений с целью повышения производительности за счет кэширования ресурсоемких вычислений
- **useReducer** - управления состоянием с помощью функции reducer, аналогично тому, как это делается в Redux
- **useLayoutEffect** - выполнения побочных эффектов подобно useEffect, с той разницей, что эффект запускается синхронно после всех мутаций DOM

</details>

<details name="react-lifecycle">
<summary><b>Что такое методы жизненного цикла компонента?</b></summary>

- **useEffect** - выполнения побочных эффектов в функциональных компонентах (например, для получения данных или подписки на события)

- **componentDidMount** – вызывается сразу после рендеринга компонента в DOM. Обычно используется для задач инициализации, таких как вызов API или настройка слушателей событий.
- **componentDidUpdate** – вызывается при изменении реквизитов или состояния компонента. Позволяет выполнять побочные эффекты, обновлять компонент на основе изменений или запускать дополнительные вызовы API.
- **componentWillUnmount** – вызывается непосредственно перед удалением компонента из DOM. Используется для очистки ресурсов, которые были установлены в componentDidMount, например, для удаления слушателей событий или отмены таймеров.
</details>

<details name="react-detect-events">
<summary><b>Как обрабатывать события?</b></summary>

В React обработка событий происходит с использованием синтаксиса, аналогичного обработке событий в нативном JavaScript, но с некоторыми отличиями. Вот как обрабатывать события в React:

1. **Создание метода обработки события:**
   Создайте метод внутри компонента, который будет выполняться при возникновении события. Название метода обычно начинается с префикса "handle", за которым следует имя события или описательное имя.

2. **Привязка метода к элементу:**
   Привяжите созданный метод к элементу, который будет генерировать событие. Это делается с помощью JSX, указав метод как значение атрибута события.

3. **Использование аргументов:**
   Внутри метода обработки события вы можете получить доступ к объекту события и использовать его свойства, такие как `target`, чтобы получить информацию о событии.

Пример обработки клика:

```jsx
import React, { Component } from "react";

class Button extends Component {
  handleClick = () => {
    console.log("Кнопка была нажата");
  };

  render() {
    return <button onClick={this.handleClick}>Нажми меня</button>;
  }
}

export default Button;
```

В этом примере метод `handleClick` вызывается при клике на кнопку, выводя сообщение в консоль.

Важно заметить, что при передаче метода обработки события в качестве атрибута JSX, не следует вызывать его с помощью круглых скобок (например, не пишите `onClick={this.handleClick()}`), так как это вызовет выполнение метода сразу при рендеринге.
</details>

<details name="react-conditional-rendering">
<summary><b>Что такое условный рендеринг?</b></summary>

Условный рендеринг в React - это подход, при котором решается, должен ли компонент или его часть отображаться на основе какого-либо условия. Это позволяет динамически контролировать, какие элементы интерфейса будут показаны или скрыты в зависимости от состояния приложения или других факторов.

Пример условного рендеринга:

```jsx
import React, { Component } from "react";

class Greeting extends Component {
  render() {
    const isLoggedIn = this.props.isLoggedIn;

    if (isLoggedIn) {
      return <h1>Привет, пользователь!</h1>;
    } else {
      return <h1>Пожалуйста, войдите в систему.</h1>;
    }
  }
}

export default Greeting;
```

В этом примере компонент `Greeting` в зависимости от значения пропса `isLoggedIn` рендерит разные заголовки. Если `isLoggedIn` равен `true`, отображается приветствие, в противном случае - приглашение к входу в систему.

Условный рендеринг можно реализовать также с помощью тернарного оператора:

```jsx
class Greeting extends Component {
  render() {
    const isLoggedIn = this.props.isLoggedIn;

    return (
      <div>
        {isLoggedIn ? (
          <h1>Привет, пользователь!</h1>
        ) : (
          <h1>Пожалуйста, войдите в систему.</h1>
        )}
      </div>
    );
  }
}
```

Условный рендеринг особенно полезен, когда требуется адаптировать интерфейс на основе динамических данных или состояний, таких как авторизация пользователя, наличие данных и другие условия.

</details>

<details name="react-keys-in-array">
<summary><b>Что такое ключи (keys) в списках React-элементов и зачем они нужны?</b></summary>

В React, ключи (keys) - это специальные атрибуты, используемые при рендеринге списков компонентов или элементов. Они помогают React оптимизировать процесс обновления и перерисовки компонентов в списках.

Ключи назначаются каждому элементу в списке и должны быть уникальными среди своих соседних элементов. Когда React обновляет список компонентов, он использует ключи для определения, какие элементы были добавлены, удалены или изменены. Без ключей React будет перерисовывать и обновлять все элементы в списке, что может привести к ухудшению производительности.

Пример использования ключей:

```jsx
import React from "react";

const TodoList = ({ todos }) => {
  return (
    <ul>
      {todos.map((todo) => (
        <li key={todo.id}>{todo.text}</li>
      ))}
    </ul>
  );
};

export default TodoList;
```

В этом примере каждому элементу списка задач (`todo`) присваивается уникальный ключ (`todo.id`). Это позволяет React эффективно обновлять только измененные элементы, минимизируя количество перерисовок.

Ключи особенно важны при работе со списками, которые могут изменяться во времени, например, при добавлении, удалении или переупорядочивании элементов.

</details>

<details name="react-controlled-components">
<summary><b>Что такое "управляемые компоненты" (controlled components)?</b></summary>

"Управляемые компоненты" (controlled components) - это понятие, связанное с управлением состоянием форм и ввода данных в React. В управляемых компонентах значение элемента ввода (например, текстового поля или чекбокса) контролируется состоянием React компонента, а не DOM элементом.

Когда компонент контролирует значение ввода, он хранит это значение в своем состоянии и обновляет его с помощью обработчиков событий (например, при изменении текста в поле ввода). Это позволяет иметь полный контроль над данными формы и легко реагировать на изменения.

Пример управляемого компонента с текстовым полем:

```jsx
import React, { useState } from "react";

const ControlledComponent = () => {
  const [inputValue, setInputValue] = useState("");

  const handleInputChange = (event) => {
    setInputValue(event.target.value);
  };

  return (
    <div>
      <input type="text" value={inputValue} onChange={handleInputChange} />
      <p>Введенное значение: {inputValue}</p>
    </div>
  );
};

export default ControlledComponent;
```

В этом примере значение текстового поля `inputValue` связано со состоянием компонента. Когда значение текстового поля меняется, вызывается обработчик `handleInputChange`, который обновляет состояние и, следовательно, значение текстового поля.

Использование управляемых компонентов обеспечивает предсказуемость состояния, упрощает взаимодействие с данными и позволяет выполнять валидацию и другие операции над введенными данными перед их отправкой на сервер.

</details>

<details name="react-create-form">
<summary><b>Как создать форму?</b></summary>

Создание формы в React включает в себя использование HTML-элементов формы в JSX и управление вводом данных с помощью состояния. Вот как это делается:

1. **Создание компонента формы:**

Сначала создайте компонент формы и определите элементы формы внутри него, такие как текстовые поля, чекбоксы, кнопки и т.д.

```jsx
import React, { useState } from "react";

const MyForm = () => {
  const [formData, setFormData] = useState({
    name: "",
    email: "",
    // другие поля
  });

  const handleInputChange = (event) => {
    const { name, value } = event.target;
    setFormData({
      ...formData,
      [name]: value,
    });
  };

  const handleSubmit = (event) => {
    event.preventDefault();
    console.log(formData);
    // Здесь можно отправить данные на сервер или выполнить другие операции
  };

  return (
    <form onSubmit={handleSubmit}>
      <label>
        Имя:
        <input
          type="text"
          name="name"
          value={formData.name}
          onChange={handleInputChange}
        />
      </label>
      <br />
      <label>
        Email:
        <input
          type="email"
          name="email"
          value={formData.email}
          onChange={handleInputChange}
        />
      </label>
      <br />
      {/* Другие поля формы */}
      <button type="submit">Отправить</button>
    </form>
  );
};

export default MyForm;
```

2. **Управление состоянием:**

В этом примере используется хук `useState`, чтобы управлять состоянием данных формы. Обработчик `handleInputChange` вызывается при изменении полей ввода и обновляет состояние формы.

3. **Обработка отправки:**

Обработчик `handleSubmit` вызывается при отправке формы. В данном случае, мы предотвращаем стандартное поведение отправки формы на сервер с помощью `event.preventDefault()`, чтобы продемонстрировать обработку данных на клиенте.

4. **Привязка значений к полям:**

Значения полей формы связаны с состоянием формы. `value` элементов ввода устанавливается равным значениям из состояния, а при изменении полей вызывается обработчик `handleInputChange`.

5. **Отправка данных:**

После заполнения формы и нажатия кнопки отправки, данные можно использовать для отправки на сервер, выполнения операций или других необходимых действий.

</details>

<details name="react-conditional-add-class">
<summary><b>Как реализовать условное добавление класса к элементу?</b></summary>

В React вы можете условно добавить класс к элементу, используя тернарный оператор или функцию для определения классового имени. Вот примеры обоих подходов:

**1. С использованием тернарного оператора:**

```jsx
import React from "react";

const MyComponent = ({ isActive }) => {
  return (
    <div className={isActive ? "active" : "inactive"}>
      Содержимое компонента
    </div>
  );
};

export default MyComponent;
```

В этом примере класс `active` будет добавлен к элементу, если `isActive` равно `true`, иначе будет добавлен класс `inactive`.

**2. С использованием функции для определения класса:**

```jsx
import React from "react";

const MyComponent = ({ isActive }) => {
  const getClassNames = () => {
    return isActive ? "active" : "inactive";
  };

  return <div className={getClassNames()}>Содержимое компонента</div>;
};

export default MyComponent;
```

Здесь мы определяем функцию `getClassNames`, которая возвращает класс в зависимости от значения `isActive`.

Если вы хотите добавить несколько классов, вы можете использовать строковое объединение или библиотеки, такие как `classnames`.

```jsx
import React from "react";
import classnames from "classnames";

const MyComponent = ({ isActive, isHighlighted }) => {
  const classNames = classnames({
    active: isActive,
    highlighted: isHighlighted,
  });

  return <div className={classNames}>Содержимое компонента</div>;
};

export default MyComponent;
```

В этом примере `classnames` библиотека позволяет добавить несколько классов на основе объекта, где ключи - это названия классов, а значения - условия, при которых класс будет добавлен.

</details>

<details name="react-fragments">
<summary><b>Что такое фрагменты (fragments)?</b></summary>

Фрагменты (fragments) - это механизм в React, который позволяет вам группировать дочерние элементы без необходимости создавать лишние DOM-элементы. Они позволяют вернуть несколько элементов из компонента без оборачивания их в дополнительный DOM-контейнер.

До появления фрагментов, если вы хотели вернуть несколько элементов из компонента, вам приходилось обертывать их в дополнительный элемент (например, `<div>`) или использовать массив, что могло привести к лишнему уровню вложенности или проблемам с CSS.

С использованием фрагментов, это выглядит более чисто и эффективно:

```jsx
import React from "react";

const MyComponent = () => {
  return (
    <>
      <h1>Заголовок</h1>
      <p>Параграф 1</p>
      <p>Параграф 2</p>
    </>
  );
};

export default MyComponent;
```

Фрагменты могут быть объявлены с помощью пустых `<>` и `</>`, а внутри них вы можете размещать любое количество дочерних элементов.

Фрагменты особенно полезны, когда вам нужно вернуть несколько элементов из компонента, например, из условных блоков или маппинга массивов, и вы хотите избежать создания дополнительных контейнеров в DOM.

</details>

<details name="react-hoc">
<summary><b>Что такое HOC (Higher-Order Component)?</b></summary>


Высокоуровневый компонент (Higher-Order Component, HOC) - это паттерн в React, который позволяет повторно использовать логику компонентов, абстрагируя ее от самих компонентов. HOC не является частью API React, это скорее паттерн композиции компонентов.

HOC - это функция, которая принимает компонент и возвращает новый компонент с дополнительной логикой. HOC позволяют вынести общие функциональные или структурные аспекты компонентов и повторно использовать их с разными компонентами.

Пример HOC:

```jsx
import React from "react";

const withLogger = (WrappedComponent) => {
  return class WithLogger extends React.Component {
    componentDidMount() {
      console.log("Компонент был отрисован");
    }

    render() {
      return <WrappedComponent {...this.props} />;
    }
  };
};

const MyComponent = () => {
  return <div>Содержимое компонента</div>;
};

const EnhancedComponent = withLogger(MyComponent);

export default EnhancedComponent;
```

В этом примере `withLogger` - это HOC, который добавляет логирование в метод `componentDidMount`. Затем компонент `MyComponent` обертывается HOC, создавая `EnhancedComponent`.

HOC позволяют:

- Расширять функциональность компонентов без изменения самих компонентов.
- Переиспользовать код и логику между разными компонентами.
- Создавать общие паттерны для логирования, аутентификации, обработки ошибок и других аспектов.

Однако, с развитием React и появлением хуков, часть функциональности HOC теперь может быть реализована с использованием хуков, таких как `useEffect`, `useContext` и других. В большинстве случаев, использование хуков более предпочтительно.

</details>

<details name="react-portals">
<summary><b>Что такое порталы (portals)?</b></summary>

Порталы (portals) - это механизм в React, который позволяет рендерить дочерние элементы в DOM-узлы, которые находятся вне иерархии DOM-компонента. Это означает, что вы можете рендерить содержимое компонента в другой элемент вне текущего дерева компонентов.

Порталы полезны, когда вам нужно рендерить компоненты на верхнем уровне DOM (например, для создания модальных окон или всплывающих подсказок), но сохранить логику и состояние компонента внутри вашего React-приложения.

Пример использования порталов:

```jsx
import React from "react";
import ReactDOM from "react-dom";

const Modal = ({ children }) => {
  const modalRoot = document.getElementById("modal-root");
  return ReactDOM.createPortal(children, modalRoot);
};

const App = () => {
  return (
    <div>
      <p>Содержимое основного компонента</p>
      <Modal>
        <p>Содержимое модального окна</p>
      </Modal>
    </div>
  );
};

ReactDOM.render(<App />, document.getElementById("root"));
```

В этом примере компонент `Modal` использует порталы для рендеринга своего содержимого в DOM-узле с id `modal-root`. По сути, `Modal` создает "всплывающее" окно, которое рендерится на уровне верхнего уровня, но все еще имеет доступ к состоянию и методам компонента `App`.

Важно отметить, что порталы не изменяют иерархию компонентов в React-приложении, они просто рендерят содержимое в другом месте в DOM.

</details>

<details name="react-optimize">
<summary><b>Каким образом можно оптимизировать рендеринг компонентов?</b></summary>

Оптимизация рендеринга компонентов в React помогает улучшить производительность вашего приложения и обеспечить более плавный пользовательский опыт. Вот несколько способов, как можно оптимизировать рендеринг компонентов:

1. **Использование ключей (Keys)**:

   - При отображении списков элементов в React, уделяйте внимание уникальным ключам (`key`).
   - Ключи помогают React определить, какие элементы были добавлены, изменены или удалены, что помогает сократить количество изменений в DOM.

2. **Избегание ненужных рендеров**:

   - Используйте методы `shouldComponentUpdate` (в классовых компонентах) или `React.memo` (в функциональных компонентах) для предотвращения ненужных перерисовок.
   - Они позволяют проверить, действительно ли компонент нужно обновлять при изменении состояния или пропсов.

3. **Использование PureComponent и memo**:

   - Воспользуйтесь `PureComponent` (в классовых компонентах) или `React.memo` (в функциональных компонентах) для автоматической проверки изменений пропсов и состояния перед обновлением компонента.

4. **Разделение компонентов**:

   - Разбейте большие компоненты на более мелкие, чтобы уменьшить область обновления и сделать код более модульным.

5. **Использование хуков**:

   - Хуки, такие как `useMemo` и `useCallback`, позволяют кэшировать значения и колбэки, что уменьшает избыточные вычисления и обновления.

6. **Ленивая загрузка (Lazy Loading)**:

   - Используйте ленивую загрузку для отдельных компонентов с помощью `React.lazy` и `Suspense`, чтобы загружать компоненты только тогда, когда они действительно понадобятся.

7. **Оптимизированные список**:

   - Для отображения больших списков используйте библиотеки, такие как `react-virtualized` или `react-window`, чтобы рендерить только видимые элементы.

8. **Пакетное обновление (Batching)**:

   - React автоматически группирует несколько обновлений состояния или пропсов в одну операцию, чтобы уменьшить количество изменений в DOM.

9. **Использование Production Build**:

   - При развертывании приложения используйте оптимизированный "production" билд React, который включает минимизированный код и другие оптимизации.

10. **Профилирование**:
    - Используйте инструменты профилирования React, такие как React DevTools Profiler, чтобы выявить узкие места в производительности и оптимизировать их.

Оптимизация рендеринга компонентов – это постоянный процесс, так как производительность может зависеть от конкретного приложения и его контекста. Регулярное изучение новых инструментов и методов поможет улучшить производительность вашего React-приложения.

</details>

<details name="react-router">
<summary><b>Как работает библиотека React Router?</b></summary>

React Router - это популярная библиотека для управления маршрутизацией (навигацией) в приложениях на основе React. Она позволяет создавать одностраничные приложения (SPA), где контент меняется динамически без полной перезагрузки страницы. Вот как работает React Router:

1. **Установка и настройка:**
   Сначала нужно установить React Router с помощью пакетного менеджера, например, npm или yarn. После установки необходимо импортировать компоненты из библиотеки и настроить маршруты для приложения.

2. **Определение маршрутов:**
   Вы определяете маршруты в вашем приложении с помощью компонентов, предоставляемых React Router, таких как `BrowserRouter`, `Route`, `Switch` и `Link`. Компонент `BrowserRouter` оборачивает корневой компонент приложения и обеспечивает навигацию.

3. **Компоненты маршрутизации:**
   Вы используете компоненты `Route`, чтобы связать определенные маршруты с соответствующими компонентами. Например, вы можете определить маршрут "/about" и связать его с компонентом `About`.

4. **Навигация:**
   Для создания ссылок между различными маршрутами вы используете компонент `Link`. Он позволяет создавать кликабельные ссылки, которые переключаются между маршрутами без полной перезагрузки страницы.

5. **Переключение между маршрутами:**
   Когда пользователь переходит по ссылке или вводит URL, React Router определяет соответствующий маршрут и рендерит соответствующий компонент, связанный с этим маршрутом.

6. **Дополнительные возможности:**
   React Router также предоставляет дополнительные функции, такие как параметры маршрутов, вложенные маршруты, защита маршрутов и т.д.

В целом, React Router упрощает управление навигацией в вашем React-приложении, обеспечивая плавные переходы между различными "страницами" в рамках одной страницы.

</details>

<details name="react-css-modules">
<summary><b>Как работает CSS-модули (CSS Modules)?</b></summary>

CSS-модули представляют собой подход к организации стилей в приложении React, который помогает изолировать стили компонентов и избежать конфликтов имен классов. Вот как это работает:

1. **Создание модулей стилей**: Для каждого компонента создается файл с расширением `.module.css` или аналогичное с помощью препроцессоров. Например, `Button.module.css`. В этом файле определяются стили как обычно, но имена классов преобразуются в уникальные имена.

2. **Использование стилей**: В компоненте React вы можете импортировать стили из модуля, как обычный объект. Например:

   ```javascript
   import React from 'react';
   import styles from './Button.module.css';

   const Button = () => {
     return <button className={styles.button}>Нажми меня</button>;
   };

   export default Button;
   ```

   Здесь `styles.button` - это уникальное имя класса из модуля стилей.

3. **Автоматическая локализация имен классов**: При сборке проекта инструмент CSS-модулей автоматически генерирует уникальные имена классов для каждого компонента. Это предотвращает пересечение стилей между разными компонентами.

4. **Локальные стили**: Стили, определенные внутри модуля, ограничены областью видимости этого модуля. Они не пересекаются с другими стилями даже в том же файле.

5. **Поддержка CSS имен**: Вы можете использовать понятные имена классов в ваших стилях, поскольку имена классов из модулей не будут конфликтовать с глобальными именами.

6. **Дополнительные возможности**: Некоторые инструменты предоставляют дополнительные возможности, такие как наследование стилей, глобальные стили и т. д., чтобы облегчить управление стилями.

Использование CSS-модулей делает структуру стилей более четкой и упорядоченной, снижая вероятность ошибок и облегчая совместную разработку.
</details>

<details name="react-styled-components">
<summary><b>Что такое Styled Components, и как оно используется?</b></summary>

Styled Components - это библиотека для стилизации компонентов в React. Она предоставляет возможность определять стили непосредственно внутри компонентов с использованием синтаксиса шаблонных строк (template literals). Это позволяет создавать компоненты, которые включают в себя как логику, так и стили, делая код более читаемым и поддерживаемым.

Вот как работает Styled Components:

1. **Установка и импорт**: Начните с установки Styled Components через npm или yarn. После установки вы можете импортировать функции и компоненты из библиотеки в свой проект.

2. **Создание стилизованных компонентов**: Для создания стилизованных компонентов используйте функции из Styled Components. Например:

   ```javascript
   import styled from 'styled-components';

   const Button = styled.button`
     background-color: #3498db;
     color: white;
     border: none;
     padding: 10px 20px;
     cursor: pointer;
   `;
   ```

   Здесь `styled.button` создает компонент `<button>`, к которому применены указанные стили.

3. **Использование стилизованных компонентов**: Теперь вы можете использовать стилизованный компонент `Button` так же, как и обычный компонент:

   ```javascript
   import React from 'react';
   import Button from './Button';

   const App = () => {
     return (
       <div>
         <Button>Нажми меня</Button>
       </div>
     );
   };

   export default App;
   ```

4. **Передача пропсов**: Вы также можете передавать пропсы в стилизованные компоненты и использовать их внутри шаблонных строк:

   ```javascript
   const Button = styled.button`
     background-color: ${(props) => (props.primary ? '#3498db' : '#e74c3c')};
     color: white;
     border: none;
     padding: 10px 20px;
     cursor: pointer;
   `;
   ```

5. **Глобальные стили**: Вы можете использовать `createGlobalStyle` из Styled Components для определения глобальных стилей, которые будут применяться ко всему приложению.

Styled Components упрощает структурирование и управление стилями в вашем проекте, позволяя создавать компоненты, которые включают в себя стили и поведение. Она также обеспечивает поддержку динамических стилей и пропсов, что делает стилизацию компонентов более гибкой.
</details>

<details name="react-useeffect-and-uselayouteffect">
<summary><b>Какие особенности имеют хуки useEffect и useLayoutEffect?</b></summary>

`useEffect` и `useLayoutEffect` - это два хука в React, которые позволяют выполнять побочные эффекты в функциональных компонентах. Однако у них есть некоторые отличия:

1. **Время выполнения:**

   - `useEffect`: Этот хук выполняет побочные эффекты после того, как браузер обновил экран (после того, как произошел рендеринг и компонент отобразился на экране). Он не блокирует браузер и выполняется асинхронно.
   
   - `useLayoutEffect`: Этот хук выполняет побочные эффекты **синхронно**, немедленно после завершения рендеринга компонента и перед отображением изменений на экране. Он блокирует браузер до тех пор, пока все эффекты не будут выполнены.

2. **Использование:**

   - Оба хука используются для выполнения побочных эффектов, таких как отправка сетевых запросов, подписка на события или изменение DOM.
   
   - Разница заключается в том, что если вам нужно выполнить действия, зависящие от макета (layout) до того, как пользователь увидит обновленный интерфейс, вы можете использовать `useLayoutEffect`.

3. **Рекомендации:**

   - В большинстве случаев предпочтительно использовать `useEffect`, так как он не блокирует браузер и обычно достаточно эффективен для большинства сценариев.
   
   - `useLayoutEffect` стоит использовать тогда, когда вам **действительно** нужно выполнить побочные эффекты синхронно после рендеринга компонента.

Выбор между `useEffect` и `useLayoutEffect` зависит от конкретных требований вашего приложения и времени, в которое вы хотите, чтобы эффекты выполнились.
</details>

<details name="react-lazy-loading">
<summary><b>Как работает "ленивая загрузка" (lazy loading) компонентов?</b></summary>


"Ленивая загрузка" (lazy loading) - это техника оптимизации, используемая в React, чтобы отложить загрузку компонентов до тех пор, пока они действительно не понадобятся. Это помогает ускорить начальное время загрузки приложения, особенно когда приложение имеет большой объем кода.

Для реализации ленивой загрузки в React используется динамический импорт - специальная возможность JavaScript, которая позволяет загружать модули по требованию.

Пример использования ленивой загрузки компонентов с помощью динамического импорта:

```jsx
import React, { lazy, Suspense } from 'react';

const LazyComponent = lazy(() => import('./LazyComponent'));

function App() {
  return (
    <div>
      <Suspense fallback={<div>Loading...</div>}>
        <LazyComponent />
      </Suspense>
    </div>
  );
}
```

В этом примере, компонент `LazyComponent` будет загружаться асинхронно только тогда, когда он действительно нужен. Если компонент еще не загрузился, пока он не понадобится, то будет показан компонент, указанный в `fallback`.

После компонентов лениво загруженных через `lazy`, можно использовать их так же, как и другие компоненты.

Примечания:

- Ленивая загрузка работает в основном с компонентами, но также может быть применена к другим модулям JavaScript.
- Ленивая загрузка хорошо сочетается с "code splitting", позволяя разделять и загружать только те части приложения, которые действительно требуются для текущего представления.
- Не рекомендуется использовать ленивую загрузку для всех компонентов, так как это может привести к чрезмерной сложности. Вместо этого, применяйте ее там, где это действительно оправдано с точки зрения оптимизации.

</details>

<details name="react-lazy-loading">
<summary><b>Как работает "ленивая загрузка" (lazy loading) компонентов?</b></summary>


</details>

## Next

## Mobx

## Axios

## Antd

## CSS, SCSS, SASS

<details name="css-scss-sass-preprocessor">
<summary><b>Что такое препроцессоры?</b></summary>

CSS препроцессор - это программа, которая имеет свой собственный синтаксис (syntax), но может сгенерировать из него CSS
код. Существует множество препроцессоров. Большинство из них расширяет возможности чистого CSS, добавляя такие опции
как: примеси, вложенные правила, селекторы наследования и др. Эти особенности облегчают работу с CSS: упрощают чтение
кода и его дальнейшую поддержку.

Преимущества:

- Возможность записать код короче
- Легкость изучения
- Простота применения
- Логичная и понятная структура
- Добавление миксинов
- Модули

</details>
