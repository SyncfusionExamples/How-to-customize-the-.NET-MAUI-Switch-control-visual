# How-to-customize-the-.NET-MAUI-Switch-control-visual

In this article, you can learn about how to customize the [.NET MAUI Switch](https://www.syncfusion.com/maui-controls/maui-switch) control's visuals, like Cupertino and Fluent themes. This customization is done using the [SwitchSettings](https://help.syncfusion.com/cr/maui/Syncfusion.Maui.Buttons.SwitchSettings.html?tabs=tabid-1#Syncfusion_Maui_Buttons_SwitchSettings_TrackBackground) property within the `VisualStateManager`. Below is an example of how to implement these styles in XAML.

**XAML**

```
 <ContentPage.Resources>
     <ResourceDictionary>
         <Style x:Key="FluentStyle" TargetType="syncfusion:SfSwitch">
             <Setter Property="VisualStateManager.VisualStateGroups">
                 <Setter.Value>
                     <VisualStateGroupList>
                         <VisualStateGroup x:Name="CommonStates">
                             <VisualState x:Name="Off">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="#A19F9D"
                                                 ThumbCornerRadius="6"
                                                 ThumbHeightRequest="11"
                                                 ThumbStroke="#A19F9D"
                                                 ThumbWidthRequest="11"
                                                 TrackBackground="Transparent"
                                                 TrackHeightRequest="19"
                                                 TrackStroke="#A19F9D"
                                                 ThumbStrokeThickness="1"
                                                 TrackStrokeThickness="1"
                                                 TrackWidthRequest="39" />
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="OffPressed">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="#A19F9D"
                                                 ThumbCornerRadius="7"
                                                 ThumbHeightRequest="13"
                                                 ThumbStroke="#A19F9D"
                                                 ThumbWidthRequest="13"
                                                 TrackBackground="Transparent"
                                                 TrackHeightRequest="19"
                                                 TrackStroke="#A19F9D"
                                                 ThumbStrokeThickness="1"
                                                 TrackStrokeThickness="1"
                                                 TrackWidthRequest="39" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="OffHovered">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="#A19F9D"
                                                 ThumbCornerRadius="7"
                                                 ThumbHeightRequest="13"
                                                 ThumbStroke="#A19F9D"
                                                 ThumbWidthRequest="13"
                                                 TrackBackground="Transparent"
                                                 TrackHeightRequest="19"
                                                 TrackStroke="#A19F9D"
                                                 ThumbStrokeThickness="1"
                                                 TrackStrokeThickness="1"
                                                 TrackWidthRequest="39" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="On">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="#1B1A19"
                                                 ThumbCornerRadius="6"
                                                 ThumbHeightRequest="11"
                                                 ThumbStroke="#1B1A19"
                                                 ThumbWidthRequest="11"
                                                 TrackBackground="#0078D4"
                                                 TrackHeightRequest="19"
                                                 TrackStroke="#0078D4"
                                                 ThumbStrokeThickness="1"
                                                 TrackStrokeThickness="1"
                                                 TrackWidthRequest="39" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="OnPressed">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="#1B1A19"
                                                 ThumbCornerRadius="7"
                                                 ThumbHeightRequest="13"
                                                 ThumbStroke="#1B1A19"
                                                 ThumbWidthRequest="13"
                                                 TrackBackground="#0078D4"
                                                 TrackHeightRequest="19"
                                                 TrackStroke="#0078D4"
                                                 ThumbStrokeThickness="1"
                                                 TrackStrokeThickness="1"
                                                 TrackWidthRequest="39" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="OnHovered">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                  ThumbBackground="#1B1A19"
                                                  ThumbCornerRadius="7"
                                                  ThumbHeightRequest="13"
                                                  ThumbStroke="#1B1A19"
                                                  ThumbWidthRequest="13"
                                                  TrackBackground="#0078D4"
                                                  TrackHeightRequest="19"
                                                  TrackStroke="#0078D4"
                                                  ThumbStrokeThickness="1"
                                                  TrackStrokeThickness="1"
                                                  TrackWidthRequest="39" />  
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                         </VisualStateGroup>
                     </VisualStateGroupList>
                 </Setter.Value>
             </Setter>
         </Style>

         <Style x:Key="CupertinoStyle" TargetType="syncfusion:SfSwitch">
             <Setter Property="VisualStateManager.VisualStateGroups">
                 <Setter.Value>
                     <VisualStateGroupList>
                         <VisualStateGroup x:Name="CommonStates">
                             <VisualState x:Name="On">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="White"
                                                 ThumbCornerRadius="15"
                                                 ThumbHeightRequest="26"
                                                 ThumbStroke="White"
                                                 ThumbStrokeThickness="1"
                                                 ThumbWidthRequest="26"
                                                 TrackBackground="#0078D4"
                                                 TrackHeightRequest="28"
                                                 TrackStroke="#0078D4"
                                                 TrackStrokeThickness="1.5"
                                                 TrackWidthRequest="48" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                             <VisualState x:Name="Off">
                                 <VisualState.Setters>
                                     <Setter Property="SwitchSettings">
                                         <Setter.Value>
                                             <syncfusion:SwitchSettings
                                                 ThumbBackground="White"
                                                 ThumbCornerRadius="15"
                                                 ThumbHeightRequest="26"
                                                 ThumbStroke="White"
                                                 ThumbStrokeThickness="1"
                                                 ThumbWidthRequest="26"
                                                 TrackBackground="#39393D"
                                                 TrackHeightRequest="28"
                                                 TrackStroke="#39393D"
                                                 TrackStrokeThickness="1.5"
                                                 TrackWidthRequest="48" />   
                                         </Setter.Value>
                                     </Setter>
                                 </VisualState.Setters>
                             </VisualState>
                         </VisualStateGroup>
                     </VisualStateGroupList>
                 </Setter.Value>
             </Setter>
         </Style>

     </ResourceDictionary>
 </ContentPage.Resources>

 <VerticalStackLayout
     x:Name="mainStack"
     VerticalOptions="Center"
     HorizontalOptions="Center"
     WidthRequest="350">
     ...
     <Grid Margin="0,10,10,10"
          HeightRequest="75">
         ...
         <syncfusion:SfSwitch
             Grid.Row="0"
             Grid.Column="0"
             AllowIndeterminateState="False"
             IsOn="True"/>
         <syncfusion:SfSwitch
             Grid.Row="0"
             Grid.Column="1"
             AllowIndeterminateState="False"
             IsOn="True"
             Style="{StaticResource CupertinoStyle}" />
         <syncfusion:SfSwitch
             Grid.Row="0"
             Grid.Column="2"
             AllowIndeterminateState="False"
             IsOn="True"
             Style="{StaticResource FluentStyle}" />
         ...
     </Grid>
 </VerticalStackLayout>
```

By utilizing the `SwitchSettings` property and defining different visual states, the .NET MAUI Switch control can be customized to fit various design requirements. This allows for a more tailored user experience in applications.