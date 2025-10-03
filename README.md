# Create-_UI.
class window_button:
    def paint(self):
        pass
class window_checkbox:
    def paint(self):
        pass
class mac_button:
    def paint(self):
        pass
class mac_checkbox:
    def paint(self):
        pass
class window_factory:
    def create_button(self):
        return window_button()
    def create_checkbox(self):
        return window_checkbox()
class mac_factory:
    def create_button(self):
        return mac_button()
    def create_checkbox(self):
        return mac_checkbox()
def create_ui(factory):
    button=factory.create_button()
    checkbox=factory.create_checkbox()
    print(button.paint())
    print(checkbox.paint())
create_ui(window_factory())
create_ui(mac_factory())
        
