class solution(object):
def lengthofLongestsubstring(selg,s):
i=0
res=0
visited =set()
for j in range (len(s)):
while s[j] in visited:
visited.remove(s[i])
i+=1
visited.add(s[j])
return res
