# SCICHART LICENSING TEST APP 

This is a troubleshooting application for applying licenses to SciChart WPF Charts in both WPF applications and WinForms. 

For more information, see the [SciChart Licensing Troubleshooting](https://www.scichart.com/scichart-licensing-troubleshooting/) page. 


### Steps to Troubleshoot Licenses
 
 1. Download this Licensing Test App and unzip it to your computer.
 2. Enter your Runtime License key from your Profile page at [www.scichart.com/profile](https://www.scichart.com/profile/) in App.xaml.cs & compile the Licensing Test App
 3. Run the Licensing Test App on the other computer where you are experiencing problems. Make sure this is a computer without an activated developer license. This is because the Activated Developer license will interfere with this test.
		- **Expected Result:** You should not see a ‘Powered by SciChart’ watermark or a trial expired when running the Licensing Test App.
		- If you do, contact us, you’ve probably found a bug 🙂
 4. Debug the Licensing Test App on another computer.Make sure this is a computer without an activated developer license. This is because the Activated Developer license will interfere with this test.
		- **Expected Result:** You should see a ‘Powered by SciChart’ watermark or a trial expired notice.
		- This is expected behaviour as SciChart has detected you are running inside Visual Studio and is searching for a developer license.
		
If either expectation above fails, please contact tech support and we will be glad to assist. Please tell us what you tried, and what version of SciChart you are using.

If the expectations above pass, it is likely that the Runtime key has been set incorrectly in your main application. Please double check you have set the Runtime Key once and once only in your app. It should be set before any SciChartSurface instances are created. A good guide to do this is our FAQ on [Licensing in a DLL](https://www.scichart.com/questions/question/license-in-dll).



