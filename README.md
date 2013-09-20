# CEF widget

This is a widget that embed https://code.google.com/p/cefpython into a Kivy widget.
Works currently only on linux 64bits with python 2.7.

This project shouldn't considered stable. There are major things (ex. popups) which aren't implemented or causing proplems.
Tested on Ubuntu 12.04 with the follwoing debian packages installed: libnss3-1d libnspr4-0d


# Example

    from kivy.garden.cefpython import CefBrowser, cefpython
    from kivy.app import App

    class CefBrowserApp(App):
        def build(self):
            return CefBrowser(start_url='http://kivy.org')

    CefBrowserApp().run()
    
    cefpython.Shutdown()


# Hints

Don't use browser.Navigate() to chang the url. Use the function change_url(url) instead.
Read in '__init__.py' at function change_url() why.
