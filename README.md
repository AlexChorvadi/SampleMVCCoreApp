Understanding <a href="https://learn.microsoft.com/en-us/aspnet/core/mvc/overview?view=aspnetcore-8.0">MVC</a> Core Concept as Beginner 

<ul>
  <li>
    <a href="https://learn.microsoft.com/en-us/aspnet/core/mvc/views/layout?view=aspnetcore-8.0">_Layout.cshtml</a> :-
    <ul>
      <li>Contain in Shared Folder. This File is Same Like Master Page in WebForms</li>
    </ul>
  </li>
  <li>
    <a href="https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/adding-controller?view=aspnetcore-8.0&tabs=visual-studio"> Controller.cs</a> :- 
    <ul>
      <li>Calling Any Function With <code>IActionResult</code> Method.</li>
      <li>For Example -
          _Layout.cshtml Code Snippet -> 
          <code>&lta asp-controller="Home" asp-action="Foo"> Foo Text &lt/a></code><br/>
          HomeController.cs Code Snippet -> <code>public IActionResult Foo() { return View();  }</code>
          This Defining That We Use Foo Method of HomeController
      </li>
    </ul>
  </li>
  <li>
    <a href="https://learn.microsoft.com/en-us/aspnet/core/tutorials/first-mvc-app/adding-model?view=aspnetcore-8.0&tabs=visual-studio"> Model</a> :- 
      <ul>
        <li>Add New Model File With Visual Studio -> <code>Right-click the Models folder > Click Add > Click Class > Name the file ModelName.cs</code> </li>
        <li>Same as Prop We Made in WebForms. We Can Use Model Directly in View Page With Help of Razor Page Using @ModelName</li>
      </ul>
  </li>
  <li>
    <h5>Add <code>Model</code> In View Page <code>ViewPageName.cshtml</code></h5>
    <ul>
      <li> Top of the Page Add <code>@model ModelName</code> </li>
      <li> For Storing Value in Model We Use <code>asp-for</code> attribute in Element
        <br/>For Example : <code>&ltinput type="text" asp-for="FirstName" id="FirstName"></code>
      </li>
      <li><code>asp-for</code> Only Works When we add <code>Model</code> into our View page as per First Point</li>
    </ul>
  </li>
</ul>
