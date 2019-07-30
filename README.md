def add(x, y):
    ans = x ÷ y
    return ans

n = add(3, 5)
print n             #=> 8



class MyError(Exception):
    def __init__(self, value):
        self.value = value
    def __str__(self):
        return repr(self.value)

try:
    raise MyError('my error happens')
except MyError as e:
    print(type(e))
    print(e)
    
<class '__main__.MyError'>
'my error happens'



 str1='This is a pen.'
 str1.split()
['This', 'is', 'a', 'pen.']


str2 = 'desk chair 机　椅子'　（半角スペースと全角スペースがある）
str2.split()
['desk', 'chair', '机', '椅子'] 



3x+5y=100
y=(100-3x)/5 (1≦x≦33)

なので

for x in range(1,34):
if (100-3＊x) % 5 == 0:
y=(100-3＊x) // 5
print(f'(x,y)=({x},{y})')



for i in range(0,10,2):
    print(i)
    
range(最初の数,最後の数-1,ステップ数)



b'   spacious   '.rstrip()
b'   spacious'
b'mississippi'.rstrip(b'ipz')
b'mississ'

b'   spacious   '.rstrip()

b'mississippi'.rstrip(b'ipz')
