# How to show WebView in Xamarin.Forms Accordion (SfAccordion) 

You can show the [WebView](https://docs.microsoft.com/en-us/xamarin/xamarin-forms/user-interface/webview?tabs=macos) in [Accordion](https://help.syncfusion.com/xamarin/accordion/getting-started?) by setting the WebView height in Xamarin.Forms.

You can also refer the following article.

https://www.syncfusion.com/kb/11373/how-to-show-webview-in-xamarin-forms-accordion-sfaccordion 

``` xml
<syncfusion:SfAccordion ExpandMode="SingleOrNone">
    <syncfusion:SfAccordion.Items>
        <syncfusion:AccordionItem>
            <syncfusion:AccordionItem.Header>
                <Grid>
                    <Label TextColor="#495F6E" Text="Xamarin" Margin="5" HeightRequest="50" VerticalTextAlignment="Center"/>
                </Grid>
            </syncfusion:AccordionItem.Header>
            <syncfusion:AccordionItem.Content>
                <StackLayout Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                    <WebView HeightRequest="250" VerticalOptions="FillAndExpand" HorizontalOptions="FillAndExpand" Source="http://xamarin.com" />
                </StackLayout>
            </syncfusion:AccordionItem.Content>
        </syncfusion:AccordionItem>
        <syncfusion:AccordionItem>
            <syncfusion:AccordionItem.Header>
                <Grid>
                    <Label TextColor="#495F6E" Text="Microsoft" Margin="5" HeightRequest="50" VerticalTextAlignment="Center"/>
                </Grid>
            </syncfusion:AccordionItem.Header>
            <syncfusion:AccordionItem.Content>
                <StackLayout Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                    <WebView HeightRequest="250" VerticalOptions="FillAndExpand" HorizontalOptions="FillAndExpand" Source="https://www.microsoft.com/en-in" />
                </StackLayout>
            </syncfusion:AccordionItem.Content>
        </syncfusion:AccordionItem>
        <syncfusion:AccordionItem>
            <syncfusion:AccordionItem.Header>
                <Grid>
                    <Label TextColor="#495F6E" Text="Syncfusion" Margin="5" HeightRequest="50" VerticalTextAlignment="Center"/>
                </Grid>
            </syncfusion:AccordionItem.Header>
            <syncfusion:AccordionItem.Content>
                <StackLayout Padding="10,10,10,10" BackgroundColor="#FFFFFF">
                    <WebView HeightRequest="250" VerticalOptions="FillAndExpand" HorizontalOptions="FillAndExpand" Source="https://www.syncfusion.com/" />
                </StackLayout>
            </syncfusion:AccordionItem.Content>
        </syncfusion:AccordionItem>
    </syncfusion:SfAccordion.Items>
</syncfusion:SfAccordion>
```

**Output**

![WebViewInAccordion](https://github.com/SyncfusionExamples/webview-in-accordion-xamarin/blob/master/ScreenShots/WebViewInAccordion.png)
