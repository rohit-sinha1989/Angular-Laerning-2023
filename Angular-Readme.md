[### Angular Questions and Answers

# **1. What is SPA? How it is different from server-side rendering and what are the pros and cons of SPA?**
    SPA - It means that we don't have anything on the backend but just client JavaScript.This client JavaScript is being loaded inside the client browser and is executed and then everything is rendered on screen just with the help of JavaScript.
    Single page applications are web based applications that only need to be loaded once, with new functionality consisting of only minor changes to the user interface. It does not load new HTML pages to display the content of the new page, but rather generates it dynamically. This is made feasible by JavaScript's ability to alter DOM components on the current page. A Single Page Application method is speedier, resulting in a more consistent user experience.


  # Sharing Data between components

     4 Methods to Share Data between Components in Angular
     Method 1: Parent to Child via @Input decorator.
     Method 2: Child to Parent via @Output decorator and EventEmitter.
     Method 3: Child to Parent via @ViewChild decorator.
     Method 4: Unrelated Components via a Service.

      https://www.samarpaninfotech.com/blog/methods-to-share-data-between-angular-components/

     Method 1: Parent to Child via @Input decorator.
                Let’s assume, you have one component, where you have some data and you want to supply that data to the child component, How it possible ??? Answer is @input. So what is @Input?? @Input is a decorator which allows you to accept the input from the parent component. Input can be imported from @angular/core.

    Method 2: Child to Parent via @Output decorator and EventEmitter
                If you want to pass data from the child component to the parent component use @Output() and EventEmitter.

                First, let us discuss what is @Output and EventEmitter, @Output is a component decorator which becomes the output for the parent component and EventEmitter is something that has the capability to propagate the event from the child component to the parent component.

                To pass data from the child to the parent, you have to emit it from the child. The parent will be listening for the event will grab the data.

    Method 3: Child to Parent via @ViewChild decorator
                Here as we know we have @output and event emitter to share the data from child to parent component, so why @Viewchild is needed ? hold on it is needed because it gives extra control to parent component to access the child events.

                Here we are just understanding by passing the data from child to parent by using @Viewchild decorator, Let’s see.



     
  # What is the difference between @ViewChild() and @ViewChildren()
           https://www.pluralsight.com/guides/querying-the-dom-with-@viewchild-and-@viewchildren


  # What ways of binding in Angular?
              One-way Binding
              Two-Way Binding

 # What is service in Angular?
                
    1. Services in Angular are simply typescript classes with the @injectible decorator. This decorator tells angular that the           class is a service and can be injected into components that need that service. They can also inject other services as             dependencies. 
    2. As mentioned earlier, these services are used to share a single piece of code across multiple components. These services are used to hold business logic. Services are used to interact with the backend. For example, if you wish to make AJAX calls, you can have the methods to those calls in the service and use it as a dependency in files.
    In angular, the components are singletons, meaning that only one instance of a service that gets created, and the same            instance is used by every building block in the application. 
    A service can be registered as a part of the module, or as a part of the component. To register it as a part of the               component, you’ll have to specify it in the providers’ array of the module.

# What is AOT (Ahead-Of-Time) Compilation?
           The Angular Ahead-of-Time compiler pre-compiles application components and their templates during the build process.              Apps compiled with AOT launch faster for several reasons.
          Templates are embedded as code within their components so there is no client-side request for template files.
            At the end of the restore view phase of the JSF request lifecycle, Seam attempts to restore any previous long-running         conversation context. If none exists, Seam creates a new temporary conversation context.
        Application components execute immediately, without client-side compilation
        The compiler discards unused Angular directives that a tree-shaking tool can then exclude

  
# What is ViewEncapsulation and how many ways are there do to do it in Angular?
      To put simply, ViewEncapsulation determines whether the styles defined in a particular component will affect the entire application or not. Angular supports 3 types of ViewEncapsulation:
      Emulated : Styles used in other HTML spread to the component
      Native : Styles used in other HTML doesn’t spread to the component
      None : Styles defined in a component are visible to all components of the application


# What is AOT Compilation?
    Angular AOT contains mainly of components and their HTML templates.The components and templates are provided by the angular requires a compilation process before it can run in browser.AOT helps in converting Angular HTML and TypeScript code in to efficient JavaScript code while building phase before the browser downloads and runs the code.
    Here are some reasons you might want to use AOT:
    Faster rendering
    Fewer asynchronous requests
    Smaller Angular framework download size
    Detect template errors earlier
    Better security

