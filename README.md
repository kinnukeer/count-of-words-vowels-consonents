# count-of-words-vowels-consonents
a=input().split()
wc=len(a)
vc=0
cc=0
v="aeiouAEIOU"
for i in a:
  for j in i:
    if j.isalpha():
      if j in v:
        vc=vc+1
      else:
        cc=cc+1
print(wc,vc,cc)

#for test cases
t=int(input())
v="aeiouAEIOU"
for _ in range(t):
  s=input()
  vc=0
  cc=0
  for i in s:
    if i.isalpha():
      if i in v:
        vc=vc+1
      else:
        cc=cc+1
  a=s.split()
  wc=len(a)
print(wc,vc,cc)
