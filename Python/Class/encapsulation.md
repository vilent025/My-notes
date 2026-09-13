class Phone:

    __current_voltage = None  #私有成员变量， 要以两个下划线开头

    def __init__(self, current_voltage):  #私有成员函数同理
        self.__current_voltage = current_voltage
