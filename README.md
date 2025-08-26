# NumberToWords

Overview

Number to Words Converter is a lightweight ASP.NET Core MVC web application that converts numerical currency values into their English word equivalents (e.g., 1234.56 → One Thousand Two Hundred Thirty-Four Dollars and Fifty-Six Cents). It includes both manual input and quick test case buttons.

🚀 Features

Convert numbers (up to millions) into words

Supports decimal to cent conversion

Quick test case buttons for demo/testing

Responsive, user-friendly UI (Bootstrap 5)

CSRF-protected POST requests

🧰 Technologies Used

ASP.NET Core MVC (v6 or later)

C#

Razor Views

Bootstrap 5 (for styling)

Visual Studio or VS Code

📁 Folder Structure
NumberToInteger/
├── Controllers/
│   └── HomeController.cs
├── Models/
│   └── ErrorViewModel.cs
├── Views/
│   ├── Home/
│   │   └── Index.cshtml
│   └── Shared/
│       └── _Layout.cshtml
├── wwwroot/
│   └── css/, js/, lib/
├── Program.cs
├── Startup.cs or builder config
└── README.md

🛠️ How to Build and Run the App
✅ Prerequisites

.NET SDK 6.0 or later

Visual Studio 2022+
 or Visual Studio Code

Git (optional)

🔧 Steps to Build & Run Locally

Clone the repository

git clone https://github.com/yourusername/NumberToInteger.git
cd NumberToInteger


Open the project

In Visual Studio: Open NumberToInteger.sln

In VS Code: Open the folder using File > Open Folder

Run the project

In Visual Studio: Press F5 or click Start Debugging

In terminal:

dotnet run


Visit the app in your browser

Navigate to: https://localhost:5001 or http://localhost:5000

🌐 How to Use the App

Enter a number in the input field (e.g., 987.65)

Click the "Convert" button

View the converted text in the result area

Optionally, click one of the Quick Test Case buttons (like 1234.56) to instantly see the result

🧪 Test Cases
Input	Output
1234.56	One Thousand Two Hundred Thirty-Four Dollars and Fifty-Six Cents
1000000	One Million Dollars
0.99	Ninety-Nine Cents
0	Zero Dollars
🛡️ Security Notes

Uses default ASP.NET Core anti-forgery tokens (@Html.AntiForgeryToken()).

No input is stored; it's a transient, stateless converter.

📦 Publish and Host

To publish and host on IIS, Azure, or Docker:

dotnet publish -c Release -o ./publish


Deploy contents of ./publish to your host (IIS / Azure App Service / Linux container).

For IIS, make sure to configure the application pool to use .NET CLR Version: No Managed Code.

💡 Future Enhancements

Support for different currencies (e.g., INR, EUR)

Localization (multi-language output)

Voice output of the result

Real-time JavaScript conversion

🧑‍💻 Author

Contact: nerdene48@gmail.com

📝 License

This project is open-source. You can use it for personal or commercial projects.
Include a proper license file like MIT or Apache 2.0 if required.
