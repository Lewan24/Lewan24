### Hi there 👋

<a href="https://app.daily.dev/lewan24"><img src="https://api.daily.dev/devcards/v2/ywbscmuGK2cKD10GdKSlJ.png?r=41o&type=wide" width="652" alt="Artur Lewandowski's Dev Card"/></a><br><br>

Some information about me as person and my activity on Github and .NET Career coded in C# language :)

```c#
// .NET 7 C#

var Artur = new Developer();

// Initialize developer's properties
Artur.Name = "Artur";
Artur.Age = 22;
Artur.Job = "Backend Developer";
Artur.Known_Languages = new() {
  "C#",
  "C++",
  "Blazor",
  ".NET MVC",
  "WebApis",
  "Python",
  "Java",
  "PHP",
  "MySQL",
  "JS"
};

// Data is stored in Developer class below
#region Get Information about developer

Artur.GetMainPersonInformation();
Artur.GetJobInformation();
Artur.GetEducationCareerInformation();

#endregion

Console.ReadKey();

public sealed class Developer
{
    #region Variables
    private string? _name;
    public string? Name { get => _name; set { _name = value; } }

    private string? _job;
    public string? Job { get => _job; set { _job = value; } }

    private List<string> _languages = new();
    public List<string> Known_Languages { get => _languages; set { _languages = value; } }

    private short _age = 0;
    public short Age { get => _age; set { _age = value; } }
    #endregion

    #region Public Get Information Section
    public void GetMainPersonInformation()
    {
        Console.WriteLine($"\t\t\t---- {_name}, {_age} - {_job} ----\n\n");

        Console.WriteLine(@"----- Activity -----
    Creating projects/schemes for portfolio, own educational purpose. 
I upload here also the solutions for problems that on internet are just too old or doesn't work for me." + "\n\n");

        Console.WriteLine(@"----- Licensing -----
    Almost everything that I create is on MIT licence so free to use for everyone if needed." + "\n\n");
    }

    public void GetJobInformation()
    {
        Console.WriteLine(@"----- Job -----
    For now .NET Developer mainly focused on web applications based on Blazor / .net mvc.
Currently I use the newest version of .NET for creating applications (.NET 7)" + "\n\n");
    }

    public void GetEducationCareerInformation()
    {
        Console.WriteLine(@"----- Education / Career -----
    I learn by creating own projects and solving own problems in work. 
I read programming books about .NET or the style of beeing the developer. 
And also I watch tutorials on yt or by buying on Udemy.

For future I want to learn some frontend languages such as 
Angular or React. Also I want to start T - SQL learning.");
    }
    #endregion
}
```
