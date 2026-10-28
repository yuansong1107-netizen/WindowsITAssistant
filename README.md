# Windows IT Health and Troubleshooting Assistant

A local Windows support utility that helps users review selected computer information, understand supported Windows conditions, and choose carefully bounded troubleshooting actions.

The application runs locally on the user's computer. It is not a remote-control tool and does not upload normal dashboard information to an online service.

## Features

- **Start Here** problem-oriented routes for common support situations.
- **Computer Information** for supported Windows, hardware, storage, graphics, battery, sensor, audio, and network-adapter evidence.
- **Storage and Cleanup** for drive usage, installed applications, and user-controlled uninstall routes.
- **Copy Backup** for copying a user-selected source folder to a user-selected destination while leaving the original files unchanged.
- **Network and Internet** checks, a bounded connection-stability test, and an optional Internet speed estimate.
- **Performance and Startup Apps** for bounded CPU and memory observations, running-app review, and supported startup-entry management.
- **Windows Services**, **Devices and Tests**, and **Printers** for selected Windows-reported evidence and guided next steps.
- **Browser device tests** for keyboard, mouse, speaker, microphone, and webcam, subject to user interaction and browser permission.
- **Windows Repair Centre** with a read-only repair-status check and fixed, user-approved Windows maintenance actions.

## Safety

The application does not make changes simply because a check detects attention.

- State-changing actions require an explicit user confirmation.
- Administrator actions use the standard Windows User Account Control prompt.
- The dashboard cannot send arbitrary commands to Windows.
- It does not install drivers, edit the registry, remove malware, apply broad system tweaks, or permanently reconfigure a network automatically.

Windows-reported status and short observations do not prove that every physical device, application, network, or printer function is fault-free.

## Download and run

1. Download the Windows ZIP from the latest GitHub Release.
2. Extract the complete ZIP folder.
3. Keep `WindowsITAssistant.exe` and the `_internal` folder together.
4. Run `WindowsITAssistant.exe`.
5. Wait for the local dashboard to open in the default browser.

Do not run the application directly from inside the ZIP file.

The current packaged build was validated locally on 64-bit Windows 11. Other target Windows versions should be tested before relying on them for deployment.

## Development

The application is implemented with Python, FastAPI, HTML, CSS, JavaScript, and Windows PowerShell/CIM/PnP evidence sources. It is packaged as a PyInstaller one-folder application.

Current controlled regression result: **505/505 tests passed**.

## Important limitations

This project is intended as a local first-line support utility. It does not replace IT support, hardware repair, professional malware removal, enterprise device management, remote support, or a complete Windows recovery strategy.

## Third-party notices

The packaged application includes the local LibreHardwareMonitor component. Its license and third-party notices are retained under `app/vendor/librehardwaremonitor/`.
