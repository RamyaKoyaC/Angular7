Angular 7 from scratch 

#### 1 - How to install Angular 7? 
In Command Line, 
`npm install -g @angular/cli`

#### 2 - How to create a new project? 
`ng new ng7-pre`

#### 3 - Angular will ask you questions like...
Would you like to add Angular routing? Yes
Which stylesheet format would you like to use? SCSS

--> You can enter any stylesheet format you want to. 

#### 4 - Next, navigate to the folder of your project

#### 5 - Later, open any code editor to start working on changes

#### 6 - To run the Angular Project on the localhost 
`ng serve -o`

#### In Angular, we have components 
In each component we have 
1. HTML template
2. Logic 
3. Stlyling - CSS 

- Initially when we create a project, as a starter we get a component under /src/app/ in which we have files like 
/app.component.html
/app.component.scss
/app.component.ts --> This is where the heart lies. 

In the ts file we write the logic under "export class" line of the code. We can create customised components using commands like 

`ng generate component test`
a shortcut for this can be 
`ng g c test`
g- generate 
c-component 
test is just the name of the component you would like to create 

When we create the components, they get created under /src/folder - the folder is the one we created

### how to check the current angular version using for your website or application/app?
Simply type in the terminal 
```
ng --version
```

You will now see on terminal, the version of Angular you use. 

### ways to represent a selector in component.ts declared inside decorator: 

``` 
selector: 'app-test'
selector: '.app-test'
selector: '[app-test]'
```
1. Here we can simply use this app-test in the html by calling <app-test></app-test>
2. For the 2nd one, we can use the as a class, <div class"app-test"> </div>
3. For the 3rd way, we can use it as <div app-test> </div> 


### Ways of writing a template in component
Usually we write the template in the component decorator as 
```
templateUrl: '.test/test.component.html'
```
But to write template in the direct component file is by writing it as:
```
template: '<div> Inline Template </div>'
```
Because this is one line we were able to write in single quotes, we will use back stashes for this for multiple lines to be written

```
template:`<div> Inline Template </div>`
```
same can be done to styles as well 
```
styles: ` 
div {
color: red 
}`
```
