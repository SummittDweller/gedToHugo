# gedToHugo
My take on a gedcom-to-Hugo static site builder, based on tektsu/gedcom2hugo 

`main.go` is just what it implies, the "main" trunk of the project.   Note that in order to compile with the latest dependencies, the one change I had to make here was casting all `cli.BoolFlag` and `cli.StringFlag` references as pointers, so they became `&cli.BoolFlag` and `&cli.StringFlag`.  

I built this project using JetBrains' GoLang IDE.  In order to make breakpoints and debugging work in the module code the project had to be built not as a "Go" application, but as a "Go Modules" application.