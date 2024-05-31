Understanding MVC Core as Beginner

_Layout.cshtml :-
<ul>
  <li>Contain in Shared Folder. This File is Same Like Master Page in WebForms</li>
</ul>
<a href="https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/adding-controller?view=aspnetcore-8.0&tabs=visual-studio"> Controller.cs</a> :- 
<ul>
  <li>Calling Any Function With <code>IActionResult</code> Method.</li>
  <li>
    For Example -
      _Layout.cshtml Code Snippet -> 
      <code>&lta asp-controller="Home" asp-action="Foo"> Foo Text &lt/a></code>
      HomeController.cs Code Snippet -> <code> public IActionResult About() { return View();  } </code>
      This Defining That We Use Foo Method of HomeController
  </li>
</ul>
<a href="https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/adding-model?view=aspnetcore-8.0&tabs=visual-studio"> Model</a> :- 
  <ul>
    <li>Add New Model File With Visual Studio -> <code>Right-click the Models folder > Click Add > Click Class > Name the file ModelName.cs</code> </li>
    <li>Same as Prop We Made in WebForms. We Can Use Model Directly in View Page With Help of Razor Page Using @ModelName</li>
  </ul>
