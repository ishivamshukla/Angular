## Angular

### What is Angular?

- Angular is a JavaScript framework, built using TypeScript for building web applications.

- It is developed and maintained by Google and is used for building complex, large-scale, and scalable applications.

- Angular uses a component-based architecture for building applications.

- Angular is called a framework because it comes with batteries included(Routing, forms management, client-server communication and more...).

### Why Angular?

Angular is a framework which means it comes with many built-in features, such as:

- Component-based architecture
- Two-way data binding
- Dependency Injection
- Built-in TypeScript support
- Strong template language
- Built-in Routing
- Awesome community support

### React v/s Angular

React and Angular are both popular JavaScript frameworks for building web applications, but they have some key differences in terms of their design philosophy, architecture, and use cases.

- React is a JavaScript library for building user interfaces, whereas Angular is a full-featured framework for building web applications.

- React uses a virtual DOM (Document Object Model) to improve the performance of updates and rendering. This allows React to update only the specific components that need to be changed, rather than re-rendering the entire application. Angular uses a real DOM, which can be less performant on large and complex applications.

- React is more flexible and easy to learn, it allows you to use it with other libraries and frameworks, whereas Angular follows a more opinionated approach and provides a set of conventions and best practices to follow.

- In terms of use cases, React is generally better suited for building small to medium-sized web applications, whereas Angular is a better choice for building large-scale, complex web applications.

### Brief history of Angular

- Angular(AngularJS) was initially released in 2010 by Google. It was developed by a team of engineers led by Misko Hevery and Adam Abrons. This initial release was a JavaScript framework for building dynamic web applications, and it quickly gained popularity among developers.

- In 2016, Google released Angular 2, a complete rewrite of the original framework. Angular 2 introduced a number of new features and improvements, such as a component-based architecture, improved performance, and support for mobile devices.

- This rewrite of Angular 2 (commonly now known as Angular) was a breaking change as it was re-written with TypeScript from the ground up and had backward compatibility issues.

- After Angular 2 we got 4, 5, 6 and so on and all of them are now referred to as Angular. The current Angular version is 15

### Starting with Angular

- Before starting Angular we need the basic knowledge of HTML, CSS, and JavaScript (Knowledge of TypeScript is helpful, but not required).

- We need to have NodeJS installed in our system along with the npm package manager

### Installing Angular

- To set up a project we need to use Angular CLI and to use Angular CLI we need to install it in our system first

- To install Angular CLI run the following command

```bash
npm install -g @angular/cli
```

- The above command will install the Angular CLI globally in your system

### Scaffolding a new Angular web application

- Now we can use ng command to scaffold a new Angular project. (We got ng command after installing Angular CLI)

- Run the following command in your terminal to scaffold a new Angular project with the help of Angular CLI

```bash
ng new <app_name>
```

- The ng new command prompts you for information about features to include in the initial app. Accept the defaults by pressing the Enter or Return key.

- The Angular CLI installs the necessary Angular npm packages and other dependencies. This can take a few minutes.

### Run the application

- After successful app installation, cd in to the folder

```bash
cd <app_name>
```

- Now run the serve command inside the Angular project folder

```bash
ng serve
```

- If your installation and setup was successful, you should see a welcome page with some helpful links

### Understanding Angular folder/files structure

- Explain the folder structure

### What the TypeScript???

- What is TypeScript?

  - TypeScript is an open-source programming language developed and maintained by Microsoft. It is a typed superset of JavaScript that compiles to plain JavaScript.

- Installing and creating first TypeScript program

  - You need to have node installed.
  - Do `npm init` to create a `package.json` file.
  - Install TypeScript `npm i typescript`.
  - Initialize TypeScript `npx tsc --init`

- After that you will find a tsconfig.json file in your root directory.

- Let us create a file app.ts and play with TypeScript

### Important data types in TypeScript

- string
- number
- boolean
- array
- object
- any
- undefined

### Types with examples

- string

  - ```ts
    const myStr: string = "My Name";
    ```

- number

  - ```ts
    const myNum: number = 123;
    ```

- boolean

  - ```ts
    const myBool: boolean = true;
    ```

- array

  - ```ts
    const myArr: string[] = ["One", "Two", "Three"];
    ```

  - ```ts
    const myArr: number[] = [1, 2, 3];
    ```

- object

  - ```ts
    const myObj: { name: string; age: number } = { name: "name", age: 100 };
    ```

- any

  - ```ts
    const myObj: any = { name: "name", age: "45" };
    ```
  - Note: Avoid using any as much as you can.

- undefined
  - ```ts
    const notDefined: undefined = undefined;
    ```

### Program with TypeScript

```ts
const num1: number = 45;
const num2 = 55;

const sumTwo = (a: number, b: number): number => {
  return a + b;
};

console.log(sumTwo(num1, num2));
```

### interface in TypeScript

```ts
// This is how we create an interface
interface ISumTwo {
  (num1: number, num2: number): number; // A function which accepts 2 numerical inputs(num1, num2) and returns a numerical output(sum of num1 & num2)
}

const num1: number = 45;
const num2 = 55;

const sumTwo: ISumTwo = (a, b) => {
  return a + b;
};

console.log(sumTwo(num1, num2));
```
