# IIS configuration

TODO: ...

- Enable "Application Initialization" (under Web Server (IIS) / Web Server / Application Development)

- Turn off app pool recycling
- App pool - advanced settings - Start Automatically - true (is the default but below won't work without it)
- App pool - advanced settings - Start mode: AlwaysRunning
- App pool - advanced settings - Iddle Time-out: 0
- Site - advanced settings - Preload enabled: true 
- ~~Disable dynamic compression (??)~~ - done in web.config