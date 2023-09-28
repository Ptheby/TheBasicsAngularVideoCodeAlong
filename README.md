# TheBasicsAngularVideoCodeAlong
Coding along with the basics video playlist for angular course. 
The Basics Videos
Video 1- Module Introduction- no info really
Video 2- How an Angular App gets Loaded and Started
It all starts at the main.ts file where we use bootstrap to pass appModule as an argument like this   bootstrap(appModule) which the appModule is also listed as an Import on that same main.ts file. The appModule argument tells Angular to look at the app.module.ts, where the bootstrap has AppComponent and AppComponent is listed as an import there, this directs it to look at the app components , possible the css, html, ts. Maybe it looks at the app. component. ts first and sees the setup for the selector property of the @Component with 'app-root' as a value. now the index.html file with app-root in the body can pass along the app.component.html file which is what displays!

Video 3-Components are Important
Components are key feature in Angular. You build your whole applicaiton by composing it from components, which you create on your own. You start with the app/root component. We nest or add our other components to this app/root.
Angular apps are built from different components, each component has it's own template, html, maybe styling, and business logic. So you can easily reuse different parts without having to scrunch all the html/styling/script into one page. easier to change, update, exchange, and reuse this way. 

Video-4 - Creating a New Component
In this video we created our own component called server. WE did this by creating a new folder in the "app" folder. we nnamed this folder "server" in this folder we created first, the new server.component.ts file where we first:
Import { Component} from angular with "from '@angular/core'; then we use the component decorator @Component and use the selecotr to pick "app-server", and then  another importnat part is picking the "templateUrl: and this is a file we create as a template which is an html file: server.component.html for this component.  NExt we export class ServerComponent {   so that it can be used elsewhere. Then in order to use it, we must go then to the app.module.ts where he shows us how to use it in the next video. 

Video 5- Understanding the Role of AppModule and Component Declaration
Angular uses components to build webpages and modules to package them together to use. Bundling functionalities of our apps and gives Angular the information on which features to have and use. It;s also an empty Typsecript class we can transform into someting else by using a decorator, the @NgModule decorator which is also imported from @angular/core.  We need to tell angular that the new server.component exists, we do that by registering it with the @NgModule under the declarations as ServerComponent, which we named. Now it knows it exists but that is not enough, typescript wouldnt know where to find it. so we have to use an Import at the top of the app.module.ts file  we are already in with: import { ServerComponent} from './server/server.component';



































