# set_fun-and-call_fun-
闭包和装饰器详解

def set_fun(func):
    def call_fun(*args, **kwargs):
        return func(*args, **kwargs)
    return call_func
    
@set_fun  # @set_fun ==>> test = set_fun(test)
def test():
    pass  # 函数体
test()  # 调用内部函数
