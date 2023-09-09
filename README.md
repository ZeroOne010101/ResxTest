# ResxTest

### Issue

I am trying to localize another avalonia project, but i cannot get .resx files to work properly. This is a minimal example to demonstrate the error.

### Error

Unable to resolve Greeting as static field, property, constant or enum value Line 16, position 14.	ResxTest	C:\Users\ZeroOne\Documents\Programming\ResxTest\ResxTest\Views\MainView.axaml	16	

### Relevant Sections:

App.axaml.cs, ln 20

```Assets.i18n.Resources.Culture = new CultureInfo("en-US");```

MainView.axaml, ln 6

```xmlns:i18n="clr-namespace:ResxTest.Assets.i18n"```

MainView.axaml, ln 16

```<TextBlock Text="{x:Static i18n:Resources.Greeting}" HorizontalAlignment="Center" VerticalAlignment="Center"/>```

Assets/i18n/Resources.resx

```Entire File```
