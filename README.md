# Research-Repository-
Assessment 3
class Calculateaverage:
    def calculate_average(numbers):
        if len(numbers) == 0:
            return 0 # Return 0 if the list is empty
        else: 
            return sum(numbers) / len(numbers) # Calculate the average
             
    numbers = [15,25,35,45,55,65]
    average = calculate_average(numbers)
    print("Average", average)  

# KISS (Keep It Simple, Stupid) The value of simplicity in design and problem-solving is emphasized by the KISS (Keep It Simple, Stupid) approach. By making the code clear and concise, we adhere to the KISS principle in this method. The average is produced by the function calculate_average, which accepts a list of values as input. If the list is empty, it first determines whether to return 0 or not. Otherwise, the sum and len functions are used to get the average. 
# This code adheres to the KISS principle by avoiding needless complexity like excessive error handling or duplicative calculations. It focuses on providing a clear and straightforward solution to the fundamental issue of finding the average of a set of numbers.



# With DRY principle
def calculate_area(length, width=None):
    if width is None:
        return length * length  # Calculate area of a square
    else:
        return length * width   # Calculate area of a rectangle
    print(calculate_area)

# In the first  set of functions, we adhere to the DRY principle by using a single function, calculate_area, which, depending on the quantity of parameters, may determine the areas of both rectangles and squares. This adheres to the DRY principle and lessens code duplication.


# Without DRY principle
def calculate_area_of_rectangle(length, width):
    return length * width

def calculate_area_of_square(side):
    return side * side

# A software development philosophy called DRY (Don't Repeat Yourself) promotes reuse of code and lessens duplication in software systems. The DRY principle's core idea is to refrain from writing the same code or logic more than once within your codebase. Instead, make an effort to only develop code once and reuse it as often as possible. This improves maintainability, lowers the chance of errors, and increases the effectiveness of the codebase.

class FileManager:
    def __init__(self, file_name):
        self.file_name = file_name

    def read_file(self):
        self.read_file = read_file
        #c Code for reading the file
        
    def write_file(self, data):
        self.write_file = write_file
        # Code for writing to the file 
# FileManager has two methods for reading data and writing data in to a file and its SR is file managment

class DataProcessor:
    def process_data(self, data):
        self.process_data = process_data
        # Code for processing data 
        
    def save_data(self, data):
        self.save_data = save_data
        # Code for saving data 
# DataProcessor has two methods for processig data and saving data in to a file and its SR is data processing. 
# Following the single responsibility principle by categorizing these duties into two distinct classes. As a result of this division, the code is simpler to maintain and comprehend because each class has a specific and defined purpose.

