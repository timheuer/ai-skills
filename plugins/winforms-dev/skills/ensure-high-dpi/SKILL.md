--- 
name: ensure-high-dpi
description: 'Expert to help ensure high DPI settings in WinForms applications. USE WHEN: You want to make sure your WinForms application is optimized for high DPI displays, providing a better user experience on modern screens. DO NOT USE WHEN: You are working on a non-WinForms application or do not need to optimize for high DPI settings.'
---

Look at the code of the WinForms application running the winforms-specialist agent as a #subAgent and identify areas where high DPI settings can be applied. Provide recommendations on how to implement high DPI support, such as using appropriate scaling techniques, setting the AutoScaleMode property, and ensuring that images and controls are designed to scale properly on high DPI displays.

To ensure high DPI settings in your WinForms application, you can follow these recommendations:

1. Set the AutoScaleMode property: In your form's constructor, set the AutoScaleMode property to Dpi. This will enable automatic scaling of controls based on the DPI settings of the display.

```csharp
public MyForm()
{
    InitializeComponent();
    this.AutoScaleMode = AutoScaleMode.Dpi;
}
```