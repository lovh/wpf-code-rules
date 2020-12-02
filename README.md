# wpfcoderules

## Get Started
## Overview
1. Property
2. Region
## Property Code Styles

### Property
```csharp
public string Email { get; set; }
```

### Get Set Property
```csharp
private string _email;
public string Email 
{ 
    get { return _email; } 
    set { _email = value; } 
}
```
Be sure to name the `private` access restrictor for the variable.
### Observable Property
```csharp
private string _email;
public string Email 
{ 
    get { return _email; } 
    set { _email = value; OnPropertyChanged(); } 
}
```
~base.OnPropertyChanged();~   
*Do not recommended to use `.base` for prefixes.*

### Property with method in setter
```csharp
private string _email;
public string Email 
{ 
    get { return _email; } 
    set { _email = value; Something(); OnPropertyChanged(); } 
}
```

## Region

### Region: Property
```csharp
#region Email

private string _email;
public string Email
{
    get { return _email; }
    set { _email = value; OnPropertyChanged(); }
}
#endregion
```

## 89. Resource Name

* Style
  - Button : BTN
  - TextBlock : TXB
  - TreeView : TRV
  - TreeViewItem : TRVI
  - ListBox : LBX
  - ListBoxItem : LBXI

## 99. References
### Markdown
[Temp Link](https://docs.microsoft.com/en-us/windows/communitytoolkit/parsers/markdownparser)
