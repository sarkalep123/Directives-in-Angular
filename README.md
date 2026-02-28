# Directives-in-Angular
this is my repo

# Directives-in-Angular
this is my repo
# App.ts
ngSwitch Use in Directives
color='black';
   changeColor(color: string){
   this.color = color;
  }

  # App.html

  <!-- <h1>*ngSwitch Directive in Angular</h1>
<br>
<br>

<button (click)="changeColor('red')">Red</button>
<button (click)="changeColor('green')">Green</button>
<button (click)="changeColor('orange')">Orange</button>
<button (click)="changeColor('aqua')">Aqua</button>
<button (click)="changeColor('pink')">Pink</button>
<button (click)="changeColor('yellow')">Yellow</button>

<br>
<br>

<div [ngSwitch]="color">
<h1 *ngSwitchCase="'red'"   style="background-color: red;">red color</h1>
<h1 *ngSwitchCase="'green'" style="background-color: green;">green color</h1>
<h1 *ngSwitchCase="'orange'"style="background-color: orange;">orange color</h1>
<h1 *ngSwitchCase="'aqua'"  style="background-color: aqua;">aqua color</h1>
<h1 *ngSwitchCase="'pink'"   style="background-color: pink;">pink color</h1>
<h1 *ngSwitchCase="'yellow'" style="background-color: yellow;">yellow color</h1>
<h1 *ngSwitchDefault >No Color Match</h1>
</div>

# NgIf 
# App.html

 <!-- <div *ngIf="login; else elseBlock">
        <a href="/">logout</a>
</div>

<ng-template #elseBlock>
    <a href="/">login</a>
</ng-template> 

 <div *ngIf="block==0">
<h1>Heading 1</h1>
</div>">

<div *ngIf="block==1">
    <h1>Heading 2</h1>

</div>
<div *ngIf="block==2">
    <h1>heading 3</h1>

</div>

<button (click)="updateBlock()">Update Block</button>
 
# App.html
 ngIf Use in Directives
   login=false
   block=0
   updateBlock(){
   this.block++;
   }


// NgFor derective in Angular Using Array and Array Object//

# App.ts

students=["anil","sunil","suresh","ramesh","mahesh"];

studentData=[
  {
  name:'anil',
  age:'24',
  email:'anil03@gmail.com'
},

{
  name:'sunil',
  age:'26',
  email:'sunil02@gmail.com'
},

{
  name:'suresh',
  age:'27',
  email:'suresh01@gmail.com'
},
{
  name:'ramesh',
  age:'24',
  email:'ramesh03@gmail.com'
},
{
  name:'ramesh',
  age:'8',
  email:'ramesh04@gmail.com'
}
]

# App.html
<ul>
    <li *ngFor="let student of students">
        {{student}}</li>
</ul>

<ul>
    <li *ngFor="let data of studentData">
        {{data.name}} - {{data.age}} - {{data.email}}
    </li>
</ul>




