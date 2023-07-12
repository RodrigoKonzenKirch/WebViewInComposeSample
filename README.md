# WebViewInComposeSample
Sample app that shows a webView in Compose

As of 2023, there is no native implementation of WebView in Compose.
The solution is to use the factory AndroidView() that wraps a View in a Composable.

Basic steps to have a webpage running in Composable:

1. Add Internet permission in AndroidManifest:
   <uses-permission android:name="android.permission.INTERNET"/>

2.  Setup a webview using the AndroidView() factory. Optionally: Make changes to the Webview layout inside the factory using layoutParams.

3.  Pass in the Url to be loaded.

4.  Done. We have a Webpage up and running.
  
To add more advanced features, it can be implemented in the Composable, outside the factory, like any other Composable component. 
