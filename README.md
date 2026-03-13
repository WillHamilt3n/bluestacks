# BlueStacks Application

A WPF-based Windows application built with .NET 6 that appears to be related to BlueStacks functionality.

## Features

- **WPF User Interface**: Modern Windows Presentation Foundation application
- **Custom Controls**: Custom button controls and styling
- **Database Integration**: Uses Entity Framework Core with SQLite
- **Network Interception**: Includes network interception capabilities with WindivertDotnet
- **Service Management**: System service interaction capabilities
- **Bungie API Integration**: Includes DotNetBungieAPI for gaming-related functionality
- **Visual Effects**: Snow effects and custom visual styling
- **Data Visualization**: OxyPlot integration for charts and graphs
- **System Tray**: NotifyIcon support for system tray functionality
- **File Compression**: SharpCompress for archive handling

## Technology Stack

- **.NET 6**: Target framework with Windows-specific features
- **WPF (Windows Presentation Foundation)**: UI framework
- **Entity Framework Core**: Database ORM with SQLite provider
- **WindivertDotnet**: Network packet interception
- **OxyPlot**: Data visualization and charting
- **DotNetBungieAPI**: Bungie.net API integration
- **SharpCompress**: Archive/compression handling

## Project Structure

```
bluestacks/
├── Database/           # Database-related files and models
├── Interception/       # Network interception functionality
├── Models/             # Data models and entities
├── Utility/            # Utility classes and helpers
├── Windows/            # WPF windows, controls, and assets
│   ├── Assets/         # Images, fonts, icons, and resources
│   ├── Controls/       # Custom WPF controls
│   └── Converters/     # Value converters and effects
├── bin/                # Build output (ignored in git)
├── obj/                # Build intermediates (ignored in git)
└── .vs/                # Visual Studio files (ignored in git)
```

## Key Files

- **App.xaml**: Application resources, styles, and startup configuration
- **bluestacks.csproj**: Project file with dependencies and build settings
- **GlobalXamlCatcher.cs**: Global XAML event handling
- **LoginDebugHandler.cs**: Login debugging functionality
- **LoginFlowDebugger.cs**: Login flow debugging and analysis

## Prerequisites

- Windows 10/11
- .NET 6.0 Runtime
- Visual Studio 2022 (for development)

## Building the Project

1. Open the solution in Visual Studio 2022
2. Restore NuGet packages
3. Build the solution (Ctrl+Shift+B)
4. Run the application (F5)

### Command Line Build

```bash
dotnet restore
dotnet build
dotnet run
```

## Dependencies

This project uses several NuGet packages:

- `DotNetBungieAPI` (2.12.1) - Bungie.net API client
- `Hardcodet.NotifyIcon.Wpf` (1.1.0) - System tray notifications
- `MathConverter` (2.2.1-preview) - XAML math conversions
- `Microsoft.EntityFrameworkCore.Sqlite` (7.0.2) - SQLite database support
- `OxyPlot.Wpf` (2.1.2) - Data visualization
- `SharpCompress` (0.36.0) - Archive handling
- `System.Management` (7.0.0) - Windows management APIs
- `System.ServiceProcess.ServiceController` (8.0.0) - Windows service control
- `WindivertDotnet` (1.1.2) - Network packet interception

## Configuration

The application uses:
- SQLite database for data storage
- Custom fonts (KantumruyPro-Regular.ttf)
- Application manifest for Windows compatibility
- Custom icon (appLogo.ico)

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## License

Please specify the license for this project.

## Notes

- This application requires administrative privileges for network interception features
- The project includes debugging tools for login flows
- Database migrations may be required on first run
- Some features may require specific Windows permissions

## Support

For issues and questions, please use the GitHub Issues section.