# CEF widget

This is a widget that embed https://code.google.com/p/cefpython into a Kivy widget.
Works currently only on linux 64bits with python 2.7.

More informations to come.

# Example

    from kivy.garden.cefpython import CefBrowser, cefpython
    from kivy.app import App

    class CefBrowserApp(App):
        def build(self):
            return CefBrowser(start_url='http://kivy.org')

    CefBrowserApp().run()
    
    cefpython.Shutdown()
