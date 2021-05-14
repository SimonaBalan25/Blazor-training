                                                                                                                                                             AUTHENTICATION & AUTHORIZATION

Microsoft.AspNetCore.Components.WebAssembly.Authentication + Microsoft.AspNetCore.Components.Authorization packages (Blazor WebAssembly)


In Blazor Web Assembly, authentication is done using custom AuthenticationStateProvider and mechanism for secure web assembly on .net 


In Blazor Server, authentication is done based on SignalR, right after the connection with it is done and corresponds to general mechanism in .net core that secure .net apps 

Set the Authentication in action:
<Router AppAssembly="@typeof(Program).Assembly">
<Found Context="routeData">
<AuthorizeRouteView RouteData="@routeData" DefaultLayout="@typeof(MainLayout)" />
</Found>
<NotFound>
<LayoutView Layout="@typeof(MainLayout)">
<CustomNotFound />
</LayoutView>
</NotFound>
</Router>




….



    





