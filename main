p,q,e,M = int(input("輸入質數p: ")), int(input("輸入質數q: ")), int(input("輸入公鑰e: ")), str(input("輸入要加密的訊息M: "))
n = p*q

array = []
if(len(M) % 2 == 1):
  M = M + " "
for i in range(0,len(M),2):
  now = ord(M[i]) - ord('A')
  next = ord(M[i+1]) - ord('A')
  if(M[i] == ' '):
    now = 26
  if(M[i+1] == ' '):
    next = 26      
  array.append(now * 100 + next)
print("訊息: ",array)

c = []
for i in range(len(array)):
  temp = pow(array[i], e, n)
  c.append(temp)
print("密文: ,c")

d = int(input("請輸入私鑰d: "))
m = []
for i in range(len(c)):
  temp = pow(c[i], d, n)
  m.append(temp)
print("解密成功!After decoding是: ",m)
