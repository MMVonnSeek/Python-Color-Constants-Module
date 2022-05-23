# Python-Color-Constants-Module
For Pygame and other graphics work, it’s helpful to have color constants that hold the color RGB values. I created a color_constants module that:


1 - Contains constants for 551 named colors* (e.g, as named tuples:


Color = namedtuple('RGB','red, green, blue')


2 - Extends the Color class to include a method for getting the hex formatted color:


class RGB(Color):

def hex_format(self):

return '#{:02X}{:02X}{:02X}'.format(self.red,self.green,self.blue)


3 - Stores these constants in an OrderedDict.
