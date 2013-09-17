# CEF widget

This is a widget that embed https://code.google.com/p/cefpython into a Kivy widget.

More informations to come.

# Example

	from kivy.garden.cefpython import CefBrowser

    class CefBrowserApp(App):
        def build(self):
            return CefBrowser(start_url='http://kivy.org')

    CefBrowserApp().run()
    
    cefpython.Shutdown()
