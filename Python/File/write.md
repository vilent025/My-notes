"""
f = open('python','w')

f.write("hello world")

f.flush  #内容刷新，内容写进文件
"""

f = open("test.txt", 'w')

f.write("hello world")

f.flush()

f.close()  #自带flush功能
