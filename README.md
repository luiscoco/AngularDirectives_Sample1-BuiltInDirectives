# Built-in Directives

https://angular.io/guide/built-in-directives

https://stackblitz.com/~/github.com/luiscoco/AngularDirectives_Sample1-BuiltInDirectives

In Angular, built-in directives are pre-defined instructions that can be applied to HTML elements to manipulate their behavior or appearance. These directives are provided by Angular itself and are available for use without requiring any additional configuration or imports.

Here are some commonly used built-in directives in Angular:

## *ngIf
This directive is used to conditionally render elements in the DOM based on a given expression. It adds or removes the element from the DOM based on the truthiness of the expression.

```typescript
<div *ngIf="isLoggedin">User is logged in</div>
```

In this example, the div element will only be displayed if the isLoggedin property evaluates to true.

## *ngFor
This directive is used for iterating over a collection and rendering elements dynamically. It allows you to repeat a portion of HTML markup for each item in an array or an iterable object.

```typescript
<ul>
  <li *ngFor="let item of items">{{ item }}</li>
</ul>
```

In this example, each item in the items array will be rendered as a list item (li).

## *ngSwitch
This directive is used for conditionally displaying content based on multiple cases. It works similar to a switch-case statement.

```typescript
<div [ngSwitch]="color">
  <div *ngSwitchCase="'red'">Red color selected</div>
  <div *ngSwitchCase="'blue'">Blue color selected</div>
  <div *ngSwitchCase="'green'">Green color selected</div>
  <div *ngSwitchDefault>Color not selected</div>
</div>
```
  
In this example, based on the value of the color variable, the corresponding div block will be displayed.

## [ngClass]
This directive is used to dynamically apply CSS classes to an element based on a condition.

```typescript
<div [ngClass]="{ 'active': isActive, 'disabled': isDisabled }">Some content</div>
```

In this example, the CSS class active will be applied if the isActive property is true, and the disabled class will be applied if the isDisabled property is true.

These are just a few examples of the built-in directives in Angular. There are several others available that provide various functionalities to make development easier and more efficient.
