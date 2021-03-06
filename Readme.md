<!-- default file list -->
*Files to look at*:

* [Form1.cs](./CS/StandaloneCustForm/Form1.cs) (VB: [Form1.vb](./VB/StandaloneCustForm/Form1.vb))
<!-- default file list end -->
# How to display the Customization Form near the PivotGridControl


This example demonstrates how to display the Customization Form near the PivotGridControl.

When displayed, the form is located in the [SplitContainerControl](https://docs.devexpress.com/WindowsForms/DevExpress.XtraEditors.SplitContainerControl) - a parent container for the PivotGridControl and Customization Form. To specify the SplitContainer's panel as the Customization Form's owner, handle the  [PivotGridControl.ShowingCustomizationForm](https://docs.devexpress.com/WindowsForms/DevExpress.XtraPivotGrid.PivotGridControl.ShowingCustomizationForm) event and use the [CustomizationFormShowingEventArgs.ParentControl](https://docs.devexpress.com/WindowsForms/DevExpress.XtraPivotGrid.CustomizationFormShowingEventArgs.ParentControl) property. 

The form's appearance is specified with the [PivotGridOptionsCustomization.CustomizationFormStyle](https://docs.devexpress.com/CoreLibraries/DevExpress.XtraPivotGrid.PivotGridOptionsCustomization.CustomizationFormStyle) property.

Call the [PivotGridControl.FieldsCustomization](https://docs.devexpress.com/WindowsForms/DevExpress.XtraPivotGrid.PivotGridControl.FieldsCustomization.overloads) method to show the form.

![screenshot](https://github.com/DevExpress-Examples/how-to-display-the-customization-form-near-the-pivotgridcontrol-e4572/blob/18.2.4%2B/images/screenshot.png)
