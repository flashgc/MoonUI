MoonUI
======

Milk-blue style for WPF controls (.NET 4.0)

======
USAGE
======
There are some ways to use it.

* Copy Theme/MoonUICore.xaml to your Application. Add dictionary right in your app.xaml file (this way used in example):

```csharp
<Application.Resources>
		<!-- Resources scoped at the Application level should be defined here. -->
		<ResourceDictionary>
			<ResourceDictionary.MergedDictionaries>
				<ResourceDictionary Source="Theme/MoonUICore.xaml"/>
			</ResourceDictionary.MergedDictionaries>
		</ResourceDictionary>
</Application.Resources>
```
* Copy Theme/MoonUICore.xaml to your Application. Add reference in your code:
```csharp
this.Resources.MergedDictionaries.Add(new ResourceDictionary() { Source = new Uri("Theme/MoonUICore.xaml.xaml", UriKind.RelativeOrAbsolute) });
```
* Compile sample project. Add reference in your application to compiled sample program. Add reference in your code:
```csharp
this.Resources.MergedDictionaries.Add(new ResourceDictionary() { Source = new Uri("/MoonUI_Net4;component/Theme/MoonUICore.xaml.xaml", UriKind.RelativeOrAbsolute) });
```
==========
Notes
==========

There are some problems in wpf designer (VS2010) using first way, but it compiles without any problems. You can try to work in VS2012 or to use 2nd/3rd method.

Also there is a lot of crap code because of using only Blend to create it, but style is already usable. Later it shall be refactored.


----
sorry for my english =)